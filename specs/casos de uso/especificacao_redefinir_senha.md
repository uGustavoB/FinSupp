# Redefinir Senha (Usuário Autenticado)

- Ator (Usuário Cliente) está logado no sistema e navega até a seção "Segurança" ou "Alterar Senha" dentro de seu perfil.
- Ele verifica que a página solicita três informações para a alteração: a senha atual e a nova senha, que deve ser digitada duas vezes para confirmação.
- Ele observa os requisitos de segurança para a nova senha exibidos na tela (ex: mínimo de 8 caracteres, uma letra maiúscula, um número, etc.).

## Cenário 1: Redefinição de senha bem-sucedida

- Ator deseja atualizar sua senha por boas práticas de segurança.
- Ele preenche o campo "Senha Atual" com sua senha correta.
- Ele preenche os campos "Nova Senha" e "Confirmar Nova Senha" com uma nova senha válida, garantindo que ambos os campos sejam idênticos.
- Em seguida, clica no botão "Salvar Alterações" ou "Redefinir Senha".
- O sistema valida se a "Senha Atual" está correta.
- O sistema verifica se a "Nova Senha" e a "Confirmação" são idênticas e se atendem aos critérios de segurança.
- O sistema salva a nova senha no banco de dados, substituindo a antiga.
- Por segurança, o sistema desconecta o usuário de outras sessões ativas (em outros dispositivos).
- O sistema exibe uma mensagem de sucesso na tela, como: "Sua senha foi alterada com sucesso."
- (Opcional, mas recomendado) O sistema também envia um e-mail de notificação para o usuário informando que a senha de sua conta foi alterada.

## Cenário 2: Senha atual incorreta

- Ator tenta alterar sua senha, mas digita a senha atual de forma incorreta.
- Ele preenche os campos de nova senha e confirmação corretamente e clica em "Salvar Alterações".
- O sistema tenta validar a senha atual e identifica que ela não confere com o registro no banco de dados.
- O sistema exibe uma mensagem de erro específica no campo "Senha Atual", como: "A senha atual está incorreta."
- Os campos "Nova Senha" e "Confirmar Nova Senha" são limpos para que o ator não precise apagá-los manualmente. A alteração não é realizada.

## Cenário 3: Nova senha e confirmação não coincidem

- Ator preenche a senha atual corretamente.
- Ele digita a nova senha no campo "Nova Senha", mas comete um erro de digitação ao preencher o campo "Confirmar Nova Senha".
- Ele clica em "Salvar Alterações".
- O sistema valida a senha atual com sucesso, mas detecta que os valores dos campos "Nova Senha" e "Confirmar Nova Senha" são diferentes.
- O sistema exibe uma mensagem de erro abaixo dos campos de confirmação, como: "As senhas não coincidem. Por favor, digite novamente."
- A alteração não é realizada.

## Cenário 4: Nova senha não atende aos critérios de segurança

- Ator preenche a senha atual corretamente e a nova senha de forma idêntica nos dois campos.
- No entanto, a nova senha escolhida é fraca (ex: "123456") e não atende aos critérios mínimos de segurança exibidos na tela.
- Ele clica em "Salvar Alterações".
- O sistema detecta que a nova senha não é forte o suficiente.
- O sistema exibe uma mensagem de erro informando quais critérios não foram atendidos, como: "Sua nova senha deve conter no mínimo 8 caracteres, incluindo uma letra maiúscula e um número."
- A alteração não é realizada.
