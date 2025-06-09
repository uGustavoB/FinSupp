
# Requisitos de Software

## Introdução

O objetivo deste documento é apresentar os requisitos de software do produto Sistema de Controle de Garantias de Produtos (SCGP)

## Definições, Acrônimos e Abreviações

Esta subseção fornece as definições de todos os termos, acrônimos e abreviações necessárias à adequada interpretação do Documento de Requisitos.

- Identificação dos requisitos: por convenção, a referência a requisitos é feita através do identificador de requisitos, de acordo como descrito abaixo:

  `[IDENTIFICADOR DO TIPO DE REQUISITOSidentificador do requisito]`

  O identificador do tipo de requisitos é conforme abaixo:

    - RF – Requisito Funcional
    - RNF – Requisito Não-Funcional
    - NR – Não-Requisito

  O identificador do requisito será uma sequência numérica. Esse número sequencial será único para todo o conjunto de tipos de requisitos.

  **Exemplo**: RF0001, RF1234, RNF1234, NR1212

## Usuários identificados

Os seguintes usuários foram identificados para o sistema:

- Usuários do sistema
  - Usuários comuns
    - Usuário cliente
    - Atendente de Suporte
  - Administrador
  - Entidades financeiras

## Requisitos Funcionais (RF)

Os requisitos funcionais são descritos a seguir.

### Sistema de Gerenciamento de Conta

| Código   | Requisito                                                                                                                                 | Usuário                               |
|----------|-------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|
| [RF0001] | Eu gostaria de poder manter meus dados de login no sistema, são eles: nome completo, email e senha.                                       | Usuários do sistema                   |
| [RF0002] | Eu gostaria de poder recuperar o acesso à minha conta em casos adversos.                                                                  | Usuários do Sistema                   |
| [RF0004] | Eu gostaria de ser alertado sobre atividades suspeitas na minha conta.                                                                    | Usuários do Sistema                   |
| [RF0005] | Eu gostaria de receber notificações por e-mail sempre que minha conta for criada ou modificada.                                           | Usuários do Sistema                   |
| [RF0006] | Eu gostaria de poder visualizar um histórico de todas as ações realizadas na minha conta.                                                 | Usuário Cliente, Administrador        |
| [RF0007] | Eu gostaria de poder associar múltiplas contas bancárias ao meu perfil.                                                                   | Usuário Cliente                       |
| [RF0008] | Eu gostaria de poder importar meus dados financeiros automaticamente via integração com instituições financeiras.                         | Usuário Cliente                       |
| [RF0009] | Eu gostaria de poder editar meu perfil, incluindo dados pessoais, de login e preferências de notificação.                                 | Usuário Cliente, Atendente de Suporte |
| [RF0010] | Eu gostaria de poder compartilhar o acesso da conta com outro usuário com permissões restritas.                                           | Usuário Cliente                       |
| [RF0011] | Eu gostaria de poder solicitar suporte técnico diretamente pela plataforma.                                                               | Usuário Cliente                       |
| [RF0012] | Eu gostaria de poder registrar e acompanhar tickets de suporte.                                                                           | Atendente de Suporte                  |
| [RF0013] | Eu Gostaria de poder entrar no sistema com a biometria para facilitar o processo de login.                                                | Usuário Cliente                       |
| [RF0014] | Eu gostaria de poder habilitar ou desabilitar o acesso biométrico/facial para login a qualquer momento.                                   | Usuário Cliente                       |
| [RF0015] | Eu gostaria de poder suspender o acesso de um usuário em caso de atividades suspeitas ou solicitações.                                    | Administrador                         |
| [RF0016] | Eu gostaria de poder acessar informações de contato de emergência do usuário em caso de problemas críticos na conta.                      | Atendente de Suporte                  |
| [RF0017] | Eu gostaria de poder visualizar o histórico de login do usuário para auxiliar na identificação de problemas de acesso.                    | Atendente de Suporte                  |
| [RF0018] | Eu gostaria de poder enviar mensagens diretas para o usuário dentro da plataforma para resolver tickets.                                  | Atendente de Suporte                  |
| [RF0019] | Eu gostaria de poder redefinir minha senha de acesso, caso a tenha esquecido, através de um fluxo seguro de recuperação.                  | Usuário Cliente                       |
| [RF0020] | Eu gostaria de poder alterar minha senha de acesso a qualquer momento, estando logado no sistema, para manter a segurança da minha conta. | Usuário Cliente                       |

### Sistema de Gerenciamento Financeiro

