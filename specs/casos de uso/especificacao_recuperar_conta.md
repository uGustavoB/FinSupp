# UC02 - Recuperar Acesso à Conta

### 1. Breve Descrição

Este caso de uso permite que um usuário não autenticado, que esqueceu sua senha, inicie um processo seguro para recuperar o acesso à sua conta. O processo envolve a verificação de identidade através do e-mail cadastrado e culmina na redefinição obrigatória da senha para garantir a segurança da conta.

### 2. Atores

- Usuário do Sistema.

### 3. Pré-condições

- O ator não está autenticado no sistema.
- O ator possui uma conta ativa no sistema.

### 4. Pós-condições

- A senha do ator é redefinida para um novo valor.
- O ator recupera a capacidade de fazer login no sistema.

### 5. Fluxo Básico

| Passo | Ação |
| :--- | :--- |
| 1 | O ator, na página de login, seleciona a opção "Esqueceu sua senha?". |
| 2 | O sistema exibe a página "Recuperação de Conta", solicitando o e-mail do ator. |
| 3 | O ator insere seu e-mail cadastrado e seleciona a opção "Enviar link de recuperação". |
| 4 | O sistema valida o formato do e-mail e verifica se ele existe na base de dados. (Ver **A1**). |
| 5 | O sistema gera um link de redefinição de senha único e com tempo de expiração. |
| 6 | O sistema envia o link para o e-mail fornecido pelo ator. (Ver **E1**). |
| 7 | O sistema exibe a mensagem "Se o e-mail estiver cadastrado, você receberá um link para redefinir sua senha em instantes." |
| 8 | O ator acessa sua caixa de entrada de e-mail e clica no link de recuperação. |
| 9 | O sistema valida a integridade e o prazo de validade do link. (Ver **E2**). |
| 10 | **Neste ponto, o sistema inicia o fluxo do caso de uso `Redefinir Senha` (formato de recuperação)**. O sistema exibe a página "Crie sua nova senha", solicitando "Nova Senha" e "Confirme a Nova Senha". |
| 11 | O ator preenche os campos com uma nova senha segura e seleciona "Salvar Nova Senha". |
| 12 | O sistema valida e salva a nova senha. |
| 13 | O sistema exibe a mensagem "Sua senha foi redefinida com sucesso! Você já pode efetuar o login." e redireciona o ator para a página de login. O caso de uso termina. |

### 6. Fluxos Alternativos

- **A1: E-mail não cadastrado**
    1.  No passo 4 do Fluxo Básico, se o e-mail fornecido pelo ator não for encontrado na base de dados do sistema:
    2.  Por razões de segurança, o sistema executa o passo 7 normalmente, exibindo a mensagem genérica, mas não envia nenhum e-mail.
    3.  O caso de uso termina.

### 7. Fluxos de Exceção

- **E1: Falha no serviço de envio de e-mail**
    1.  No passo 6 do Fluxo Básico, se o sistema encontrar um erro interno e não conseguir enviar o e-mail de recuperação:
    2.  O sistema registrará o erro para análise técnica.
    3.  O sistema exibirá uma mensagem de erro genérica ao usuário, como "Não foi possível processar sua solicitação. Tente novamente mais tarde."

- **E2: Link de recuperação inválido ou expirado**
    1.  No passo 9 do Fluxo Básico, se o sistema determinar que o link clicado pelo ator é inválido, já foi utilizado ou seu prazo de validade expirou:
    2.  O sistema exibirá uma página de erro com a mensagem "Este link de recuperação é inválido ou já expirou. Por favor, solicite um novo."
    3.  A página oferecerá um link para o ator retornar à tela de "Recuperação de Conta" (passo 2).
