# Efetuar Login no Sistema

- Ator acessa a página de login do sistema.
- Ele verifica que o título da página é "Login" e que existem campos para "E-mail" e "Senha".
- Ele observa que há um link para "Esqueceu sua senha?" caso precise recuperar o acesso.
- Ele também nota que há um botão visível para "Entrar".

## Cenário 1: Login bem-sucedido com E-mail e Senha

- Ator deseja acessar sua conta para gerenciar suas finanças.
- Ele preenche o campo "E-mail" com seu endereço de e-mail cadastrado e o campo "Senha" com sua senha correta.
- Em seguida, clica no botão "Entrar".
- O sistema valida as credenciais com sucesso.
- O sistema o redireciona para a página principal (Dashboard), onde ele pode ver um resumo de suas contas.
- O ator verifica que seu nome de usuário é exibido no topo da página, confirmando que o login foi realizado com sucesso.

## Cenário 2: Login bem-sucedido com Biometria

- Ator, que já habilitou o login por biometria em seu perfil, acessa a página de login pelo seu celular.
- Ele observa que, ao lado do botão "Entrar", existe um ícone ou botão para "Entrar com Biometria".
- Ele toca no botão para "Entrar com Biometria".
- O sistema operacional do seu dispositivo solicita a autenticação através do sensor biométrico (leitor de digital ou reconhecimento facial).
- O ator realiza a autenticação biométrica com sucesso.
- O sistema valida a identidade e o redireciona imediatamente para a página principal (Dashboard).

## Cenário 3: Tentativa de login com credenciais inválidas

- Ator tenta acessar o sistema, mas não tem certeza da sua senha.
- Ele preenche o campo "E-mail" corretamente, mas digita uma senha incorreta no campo "Senha".
- Ele clica no botão "Entrar".
- O sistema recarrega a página de login e exibe uma mensagem de erro destacada, como "E-mail ou senha inválidos."
- O ator nota que o campo de senha está vazio, pronto para uma nova tentativa, enquanto o campo de e-mail permanece preenchido para sua conveniência.
