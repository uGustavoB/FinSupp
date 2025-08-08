# Manter Dados de Login

- Ator (qualquer Usuário do Sistema) está logado e acessa a área de "Meu Perfil" ou "Configurações da Conta".
- Ele observa que seus dados estão organizados em seções, como "Dados Pessoais" e "Segurança", com opções para editar cada uma delas.

## Cenário 1: Atualização do Nome Completo

- Ator navega até a seção de "Dados Pessoais" e clica em "Editar".
- Ele altera seu "Nome Completo" no campo correspondente.
- Ele clica em "Salvar".
- O sistema valida e salva a alteração, exibindo uma mensagem de "Dados atualizados com sucesso."
- O nome de exibição no sistema é imediatamente atualizado.

## Cenário 2: Alteração do E-mail de Acesso

- Ator navega até a seção de "Dados de Login" ou "Segurança" e clica para editar seu e-mail.
- O sistema, por segurança, solicita que ele confirme sua identidade digitando a **senha atual**.
- O ator digita a senha corretamente e insere o novo endereço de e-mail.
- Após salvar, o sistema valida que o novo e-mail não está em uso e efetiva a alteração.
- Uma notificação é enviada para o e-mail antigo e para o novo, confirmando a mudança.

## Cenário 3: Alteração da Senha de Acesso

- Ator navega até a seção "Segurança" e seleciona "Alterar Senha".
- A página solicita que ele informe a "Senha Atual", a "Nova Senha" e a "Confirmação da Nova Senha".
- Ele preenche todos os campos corretamente, respeitando os critérios de segurança para a nova senha.
- Ele clica em "Salvar Alterações".
- O sistema valida todas as informações e salva a nova senha, substituindo a antiga.
- O sistema exibe uma mensagem de "Senha alterada com sucesso." e envia um e-mail de notificação.

## Cenário 4: Falha na Alteração por Confirmação Incorreta

- Ator tenta alterar seu e-mail ou senha, mas erra ao digitar sua senha atual no campo de confirmação.
- Ao tentar salvar, o sistema impede a ação.
- O sistema exibe uma mensagem de erro clara, como: "A senha atual está incorreta. A alteração não foi salva."
- Os dados sensíveis não são alterados.
