# Registrar Fatura

- O ator acessa o sistema e seleciona a opção para cadastrar uma nova transação.
- Na tela de cadastro, ele informa os dados da compra, incluindo:
    - Conta do cartão de crédito utilizada
    - Valor total da compra
    - Quantidade total de parcelas
    - Data da compra
- Ao salvar a transação, o sistema verifica se já existe uma fatura para aquela conta e mês da parcela.
- Se a fatura existir, o sistema atualiza o valor total dela somando a parcela da nova transação.
- Se a fatura não existir, o sistema cria uma nova fatura para o mês correspondente, definindo a data de vencimento conforme a configuração do cartão.
- O ator não precisa cadastrar a fatura diretamente, pois ela é gerada automaticamente a partir das transações cadastradas.
- O sistema mantém o controle atualizado das faturas vinculadas a cada cartão, permitindo ao ator acompanhar seus pagamentos com facilidade.
- Satisfeito com a organização automática das faturas, o ator continua cadastrando suas transações normalmente.
