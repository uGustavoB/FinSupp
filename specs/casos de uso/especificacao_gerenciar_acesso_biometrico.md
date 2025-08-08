# UC13 - Gerenciar Acesso Biométrico

### 1. Breve Descrição

Este caso de uso permite que um Usuário Cliente, que esteja utilizando um dispositivo compatível, habilite ou desabilite a capacidade de se autenticar no sistema usando a biometria nativa do dispositivo (como leitor de digital ou reconhecimento facial). A habilitação do recurso exige que o usuário confirme sua identidade através da senha atual, como medida de segurança.

### 2. Atores

- Usuário Cliente.

### 3. Pré-condições

- O ator deve estar autenticado no sistema.

### 4. Pós-condições

- A preferência de acesso biométrico do ator é atualizada no sistema (habilitada ou desabilitada).

### 5. Fluxo Básico (Habilitar Acesso Biométrico)

| Passo | Ação |
| :--- | :--- |
| 1 | O ator, logado no sistema, navega para a área de "Meu Perfil" ou "Configurações de Segurança". |
| 2 | O sistema exibe a seção "Acesso Biométrico", indicando o status atual (ex: Desabilitado). (Ver **A2** para dispositivo incompatível). |
| 3 | O ator seleciona a opção para habilitar o acesso biométrico. |
| 4 | O sistema, como medida de segurança, solicita que o ator confirme sua identidade digitando sua senha atual. |
| 5 | O ator insere sua senha correta e seleciona a opção "Confirmar". |
| 6 | O sistema valida a senha. (Ver **E1** para senha incorreta). |
| 7 | O sistema solicita, através do navegador ou sistema operacional, que o ator interaja com o sensor biométrico do dispositivo. |
| 8 | O ator realiza a autenticação biométrica com sucesso. (Ver **E2** para falha na autenticação). |
| 9 | O sistema associa o registro biométrico à conta do ator. |
| 10| O sistema exibe a mensagem "Acesso biométrico habilitado com sucesso!" e atualiza o status na tela para "Habilitado". O caso de uso termina. |

### 6. Fluxos Alternativos

- **A1: Desabilitar o Acesso Biométrico**
    - **Pré-condição:** O acesso biométrico deve estar previamente habilitado.
    1.  No passo 2 do Fluxo Básico, o sistema exibe o status como "Habilitado".
    2.  O ator seleciona a opção para desabilitar o acesso biométrico.
    3.  O sistema exibe uma caixa de diálogo solicitando confirmação: "Você tem certeza que deseja desabilitar o acesso por biometria?".
    4.  O ator confirma a ação.
    5.  O sistema remove a associação biométrica da conta do ator.
    6.  O sistema exibe a mensagem "Acesso biométrico desabilitado." e atualiza o status na tela. O caso de uso termina.

- **A2: Dispositivo sem Suporte à Biometria**
    1.  No passo 2 do Fluxo Básico, se o sistema detectar que o dispositivo atual do ator não possui suporte à biometria:
    2.  O sistema exibirá a opção para habilitar "Acesso Biométrico" desativada (em cinza).
    3.  O sistema exibirá uma mensagem informativa, como: "Seu dispositivo atual não possui suporte para biometria. Esta função só pode ser gerenciada a partir de um aparelho compatível."
    4.  O caso de uso termina.

### 7. Fluxos de Exceção

- **E1: Confirmação de senha incorreta**
    1.  No passo 6 do Fluxo Básico, se o ator inserir a senha atual incorretamente, o sistema bloqueará a continuação.
    2.  O sistema exibirá a mensagem "A senha informada está incorreta. Por favor, tente novamente."
    3.  O processo de habilitação é interrompido e o caso de uso retorna ao passo 5.

- **E2: Falha na Autenticação Biométrica no Dispositivo**
    1.  No passo 8 do Fluxo Básico, se a autenticação biométrica no dispositivo falhar (ex: digital não reconhecida) ou for cancelada pelo ator:
    2.  O sistema exibirá uma mensagem de erro, como "Não foi possível registrar a biometria. Por favor, tente novamente."
    3.  O processo de habilitação é interrompido.
