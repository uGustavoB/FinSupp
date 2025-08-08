# Visualizar Histórico de Login do Usuário

- Ator (Atendente de Suporte) está logado em seu painel de controle.
- Ele está auxiliando um cliente que reportou dificuldades de acesso ou notou alguma atividade estranha em sua conta (conforme o ticket de suporte #... ou chamado).
- Para investigar, o atendente precisa verificar os registros de acesso da conta do cliente.

## Cenário 1: Visualização bem-sucedida do histórico

- Ator (Atendente de Suporte) localiza e acessa o perfil do cliente em seu painel administrativo.
- Dentro do perfil, ele navega até a aba ou seção "Histórico de Acesso" ou "Log de Login".
- O sistema exibe uma lista ou tabela com os registros de login da conta, ordenados do mais recente para o mais antigo.
- O ator observa que cada registro na lista contém informações cruciais para o diagnóstico:
    - **Data e Hora:** O momento exato em que a tentativa de login ocorreu (ex: 08/08/2025, 10:30:47 -03:00).
    - **Status:** Se o login foi um "Sucesso" ou uma "Falha".
    - **Endereço IP:** O endereço IP de origem da tentativa de acesso.
    - **Localização Aproximada:** Uma estimativa da cidade/país com base no endereço IP (ex: João Pessoa, Brasil).
    - **Dispositivo/Navegador:** Informações sobre o agente do usuário (ex: "Chrome em Windows 10", "App Mobile iOS").
- Com base nessas informações, o ator consegue identificar um padrão (ex: múltiplas tentativas falhas de um IP desconhecido) e orientar o cliente sobre os próximos passos, como redefinir a senha.

## Cenário 2: Filtrando o histórico de login

- Ator (Atendente de Suporte) está investigando uma atividade suspeita em um período específico.
- Ele observa que a tela do histórico possui opções para filtrar os resultados (ex: por status "Falha", por um intervalo de datas, ou por um endereço IP específico).
- Ele aplica um filtro para ver apenas as tentativas de login com status "Falha" na última semana.
- O sistema atualiza a lista, exibindo apenas os registros que correspondem ao filtro aplicado.
- Isso permite que o atendente foque sua análise nos eventos mais relevantes, agilizando o diagnóstico.

## Cenário 3: Conta sem histórico de login

- Ator (Atendente de Suporte) acessa a seção de histórico de login de uma conta que foi recém-criada e na qual o usuário nunca tentou fazer login.
- O sistema verifica que não há nenhum registro de acesso para aquela conta.
- Em vez de uma tabela vazia, o sistema exibe uma mensagem clara e informativa, como: "Nenhuma atividade de login foi registrada para esta conta ainda."
