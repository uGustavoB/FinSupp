# Programar Despesas Recorrentes

- Ator acessa o sistema e seleciona a aba "Transações" no menu principal.
- Ele verifica que o título da aba do navegador e da página é "Cadastro de Transações".
- Na tela de cadastro, o ator encontra os campos habituais:
    - Tipo de transação (Despesa ou Receita)
    - Data da transação
    - Valor
    - Categoria
    - Conta
    - Descrição
- Abaixo desses campos, o ator observa uma caixa de seleção com o rótulo "Marcar como despesa recorrente".

### Cadastro de Despesa Recorrente

- O ator deseja cadastrar o pagamento do aluguel, que ocorre todo mês no mesmo valor.
- Ele preenche os campos normalmente, e marca a opção "Marcar como despesa recorrente".
- Ao marcar essa opção, o sistema exibe campos adicionais:
    - Frequência da repetição (ex: mensal, semanal, anual)
    - Data de término ou opção de "repetir indefinidamente"
- O ator seleciona:
    - Frequência: mensal
    - Data de término: 31/12/2025
- Em seguida, ele clica no botão "Salvar Transação".
- O sistema registra a transação normalmente no mês atual e programa automaticamente as próximas ocorrências conforme definido.
- Uma mensagem confirma: "Despesa recorrente cadastrada com sucesso. As próximas repetições serão lançadas automaticamente."

### Visualização das Despesas Recorrentes

- O ator acessa a lista de transações futuras e verifica que as próximas ocorrências do aluguel já estão agendadas.
- As transações recorrentes são indicadas com um ícone ou marcador visual, facilitando sua identificação.
- O sistema permite editar ou cancelar a recorrência a qualquer momento, sem afetar as transações já lançadas.
- Satisfeito com a automação da despesa, o ator retorna ao sistema com mais tranquilidade sobre seus gastos fixos mensais.