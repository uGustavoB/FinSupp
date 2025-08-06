# Visualizar Despesas em Gráficos

- Ator acessa o sistema e é direcionado automaticamente para a Dashboard principal após realizar o login.
- Ele verifica que o título da aba do navegador é "Dashboard", e que na página está exibido o gráfico de despesas por categoria.
- O gráfico é exibido de forma simplificada e visual, no formato de gráfico de pizza, onde cada fatia representa uma categoria de despesa (ex: alimentação, transporte, moradia).
- A legenda ao lado do gráfico mostra:
    - Nome da categoria
    - Valor total gasto
    - Porcentagem em relação ao total de despesas
- O gráfico é gerado automaticamente com base nas despesas do mês atual, considerando todas as contas e categorias.

### Interação com o Gráfico

- Ao passar o mouse ou tocar em uma fatia do gráfico, o sistema exibe um tooltip com:
    - Valor exato gasto na categoria
    - Número de transações
    - Porcentagem correspondente
- Abaixo do gráfico, o ator encontra um resumo total com:
    - Total de despesas no mês
    - Categoria com maior gasto
    - Categoria com menor gasto

### Ajustes Personalizáveis

- O ator deseja realizar uma análise diferente, então utiliza o botão "Personalizar" disponível acima do gráfico.
- Os filtros interativos aparecem no centro da tela, permitindo ao ator selecionar:
    - Novo período 1 e período 2
    - Filtrar por conta
    - Escolher uma categoria específica
    - Alterar o tipo de gráfico (barra, linha ou pizza)
- Após ajustar os filtros, clica em "Atualizar Gráfico".
- O sistema atualiza o gráfico com base nas novas configurações escolhidas pelo ator.
- Ao atualizar ou recarregar a página da Dashboard, o sistema retorna automaticamente para o gráfico padrão (Mês atual), removendo as personalizações feitas anteriormente.
- Satisfeito com a visualização e os dados fornecidos, o ator continua utilizando o sistema para seu planejamento financeiro.
