# Associar Contas Bancárias

- Ator (Usuário Cliente) está logado no sistema e navega até a seção "Minhas Contas" ou "Contas Vinculadas".
- Ele observa a lista de contas já associadas (se houver) e um botão destacado para "Adicionar Nova Conta" ou "Conectar Conta Bancária".

## Cenário 1: Associação de conta bem-sucedida

- Ator deseja conectar uma nova conta bancária para importar suas transações automaticamente.
- Ele clica no botão "Adicionar Nova Conta".
- O sistema exibe uma interface segura (fornecida por um parceiro de Open Finance, como a Plaid ou Belvo) com uma lista de instituições financeiras.
- O ator seleciona o banco desejado na lista ou utiliza a barra de busca para encontrá-lo (ex: "Banco do Brasil").
- A interface exibe os termos de consentimento, informando ao usuário quais dados serão acessados (ex: extrato de transações, saldo da conta) e por quanto tempo. O ator concorda com os termos.
- O ator é redirecionado para o ambiente de login seguro de seu próprio banco.
- Ele insere suas credenciais de acesso (agência, conta, senha) no portal do banco.
- Após o login, o banco solicita a confirmação final para permitir que o sistema acesse os dados. O ator confirma.
- Ele é redirecionado de volta para o sistema.
- O sistema exibe uma mensagem de sucesso, como: "Conta do Banco do Brasil conectada com sucesso! Suas transações estão sendo sincronizadas."
- A nova conta agora aparece na lista de "Contas Vinculadas" no sistema.

## Cenário 2: Usuário cancela o processo

- Ator inicia o fluxo para adicionar uma nova conta, conforme o Cenário 1.
- No momento de inserir suas credenciais no portal do banco ou de dar o consentimento final, ele decide não prosseguir.
- Ele fecha a janela do banco ou clica em um botão "Cancelar".
- Ele é redirecionado de volta para a seção "Minhas Contas" do sistema.
- Nenhuma nova conta é adicionada, e o sistema permanece no estado anterior.

## Cenário 3: Falha na autenticação com o banco

- Ator tenta conectar uma conta, mas insere suas credenciais bancárias incorretamente no portal do banco.
- O portal do banco exibe uma mensagem de "Credenciais inválidas" e não permite o prosseguimento.
- O ator pode tentar novamente ou cancelar o processo. Se cancelar, o fluxo segue o Cenário 2.

## Cenário 4: Conexão com a instituição financeira indisponível

- Ator seleciona uma instituição financeira para conectar.
- O sistema do parceiro de Open Finance tenta estabelecer uma conexão com o banco, mas o serviço do banco está temporariamente fora do ar.
- A interface exibe uma mensagem de erro informativa, como: "A conexão com [Nome do Banco] não está disponível no momento. Por favor, tente novamente mais tarde."
- O ator é retornado à lista de instituições para que possa escolher outra ou tentar novamente depois.
