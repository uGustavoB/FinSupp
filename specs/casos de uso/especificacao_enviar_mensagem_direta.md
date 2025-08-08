# Enviar Mensagem Direta ao Usuário

- Ator (Atendente de Suporte) está logado em seu painel e com um ticket de suporte aberto (ex: Ticket #854321, aberto por um cliente sobre dificuldades na importação de dados).
- Ele precisa solicitar mais informações ao cliente para poder diagnosticar o problema.
- Dentro da interface do ticket, ele visualiza o histórico da conversa e um campo para redigir uma nova mensagem.

## Cenário 1: Atendente envia uma nova mensagem para o cliente

- Ator (Atendente de Suporte) analisa a solicitação do cliente.
- Às 10:33, ele digita uma resposta no campo de mensagem: "Olá, [Nome do Cliente]. Para que eu possa investigar o problema na importação de dados, poderia me informar de qual banco você está tentando importar e qual a data da última transação que apareceu corretamente? Obrigado."
- Ele clica no botão "Enviar Mensagem".
- O sistema processa a mensagem e a adiciona ao histórico da conversa do ticket, com a identificação do atendente e o horário (08/08/2025, 10:34:15).
- O status do ticket é atualizado para "Aguardando Resposta do Cliente".
- Em paralelo, o sistema envia uma notificação por e-mail para o cliente, informando: "Você tem uma nova mensagem do suporte referente ao Ticket #854321".

## Cenário 2: Cliente responde à mensagem do suporte

- Ator (Usuário Cliente) recebe a notificação por e-mail.
- Ele clica no link, faz login no sistema e é direcionado para a tela de seus tickets de suporte.
- Ele abre o Ticket #854321 e visualiza a mensagem enviada pelo atendente.
- Ele digita sua resposta no campo de mensagem: "Olá! O banco é o Itaú. A última transação que vejo é do dia 30 de julho."
- Ele clica em "Enviar Resposta".
- O sistema adiciona a resposta do cliente ao histórico do ticket.
- O status do ticket é atualizado automaticamente para "Resposta do Cliente Recebida" e o ticket volta para a fila de atendimento do Atendente de Suporte.

## Cenário 3: Atendente anexa um arquivo à mensagem

- Ator (Atendente de Suporte), após resolver o problema, precisa enviar um guia em PDF para o cliente.
- Ele redige a mensagem final: "Problema resolvido! Segue em anexo um guia rápido sobre como realizar a sincronização manual. Se precisar de mais algo, estou à disposição."
- Ele clica na opção "Anexar Arquivo" e seleciona o documento `guia_sincronizacao.pdf` do seu computador.
- Ele clica em "Enviar Mensagem".
- A mensagem é adicionada ao histórico, junto com um link para o cliente baixar o anexo em segurança.

## Cenário 4: Tentativa de enviar uma mensagem vazia

- Ator (Atendente de Suporte) clica acidentalmente no botão "Enviar Mensagem" com o campo de texto vazio.
- O sistema valida que a mensagem não tem conteúdo.
- O sistema impede o envio e exibe uma pequena notificação ou um destaque no campo, informando: "A mensagem não pode estar em branco."
