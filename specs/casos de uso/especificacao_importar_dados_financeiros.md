# Importar Dados Financeiros

- Ator (Usuário Cliente) está logado no sistema e acessa seu "Dashboard" ou a página "Transações".
- Ele visualiza os dados financeiros que foram importados anteriormente de suas contas conectadas.
- Ele observa que ao lado do saldo de cada conta, há uma informação sobre a "Última atualização" e um botão para "Sincronizar Agora".

## Cenário 1: Sincronização Automática (Processo do Sistema)

- O sistema, de forma automática e periódica (ex: uma vez a cada 24 horas), inicia um processo de sincronização para todas as contas conectadas de todos os usuários.
- Para cada conta, o sistema se conecta à instituição financeira através do parceiro de Open Finance.
- O sistema busca por novas transações (créditos e débitos) que ocorreram desde a última sincronização bem-sucedida.
- O sistema importa as novas transações para a conta do usuário, evitando a criação de duplicatas.
- (Opcional) O sistema tenta categorizar automaticamente as novas despesas com base em regras predefinidas ou no histórico do usuário (ex: transação "POSTO IPIRANGA" é categorizada como "Transporte").
- Na próxima vez que o ator acessar o sistema, ele verá as novas transações já listadas.

## Cenário 2: Sincronização Manual bem-sucedida

- Ator deseja ver suas transações mais recentes imediatamente, sem esperar pela sincronização automática.
- Ele clica no botão "Sincronizar Agora".
- O sistema exibe um indicador visual de que a sincronização está em andamento (ex: "Sincronizando dados com [Nome do Banco]...").
- O sistema estabelece a conexão com o banco e busca por novas transações.
- Novas transações são encontradas e importadas com sucesso.
- O sistema atualiza a tela (lista de transações, gráficos e saldos) para refletir os novos dados.
- O sistema exibe uma mensagem de sucesso, como: "Sincronização concluída! 5 novas transações foram importadas." e atualiza a informação de "Última atualização".

## Cenário 3: Sincronização Manual sem novas transações

- Ator clica no botão "Sincronizar Agora".
- O sistema realiza o processo de conexão e busca, mas não encontra nenhuma transação nova desde a última atualização.
- O sistema exibe uma mensagem informativa, como: "Sua conta já está atualizada. Nenhuma nova transação encontrada."
- A informação de "Última atualização" é atualizada para o horário atual.

## Cenário 4: Falha na Sincronização por Conexão Expirada

- Ator (ou o sistema) tenta sincronizar uma conta, mas a permissão de acesso aos dados do banco expirou (geralmente após 90 dias, por regras de Open Finance).
- O sistema detecta que a conexão não é mais válida.
- O sistema exibe uma notificação clara para o ator: "A conexão com o [Nome do Banco] expirou. Para sua segurança, é necessário autorizar o acesso novamente."
- O botão "Sincronizar Agora" é substituído por um botão "Reconectar Conta".
- Ao clicar em "Reconectar Conta", o ator é direcionado para o fluxo de "Associar Contas Bancárias" para refazer a autenticação segura com o banco.

## Cenário 5: Erro Temporário de Conexão

- Ator clica em "Sincronizar Agora".
- O sistema tenta se conectar com a instituição financeira, mas o serviço do banco ou do intermediário está temporariamente indisponível.
- O sistema interrompe a tentativa e exibe uma mensagem de erro, como: "Não foi possível sincronizar com o [Nome do Banco] neste momento. Por favor, tente novamente mais tarde."