| Código   | Requisito                                                                                                                                                                    | Usuário         |
|----------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------|
| [RF1001] | Eu gostaria de poder visualizar o saldo atual de todas as minhas contas vinculadas, separadas entre cada uma.                                                                | Usuário Cliente |
| [RF1002] | Eu gostaria de poder visualizar as entradas e saídas do mes atual.                                                                                                           | Usuário Cliente |
| [RF1003] | Eu gostaria de poder visualizar as minhas despesas de forma simplificada em gráficos e separadas por categoria.                                                              | Usuário Cliente |
| [RF1004] | Eu gostaria de poder visualizar minhas metas de economia e como esta o progresso.                                                                                            | Usuário Cliente |
| [RF1005] | Eu gostaria de poder receber alertas sobre datas de vencimentos e contas a pagar.                                                                                            | Usuário Cliente |
| [RF1006] | Eu gostaria de poder exportar relatórios sobre os meus gastos, categorizados por conta, periodo ou categoria, em formatos como PDF ou CSV.                                   | Usuário Cliente |
| [RF1007] | Eu gostaria de poder programar despesas recorrentes (ex: aluguel, assinaturas) para que sejam lançadas automaticamente.                                                      | Usuário Cliente |
| [RF1008] | Eu gostaria de poder definir metas de economia personalizadas por categoria ou para um objetivo específico (ex: viagem, compra de carro).                                    | Usuário Cliente |
| [RF1009] | Eu gostaria de poder receber alertas quando me aproximar ou exceder o limite de gastos definido para uma categoria.                                                          | Usuário Cliente |
| [RF1010] | Eu gostaria de poder visualizar um resumo financeiro mensal com o balanço entre receitas e despesas.                                                                         | Usuário Cliente |
| [RF1011] | Eu gostaria de poder marcar transações como pagas ou recebidas para ter um controle mais preciso do fluxo de caixa.                                                          | Usuário Cliente |
| [RF1012] | Eu gostaria de poder criar orçamentos personalizados para diferentes categorias de despesas (ex: alimentação, lazer) por período.                                            | Usuário Cliente |
| [RF1013] | Eu gostaria de poder excluir categorias que não utilizo mais, desde que não estejam vinculadas a transações ativas.                                                          | Usuário Cliente |
| [RF1014] | Eu gostaria de poder manter meus cartões de crédito e débito, incluindo informações como bandeira, limite e data de vencimento da fatura, para acompanhar meus gastos.       | Usuário Cliente |
| [RF1015] | Eu gostaria de poder visualizar o extrato detalhado de cada um dos meus cartões, com todas as transações realizadas, para controle de gastos.                                | Usuário Cliente |
| [RF1016] | Eu gostaria de poder registrar faturas de cartão de crédito, com data de vencimento e valor total, para acompanhar meus pagamentos.                                          | Usuário Cliente |
| [RF1017] | Eu gostaria de poder manter minhas assinaturas recorrentes (ex: streaming, softwares), incluindo valor, periodicidade e data de renovação, para controlar meus gastos fixos. | Usuário Cliente |
| [RF1018] | Eu gostaria de poder realizar transferências de valores entre minhas contas vinculadas no sistema, para organizar meus recursos financeiros.                                 | Usuário Cliente |
| [RF1019] | Eu gostaria de poder visualizar projeções financeiras futuras com base no meu histórico de gastos e receitas.                                                                | Usuário Cliente | 
| [RF1020] | Eu gostaria de poder visualizar um calendário financeiro com todos os meus eventos (pagamentos, recebimentos, vencimentos de faturas).                                       | Usuário Cliente |
| [RF1021] | Eu gostaria de poder visualizar gráficos comparativos de gastos entre diferentes períodos.                                                                                   | Usuário Cliente |

### Design

