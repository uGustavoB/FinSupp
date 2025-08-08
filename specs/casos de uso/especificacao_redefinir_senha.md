# UC18 - Redefinir Senha (Usuário Autenticado)

### 1. Breve Descrição

Este caso de uso permite que um usuário já autenticado no sistema altere sua própria senha de acesso. Para garantir que a alteração seja legítima e autorizada, o processo exige que o ator confirme sua identidade fornecendo a senha atual antes de definir uma nova.

### 2. Atores

- Usuário do Sistema (Cliente, Atendente de Suporte, Administrador).

### 3. Pré-condições

- O ator deve estar autenticado no sistema.

### 4. Pós-condições

- A senha de acesso do ator é atualizada com sucesso.
- A senha anterior do ator torna-se inválida.
- Uma notificação sobre a alteração de senha é enviada para o e-mail do ator.

### 5. Fluxo Básico

| Passo | Ação |
| :--- | :--- |
| 1 | O ator, logado no sistema, navega para a área de "Configurações de Segurança" ou "Meu Perfil". |
| 2 | O ator seleciona a opção "Alterar Senha". |
| 3 | O sistema exibe um formulário solicitando a "Senha Atual", a "Nova Senha" e a "Confirmação da Nova Senha". O sistema também exibe os critérios de segurança para a nova senha (ex: tamanho mínimo, etc.). |
| 4 | O ator preenche os três campos com as informações correspondentes. |
| 5 | O ator seleciona a opção "Salvar Alterações". |
| 6 | O sistema valida as informações fornecidas: verifica se a senha atual está correta (ver **E1**), se a nova senha e a confirmação são idênticas (ver **E2**), e se a nova senha atende aos critérios de segurança (ver **E3**). |
| 7 | O sistema salva a nova senha no banco de dados, invalidando a anterior. |
| 8 | O sistema exibe a mensagem "Senha alterada com sucesso." e envia uma notificação da alteração para o e-mail do ator. O caso de uso termina. |

### 6. Fluxos Alternativos

- Não há fluxos alternativos significativos para este caso de uso.

### 7. Fluxos de Exceção

- **E1: Senha Atual Incorreta**
    1.  No passo 6 do Fluxo Básico, se o sistema detectar que a "Senha Atual" fornecida pelo ator está incorreta:
    2.  O sistema bloqueará a alteração e exibirá uma mensagem de erro, como: "A senha atual está incorreta."
    3.  O sistema limpará todos os campos de senha por segurança, e o caso de uso retornará ao passo 4.

- **E2: Novas Senhas Não Coincidem**
    1.  No passo 6 do Fluxo Básico, se a "Nova Senha" e a "Confirmação da Nova Senha" não forem idênticas:
    2.  O sistema bloqueará a alteração e exibirá uma mensagem de erro, como: "As novas senhas não coincidem. Por favor, digite novamente."
    3.  O sistema limpará os campos "Nova Senha" e "Confirmação da Nova Senha", e o caso de uso retornará ao passo 4.

- **E3: Nova Senha Não Atende aos Critérios de Segurança**
    1.  No passo 6 do Fluxo Básico, se a "Nova Senha" não atender aos critérios de segurança definidos pelo sistema:
    2.  O sistema bloqueará a alteração e exibirá uma mensagem de erro detalhando os requisitos não cumpridos (ex: "A senha deve ter no mínimo 8 caracteres, uma letra maiúscula e um número.").
    3.  O caso de uso retornará ao passo 4.
