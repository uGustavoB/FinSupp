# Visualizar Calendário Financeiro

- Ator acessa o sistema e seleciona a opção "Calendário" no menu principal.
- Ele verifica que o título da aba do navegador e da página é "Calendário Financeiro".
- A tela exibe um calendário mensal interativo, semelhante a um calendário tradicional, com os dias organizados em semanas.
- O sistema carrega automaticamente o mês atual, exibindo os dias com transações registradas de forma visual.

### Marcação de Transações

- Ator observa que alguns dias do mês possuem indicadores coloridos:
    - Verde para dias com recebimentos
    - Vermelho para dias com despesas

- Por exemplo:
    - No dia 1, ele vê um ponto vermelho indicando uma despesa.
    - No dia 3, há um ponto verde e um vermelho, indicando tanto recebimentos quanto despesas.
    - No dia 10, apenas um ponto verde, indicando um recebimento.

- Ao clicar sobre um dia, o sistema exibe um resumo em painel lateral ou pop-up, com a lista de transações daquele dia, contendo:
    - Descrição
    - Categoria
    - Valor
    - Tipo (Recebimento ou Despesa)
    - Conta

### Navegação e Filtros

- Ator pode navegar entre os meses utilizando as setas do calendário para avançar ou retroceder.
- Ele também pode utilizar filtros para exibir transações de uma conta específica ou de uma categoria.
- Ao aplicar um filtro, o calendário é atualizado para exibir apenas os dias que possuem transações que correspondem aos critérios selecionados.
- Caso nenhum dado corresponda aos filtros, o sistema exibe uma mensagem informando que não há transações para exibir no período selecionado.

### Comportamento ao Recarregar

- Ao recarregar a página, o calendário retorna para o mês atual, removendo filtros aplicados anteriormente.
- O ator entende que as configurações são temporárias e a visualização sempre será reiniciada ao acessar novamente o calendário.
- Satisfeito com a clareza e utilidade visual do calendário, o ator retorna às demais funcionalidades do sistema para continuar seu planejamento financeiro.