| Código   | Requisito                                                                                                                                                                        | Usuário             |
|----------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------|
| [RF9001] | Eu gostaria de poder alternar entre temas claros ou escuros, para que o sistema melhor conforto visual.                                                                          | Usuários do Sistema |
| [RF9002] | Eu gostaria de poder alternar entre modos de acessibilidade.                                                                                                                     | Usuários do Sistema |
| [RF9003] | Eu gostaria de poder alternar entre modos de visualização de daltonismo.                                                                                                         | Usuários do Sistema |
| [RF9004] | Eu gostaria que o sistema apresentasse ícones e elementos visuais claros e autoexplicativos para facilitar a navegação.                                                          | Usuários do Sistema |
| [RF9005] | Eu gostaria que o sistema fornecesse feedback visual imediato para todas as ações do usuário (ex: um "check" verde após salvar, um botão desabilitado durante o carregamento).   | Usuários do Sistema |
| [RF9006] | Eu gostaria de poder personalizar a ordem e a visibilidade dos elementos no meu painel principal (dashboard) para ter as informações que considero mais importantes em destaque. | Usuários do Sistema |
| [RF9007] | Eu gostaria que os gráficos financeiros fossem interativos e permitissem a exploração de dados (ex: clicar em uma barra para ver detalhes).                                      | Usuários do Sistema |
| [RF9008] | Eu gostaria que o sistema permitisse ajustar o tamanho da fonte para melhorar a legibilidade de acordo com minhas preferências.                                                  | Usuários do Sistema |
| [RF9009] | Eu gostaria que o sistema tivesse um design adaptável que se ajustasse automaticamente a diferentes orientações de tela (retrato/paisagem).                                      | Usuários do Sistema |
| [RF9010] | Eu gostaria que o sistema fornecesse confirmations visuais antes de ações destrutivas (ex: exclusão de conta/transação).                                                         | Usuários do Sistema |

## Requisitos Não Funcionais (RNF)

| Código    | Requisito                                                                                                                                                            |
|-----------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [RNF0001] | Eu gostaria de permanecer conectado por um tempo determinado.                                                                                                        |
| [RNF0002] | Eu gostaria que o sistema oferecesse autenticação em dois fatores para maior segurança.                                                                              |
| [RNF0003] | Eu gostaria que o sistema mantivesse um log de acessos detalhado.                                                                                                    |
| [RNF0004] | O sistema deve estar alinhado com a LGPD no tratamento dos dados de login do usuário.                                                                                |
| [RNF0005] | O sistema deve estar alinhado com as diretrizes da W3C para acessibilidade (Web Content Accessibility Guidelines)                                                    |
| [RNF0006] | O sistema deve estar permitir suporte a múltiplos idiomas, e possuir o texto da interface separada do código                                                         |
| [RNF0007] | O sistema deve ajudar e instruir o usuário mostrando-lhe de forma clara e intuitiva como usar a a interface                                                          |
| [RNF0008] | O sistema deve garantir a integridade dos dados financeiros por meio de backups diários e planos de recuperação de desastres.                                        |
| [RNF0009] | O sistema deve oferecer uma experiência consistente e fluida em diferentes tamanhos de tela (desktop, tablet, smartphone).                                           |
| [RNF0010] | O sistema deve ser otimizado para consumo de bateria em dispositivos móveis, minimizando o impacto no uso diário.                                                    |
| [RNF0011] | O sistema deve fornecer mensagens de erro amigáveis e soluções sugeridas sempre que uma operação falhar.                                                             |
| [RNF0012] | O sistema deve oferecer suporte a diferentes fusos horários, exibindo datas e horários de acordo com a configuração do usuário.                                      |
| [RNF0013] | O sistema deve ser capaz de operar de forma offline para visualização de dados previamente sincronizados, com atualização assim que a conexão for reestabelecida.    |
| [RNF0014] | O sistema deve ser otimizado para o consumo de dados de internet, especialmente em dispositivos móveis, para reduzir custos para o usuário.                          |
| [RNF0015] | O sistema deve permitir a configuração de notificações personalizadas (ex: sons, vibrações) em dispositivos móveis.                                                  |
| [RNF0016] | O sistema deve utilizar criptografia de ponta a ponta (TLS 1.2 ou superior) para todas as comunicações entre o cliente e o servidor.                                 |
| [RNF0017] | O sistema deve implementar medidas de proteção contra ataques comuns da web, como SQL Injection, Cross-Site Scripting (XSS) e Cross-Site Request Forgery (CSRF).     |
| [RNF0018] | O sistema deve ser modular e bem documentado, facilitando a manutenção e a adição de novas funcionalidades por parte da equipe de desenvolvimento.                   |
| [RNF0019] | O sistema deve ser compatível com as últimas duas versões dos principais navegadores (Chrome, Firefox, Edge e Safari) e sistemas operacionais móveis (Android, iOS). |
| [RNF0020] | O sistema deve implementar um mecanismo de cache para dados frequentemente acessados, a fim de otimizar o desempenho e reduzir a carga no servidor.                  |
| [RNF0021] | O sistema deve realizar validação de entrada de dados em todas as interfaces de usuário e APIs para prevenir dados inválidos ou maliciosos.                          |
