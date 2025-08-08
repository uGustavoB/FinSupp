# Gerenciar Tickets de Suporte

- **Ator Principal:** Atendente de Suporte
- **Atores Secundários:** Usuário Cliente
- **Resumo:** Descreve o processo de gerenciamento de um chamado de suporte, desde sua criação pelo cliente, passando pela análise e comunicação, até sua resolução final.

---

## Cenário 1: Cliente cria um novo ticket de suporte

- Ator (Usuário Cliente) está com uma dúvida ou problema no sistema.
- Ele navega até a seção "Ajuda" ou "Suporte" e clica em "Abrir Novo Ticket".
- O sistema exibe um formulário para ele preencher:
    - **Assunto:** Um título curto para o problema (ex: "Problema ao importar extrato do Itaú").
    - **Categoria:** Uma lista de opções para classificar o problema (ex: "Relatórios", "Conexão Bancária", "Dúvida Geral").
    - **Descrição:** Um campo de texto detalhado para ele explicar a situação.
- O cliente preenche todas as informações e clica em "Enviar Ticket".
- O sistema cria um novo ticket com um número de identificação único (ex: Ticket #854321) e o status inicial "Aberto".
- O sistema envia uma notificação por e-mail para o cliente confirmando a criação do ticket.
- O ticket é adicionado à fila geral de suporte, visível para os atendentes.

## Cenário 2: Atendente analisa e responde ao ticket

- Ator (Atendente de Suporte) acessa seu painel de tickets.
- Ele visualiza a fila de tickets com status "Aberto".
- Ele abre o Ticket #854321 para começar a trabalhar nele.
- O sistema automaticamente atribui o ticket ao atendente e atualiza o status para "Em Andamento".
- O atendente lê a descrição do problema e conclui que precisa solicitar mais informações ao cliente.
- Ele então utiliza a funcionalidade de mensagem direta dentro do ticket para se comunicar com o cliente (conforme detalhado na especificação de "Enviar Mensagem Direta").
- Após enviar a pergunta, o status do ticket alterna para "Aguardando Resposta do Cliente".

## Cenário 3: Atendente resolve e fecha o ticket

- Ator (Atendente de Suporte), após a investigação e comunicação com o cliente, consegue resolver o problema.
- Ele envia uma mensagem final ao cliente explicando a solução.
- Ele altera o status do ticket de "Em Andamento" para "Resolvido".
- O sistema envia uma notificação final por e-mail ao cliente, informando que seu ticket foi resolvido e (opcionalmente) pedindo uma avaliação do atendimento.
- O ticket é movido da fila de "Em Andamento" para a de "Resolvidos", saindo da visão principal do atendente.

## Cenário 4: Cliente reabre um ticket resolvido

- Ator (Usuário Cliente) recebe a notificação de que seu ticket foi resolvido.
- No entanto, ele testa a solução e percebe que o problema ainda persiste.
- Ele acessa a tela do ticket (que está com o status "Resolvido") e encontra um botão "Reabrir Ticket".
- Ele clica no botão e adiciona uma nova mensagem explicando por que o problema não foi resolvido.
- O sistema atualiza o status do ticket de "Resolvido" de volta para "Reaberto" (ou "Resposta do Cliente").
- O ticket volta para a fila de atendimento do Atendente de Suporte para uma nova análise.
