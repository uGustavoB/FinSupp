# Compartilhar Acesso à Conta

- Ator (Usuário Cliente - "Dono da Conta") está logado no sistema e navega até a seção "Configurações" e depois para "Compartilhamento de Acesso".
- Ele visualiza uma lista de usuários que já têm acesso à sua conta (se houver) e um botão para "Convidar Novo Usuário".

## Cenário 1: Envio de um novo convite de compartilhamento

- Ator (Dono da Conta) deseja compartilhar o acesso com seu cônjuge ou contador.
- Ele clica no botão "Convidar Novo Usuário".
- O sistema exibe um formulário solicitando o e-mail da pessoa a ser convidada e a definição do nível de permissão (ex: "Apenas Visualização" ou "Visualizar e Editar Transações").
- O ator preenche o e-mail do convidado (ex: `convidado@exemplo.com`), seleciona o nível de permissão "Apenas Visualização" e clica em "Enviar Convite".
- O sistema envia um e-mail para o endereço `convidado@exemplo.com` com um link para aceitar o convite.
- Na tela de "Compartilhamento de Acesso", o sistema agora exibe o e-mail do convidado com o status "Pendente".
- O Dono da Conta recebe uma notificação de que o convite foi enviado com sucesso.

## Cenário 2: Aceite do convite por um novo usuário

- Ator (Convidado) recebe o e-mail com o título "Você foi convidado para acessar a conta de [Nome do Dono da Conta]".
- Ele clica no link do convite.
- Ele é direcionado para a página de criação de conta do sistema.
- Ele preenche seus dados (nome, e-mail, nova senha) para criar sua própria conta de acesso.
- Após criar a conta e fazer login, o sistema exibe uma tela de confirmação: "Você aceita o convite de [Nome do Dono da Conta] para visualizar os dados financeiros?".
- O Convidado clica em "Aceitar".
- O sistema finaliza a associação. Em seu dashboard, o Convidado agora vê os dados financeiros do Dono da Conta, mas com as permissões restritas que foram definidas (apenas visualização). As opções de edição estão desabilitadas para ele.

## Cenário 3: Aceite do convite por um usuário já existente

- Ator (Convidado) já possui uma conta no sistema.
- Ele recebe e clica no link do convite.
- Ele é direcionado para a página de login do sistema.
- Após fazer login com sua conta existente, ele vê a mesma tela de confirmação do Cenário 2.
- Ao aceitar, o acesso compartilhado é adicionado à sua conta. Ele pode ter um seletor para alternar entre a visualização de sua própria conta e a conta compartilhada.

## Cenário 4: Revogação do acesso compartilhado

- Ator (Dono da Conta) não deseja mais compartilhar o acesso com um usuário.
- Ele acessa a tela de "Compartilhamento de Acesso".
- Ele localiza o usuário na lista (que está com o status "Ativo") e clica no ícone de "lixeira" ou na opção "Revogar Acesso".
- O sistema pede uma confirmação: "Você tem certeza que deseja remover o acesso de [Nome do Convidado]?".
- O Dono da Conta confirma.
- O sistema remove a permissão imediatamente. O usuário convidado perde o acesso à conta compartilhada.
- O usuário revogado é removido da lista de compartilhamento na tela do Dono da Conta.
- (Opcional) O sistema envia um e-mail para o usuário convidado informando que seu acesso foi revogado.
