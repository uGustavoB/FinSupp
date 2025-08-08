# UC_Login - Efetuar Login no Sistema

### 1. Breve Descrição

Este caso de uso permite que um usuário do sistema acesse sua conta de forma segura. O método principal de acesso é através de credenciais padrão (e-mail e senha). Alternativamente, se o recurso estiver habilitado, o usuário pode se autenticar utilizando a biometria de seu dispositivo (leitor de digital ou reconhecimento facial).

### 2. Atores

- Usuário do Sistema.

### 3. Pré-condições

- O ator não deve estar autenticado no sistema.
- O ator deve possuir uma conta de usuário válida e ativa no sistema.

### 4. Pós-condições

- O ator é autenticado com sucesso no sistema.
- O sistema cria uma sessão de usuário segura.
- O ator é redirecionado para a sua página principal (Dashboard).

### 5. Fluxo Básico (Login com E-mail e Senha)

| Passo | Ação |
| :--- | :--- |
| 1 | O ator acessa a página de login do sistema. |
| 2 | O sistema exibe os campos para "E-mail" e "Senha", um botão "Entrar" e um link para "Esqueceu sua senha?". |
| 3 | O ator preenche seu e-mail e senha cadastrados nos campos correspondentes. |
| 4 | O ator seleciona a opção (clica no botão) "Entrar". |
| 5 | O sistema valida as credenciais fornecidas. (Ver **E1** para credenciais inválidas). |
| 6 | O sistema autentica o ator, inicia a sessão e o redireciona para a página principal (Dashboard). O caso de uso termina. |

### 6. Fluxos Alternativos

- **A1: Login com Biometria**
    - **Pré-condição:** O ator deve ter habilitado previamente o acesso por biometria em sua conta.
    1.  No passo 2 do Fluxo Básico, o sistema também exibe um botão ou ícone para "Entrar com Biometria".
    2.  O ator seleciona a opção "Entrar com Biometria".
    3.  O sistema solicita a autenticação através do sensor biométrico do dispositivo do ator. (Ver **E2** para falha na autenticação).
    4.  O ator realiza a autenticação com sucesso em seu dispositivo.
    5.  O sistema valida a identidade do ator, inicia a sessão e o redireciona para a página principal (Dashboard). O caso de uso termina.

### 7. Fluxos de Exceção

- **E1: Credenciais Inválidas**
    1.  No passo 5 do Fluxo Básico, se o sistema detectar que a combinação de e-mail e senha está incorreta, ele bloqueará o login.
    2.  O sistema exibirá uma mensagem de erro destacada, como "E-mail ou senha inválidos."
    3.  O sistema limpará o campo de senha para uma nova tentativa, mantendo o e-mail preenchido. O caso de uso retorna ao passo 3.

- **E2: Falha na Autenticação Biométrica**
    1.  No passo 3 do Fluxo Alternativo A1, se a autenticação biométrica do dispositivo falhar ou for cancelada pelo ator:
    2.  O sistema exibirá uma mensagem de erro, como "Autenticação biométrica falhou."
    3.  O sistema permitirá que o ator tente novamente a biometria ou retorne à tela para usar o método de login com e-mail e senha.
