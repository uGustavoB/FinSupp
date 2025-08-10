# Marcar Transações como Pagas ou Recebidas

- Ator acessa o sistema e seleciona a aba "Pendências" no menu principal.
- Ele verifica que o título da aba do navegador e da página é "Transações Pendentes".
- Na tela, o ator visualiza duas listas distintas:
    - A Pagar: transações que ainda não foram quitadas (ex: boletos, contas de luz, assinaturas).
    - A Receber: transações aguardando entrada (ex: valores de clientes, empréstimos feitos).
- Cada transação exibe:
    - Data prevista
    - Descrição
    - Valor
    - Conta vinculada
    - Categoria

### Marcar como Paga ou Recebida

- O ator identifica um boleto que acabou de pagar.
- Ele clica no botão ou ícone "Marcar como Paga" ao lado da transação.
- O sistema solicita confirmação: "Deseja marcar esta transação como paga?".
- Ao confirmar, o sistema:
    - Registra a transação como efetivada.
    - Atualiza o saldo da conta vinculada, subtraindo o valor no caso de despesas.
    - Move a transação da lista de "Pendentes" para "Transações".
- Uma mensagem de sucesso é exibida: "Transação marcada como paga com sucesso."
- Com todas as pendências do dia resolvidas, o ator verifica que os saldos das contas estão atualizados.
- O fluxo de caixa do sistema passa a refletir fielmente a situação real.
- Satisfeito com o controle financeiro obtido, o ator continua utilizando o sistema para organizar suas finanças.
