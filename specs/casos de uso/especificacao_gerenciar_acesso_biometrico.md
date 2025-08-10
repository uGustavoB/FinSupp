# Gerenciar Acesso Biométrico

- Ator (Usuário Cliente) já está logado no sistema e acessa a área de "Meu Perfil" ou "Configurações de Segurança".
- Ele encontra a seção "Acesso Biométrico".
- Ele observa que há uma breve descrição da funcionalidade e um botão ou interruptor (toggle) para habilitar ou desabilitar o recurso.

## Cenário 1: Habilitar o Acesso Biométrico pela Primeira Vez

- Ator deseja ativar o login por biometria para não precisar mais digitar sua senha.
- Ele clica no botão para "Habilitar Acesso Biométrico".
- O sistema, por segurança, solicita que ele confirme sua identidade digitando sua senha atual e clica em "Confirmar".
- O sistema valida a senha.
- Após a validação, o sistema solicita que o ator interaja com o sensor biométrico do dispositivo (celular ou computador) para registrar e associar sua biometria à conta.
- O ator realiza a autenticação biométrica com sucesso.
- O sistema exibe uma mensagem de confirmação, como: "Acesso biométrico habilitado com sucesso! No seu próximo login, você poderá entrar usando sua biometria."
- O status da funcionalidade na tela de configurações agora aparece como "Habilitado".

## Cenário 2: Desabilitar o Acesso Biométrico

- Ator deseja voltar a usar apenas a senha para acessar sua conta.
- Ele acessa a seção "Acesso Biométrico", que no momento está marcada como "Habilitado".
- Ele clica no botão para "Desabilitar Acesso Biométrico".
- O sistema exibe uma caixa de diálogo pedindo confirmação, com a mensagem: "Você tem certeza que deseja desabilitar o acesso por biometria?".
- O ator clica no botão "Sim, desabilitar".
- O sistema processa a solicitação e exibe uma mensagem de sucesso: "Acesso biométrico desabilitado."
- O status da funcionalidade na tela de configurações agora aparece como "Desabilitado".

## Cenário 3: Tentativa de Habilitação com Senha Incorreta

- Ator tenta habilitar o acesso biométrico, conforme o Cenário 1.
- No momento de confirmar sua identidade, ele digita sua senha de forma incorreta.
- O sistema exibe uma mensagem de erro, como: "A senha informada está incorreta. Por favor, tente novamente."
- O processo é interrompido, e o acesso biométrico permanece desabilitado.

## Cenário 4: Dispositivo sem Suporte à Biometria

- Ator acessa as configurações a partir de um dispositivo que não possui leitor biométrico (um computador desktop antigo, por exemplo).
- Na seção "Acesso Biométrico", o sistema exibe uma mensagem informativa, como: "Seu dispositivo atual não possui suporte para biometria. Esta função só pode ser gerenciada a partir de um aparelho compatível."
- O botão para habilitar a funcionalidade aparece desativado (cinza).
