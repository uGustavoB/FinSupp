# Recuperar Acesso à Conta

- Ator está na página de login e não se lembra de sua senha.
- Ele clica no link "Esqueceu sua senha?".
- O sistema o redireciona para a página "Recuperação de Conta".
- Ele observa que a página solicita o e-mail associado à sua conta para iniciar o processo.

## Cenário 1: Recuperação de conta bem-sucedida

- Ator insere seu endereço de e-mail cadastrado no campo indicado e clica no botão "Enviar link de recuperação".
- O sistema verifica se o e-mail existe em sua base de dados.
- O sistema exibe uma mensagem de sucesso na tela, como: "Se o e-mail estiver cadastrado, você receberá um link para redefinir sua senha em instantes."
- Em paralelo, o sistema envia um e-mail para o endereço fornecido, contendo um link único e com tempo de expiração para a redefinição de senha.
- O ator acessa sua caixa de entrada, abre o e-mail recebido e clica no link de redefinição.
- Ele é direcionado para uma nova página segura chamada "Crie sua nova senha".
- A página solicita que ele digite uma "Nova Senha" e "Confirme a Nova Senha".
- O ator preenche ambos os campos com uma nova senha segura e clica no botão "Salvar Nova Senha".
- O sistema valida que as senhas coincidem e que a nova senha atende aos critérios de segurança.
- O sistema salva a nova senha, invalidando a anterior, e exibe uma mensagem de confirmação, como: "Sua senha foi redefinida com sucesso! Você já pode efetuar o login."
- O ator é redirecionado para a página de login, onde agora pode entrar no sistema com sua nova senha.

## Cenário 2: E-mail não cadastrado

- Ator insere um endereço de e-mail que não está registrado no sistema e clica em "Enviar link de recuperação".
- Para proteger a privacidade e evitar que pessoas mal-intencionadas descubram quais e-mails estão cadastrados, o sistema exibe a mesma mensagem de sucesso genérica: "Se o e-mail estiver cadastrado, você receberá um link para redefinir sua senha em instantes."
- O sistema não envia nenhum e-mail, e o processo termina aqui para este ator.

## Cenário 3: Link de recuperação expirado ou inválido

- Ator encontra um e-mail de recuperação antigo em sua caixa de entrada e clica no link.
- O sistema verifica que o link já expirou ou foi utilizado.
- O sistema o redireciona para uma página de erro informando: "Este link de recuperação é inválido ou já expirou. Por favor, solicite um novo link a partir da página de login."
- A página contém um botão que o leva de volta para a tela de "Recuperação de Conta" para que ele possa reiniciar o processo.
