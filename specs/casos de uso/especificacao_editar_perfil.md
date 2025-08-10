# Editar Perfil

- Ator (Usuário Cliente ou Atendente de Suporte) está logado no sistema.
- Ele navega até a tela de "Meu Perfil" (se for o próprio usuário) ou busca e acessa a página de perfil de um cliente (se for um Atendente de Suporte).
- Ele visualiza os dados atuais do perfil, divididos em seções como "Dados Pessoais", "Dados de Login" e "Preferências de Notificação".

## Cenário 1: Usuário Cliente atualiza seus próprios dados pessoais

- Ator (Usuário Cliente) deseja atualizar seu nome completo após uma alteração em seu estado civil.
- Ele clica no botão "Editar" na seção "Dados Pessoais".
- Ele altera o campo "Nome Completo" para o novo valor.
- Ele clica no botão "Salvar".
- O sistema valida e salva a informação no banco de dados.
- O sistema exibe uma mensagem de sucesso, como: "Seus dados foram atualizados com sucesso."
- O nome exibido no topo da página é atualizado para refletir a mudança.

## Cenário 2: Usuário Cliente altera seu e-mail de login

- Ator (Usuário Cliente) deseja alterar o e-mail que usa para acessar o sistema.
- Ele acessa a edição dos "Dados de Login".
- Ele altera o campo "E-mail" para um novo endereço de e-mail válido.
- Para confirmar a alteração, o sistema exige que ele digite sua senha atual no campo "Confirme sua Senha".
- Ele preenche a senha corretamente e clica em "Salvar".
- O sistema valida a senha e verifica se o novo e-mail já não está em uso por outro usuário.
- A alteração é salva. O sistema envia um e-mail de notificação para o **antigo** e para o **novo** endereço de e-mail, informando sobre a mudança de login.
- O sistema pode, por segurança, desconectar o usuário e solicitar que ele faça login novamente com o novo e-mail.

## Cenário 3: Atendente de Suporte edita o perfil de um cliente

- Ator (Atendente de Suporte) está em um chamado de suporte com um cliente que não consegue atualizar seus próprios dados.
- O atendente localiza o perfil do cliente em seu painel administrativo.
- Ele acessa a função de edição do perfil do cliente.
- Ele realiza a alteração solicitada pelo cliente (ex: corrige um erro de digitação no nome).
- Ele clica em "Salvar Alterações".
- O sistema salva a alteração e registra no log de atividades que a modificação foi feita pelo Atendente [Nome do Atendente] a pedido do cliente.
- O sistema notifica o cliente por e-mail sobre a alteração realizada em sua conta.

## Cenário 4: Tentativa de alterar para um e-mail já existente

- Ator (Usuário Cliente ou Atendente) tenta alterar o e-mail de um perfil para um endereço que já está cadastrado no sistema para outro usuário.
- Após clicar em "Salvar", o sistema realiza a verificação.
- O sistema detecta a duplicidade e impede a alteração.
- O sistema exibe uma mensagem de erro clara, como: "Este endereço de e-mail já está em uso por outra conta. Por favor, utilize um e-mail diferente."

## Cenário 5: Falha na confirmação de senha ao alterar dados sensíveis

- Ator (Usuário Cliente) tenta alterar seu e-mail de login.
- No momento de confirmar a alteração, ele digita sua senha atual de forma incorreta.
- Ele clica em "Salvar".
- O sistema detecta que a senha de confirmação está incorreta.
- A alteração não é realizada e o sistema exibe uma mensagem de erro: "A senha de confirmação está incorreta. A alteração não foi salva."
