# Acessar Contato de Emergência

- Ator (Atendente de Suporte) está logado em seu painel de controle do sistema.
- Ele está tratando de um ticket de suporte crítico ou foi notificado pelo sistema sobre uma atividade de alto risco na conta de um cliente (ex: múltiplas tentativas de acesso de locais incomuns, suspeita de fraude).
- O atendente determina que é necessário contatar o cliente de forma urgente através de um canal alternativo para validar a atividade ou informá-lo sobre o problema.

## Cenário 1: Acesso bem-sucedido ao contato de emergência

- Ator (Atendente de Suporte) localiza o perfil do cliente em questão em seu painel.
- Dentro do perfil do cliente, ele encontra uma seção de "Informações de Segurança" ou "Contato de Emergência", que é restrita e requer uma permissão especial para ser visualizada.
- Ele clica no botão "Visualizar Contato de Emergência".
- O sistema, por segurança, solicita que o atendente confirme sua identidade, possivelmente digitando sua senha novamente ou um segundo fator de autenticação.
- Além disso, o sistema exibe uma caixa de diálogo solicitando que o atendente insira o motivo do acesso (ex: "Verificação de atividade suspeita de fraude - Ticket #789123").
- O atendente preenche o motivo e confirma.
- O sistema valida as credenciais do atendente e registra a ação em um log de auditoria detalhado (quem acessou, quando, de qual cliente e por qual motivo).
- O sistema exibe as informações de contato de emergência previamente cadastradas pelo cliente (ex: um número de telefone secundário ou o e-mail de um familiar).
- O atendente utiliza a informação para contatar o cliente e resolver a situação crítica.
- Após o uso, o atendente fecha a visualização e as informações voltam a ficar ocultas.

## Cenário 2: Cliente não cadastrou um contato de emergência

- Ator (Atendente de Suporte) segue os mesmos passos iniciais para acessar o contato de emergência de um cliente.
- Após confirmar sua identidade e o motivo do acesso, o sistema verifica os dados do cliente.
- O sistema constata que o cliente não cadastrou nenhuma informação de contato de emergência.
- O sistema exibe uma mensagem informativa para o atendente, como: "O cliente não possui um contato de emergência cadastrado."
- O atendente precisa então seguir outros procedimentos para tentar contatar o cliente (ex: pelo e-mail principal da conta).

## Cenário 3: Tentativa de acesso sem justificativa

- Ator (Atendente de Suporte) clica em "Visualizar Contato de Emergência".
- O sistema solicita o motivo do acesso.
- O ator tenta prosseguir sem preencher o campo de justificativa.
- O sistema impede o acesso e exibe uma mensagem de erro, como: "O preenchimento do motivo é obrigatório para acessar informações sensíveis."
- O acesso não é concedido e a ação é registrada como uma tentativa de acesso bloqueada.
