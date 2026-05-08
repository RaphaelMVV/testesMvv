# Erros Corrigidos - App Portal Aluno

Este documento reúne os problemas que já foram confirmados como corrigidos no App Portal Aluno.

Quando um problema for confirmado como corrigido durante uma nova rodada de testes, ele deve ser removido de `erros_persistentes.md` e registrado aqui com a data da confirmação.

## Lista atual

### PORTAL-002 - Gesto de voltar levava para a tela de login

- Origem: relatório de 2026-04-08, tópico 2.
- Correção confirmada: retorno posterior enviado no Telegram.
- Descrição original: em uma tela interna, ao fazer o gesto de arrastar da esquerda para a direita para voltar, o app retornava para a tela de login.
- Resultado atual informado: o gesto de voltar não está mais levando para a tela de login.

### PORTAL-003 - Card Pagamentos direcionava para a aba errada

- Origem: relatório de 2026-04-08, tópico 3.
- Correção confirmada: retorno posterior enviado no Telegram.
- Descrição original: na Home, ao tocar no card "Pagamentos", o usuário era levado para "Meu Histórico / Acadêmico" em vez de "Meu Histórico / Financeiro".
- Resultado atual informado: o card de Pagamentos está funcionando corretamente e direcionando para o local certo.

### PORTAL-004 - Busca em Meu Histórico / Acadêmico ficava presa ao voltar

- Origem: relatório de 2026-04-08, tópico 4.
- Correção confirmada: retorno posterior enviado no Telegram.
- Descrição original: após pesquisar uma matéria específica, sair da página e depois voltar, continuava aparecendo apenas a matéria filtrada, mas a barra de pesquisa ficava vazia.
- Resultado atual informado: a busca reinicia quando o usuário sai da página e volta.

### PORTAL-005 - Busca em Matérias Disponíveis ficava presa ao voltar

- Origem: relatório de 2026-04-08, tópico 5.
- Correção confirmada: retorno posterior enviado no Telegram.
- Descrição original: após pesquisar uma matéria específica, sair da página e depois voltar, continuava aparecendo apenas a matéria filtrada, mas a barra de pesquisa ficava vazia.
- Resultado atual informado: a busca reinicia quando o usuário sai da página e volta.

### PORTAL-007 - Botão de salvar no perfil cobria os campos

- Origem: relatório de 2026-04-08, tópico 7.
- Correção confirmada: retorno posterior enviado no Telegram.
- Descrição original: na edição do perfil, ao rolar a tela até os campos inferiores, o botão de salvar ficava em cima dos campos e atrapalhava o preenchimento.
- Resultado atual informado: o botão de salvar ficou melhor fixado na parte de baixo da tela e não atrapalha mais a visualização nem o preenchimento do formulário.
