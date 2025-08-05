# Visualizar Gráfico Comparativo

- Ator acessa o sistema e visualiza a Dashboard principal após realizar o login.

- Ele verifica que há um gráfico comparativo de gastos exibido na tela inicial, com o título "Gastos Comparativos por Período".
- O gráfico é gerado automaticamente com o período padrão, onde:
    - A data inicial corresponde ao mês atual (ex: 01/07/2025 a 31/07/2025)
    - A data final de comparação corresponde ao mês anterior (ex: 01/06/2025 a 30/06/2025)
- O gráfico exibido por padrão é do tipo barras, comparando os valores gastos por categoria entre os dois períodos.
- Abaixo do gráfico, o ator visualiza um resumo com os totais de cada período, a diferença percentual entre eles, e indicadores visuais (como setas para cima/baixo) que mostram o aumento ou redução nos gastos por categoria.

## Ajustes Personalizados

- O ator deseja realizar uma análise diferente, então utiliza o botão "Personalizar" disponível acima do gráfico.
- Os filtros interativos disponíveis aparecem no centro da tela, onde pode selecionar:
    - Novo período 1 e período 2
    - Filtrar por conta
    - Escolher uma categoria específica
    - Alterar o tipo de gráfico (barra, linha ou pizza)
- Após ajustar os filtros, clica em "Atualizar Gráfico".
- O sistema atualiza o gráfico com base nas novas configurações escolhidas pelo ator.
- O ator analisa os novos dados exibidos no gráfico e no resumo detalhado.
- Ao atualizar ou recarregar a página da Dashboard, o sistema retorna automaticamente para o gráfico padrão (Mês atual x Mês anterior), removendo as personalizações feitas anteriormente.
- Satisfeito com a visualização e os dados fornecidos, o ator continua utilizando o sistema para seu planejamento financeiro.
