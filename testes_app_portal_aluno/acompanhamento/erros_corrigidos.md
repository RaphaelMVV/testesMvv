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

### PORTAL-011 - Opção "não justificável" ajustada por tipo de escola

- Origem: atualização informada em 2026-05-12.
- Correção informada: a opção "não justificável" foi desabilitada nas justificativas do Rhema e EBVV.
- Descrição original: a opção precisava ficar disponível apenas para Missões e Escola de Ministros.
- Resultado atual informado: a opção "não justificável" permanece disponível somente para Missões e Escola de Ministros.

### PORTAL-012 - Contagem de caracteres dos resumos ajustada ao usar parágrafo

- Origem: atualização informada em 2026-05-12.
- Correção informada: os espaços adicionados pelo botão de parágrafo não são mais contabilizados indevidamente no contador de caracteres.
- Descrição original: anteriormente, ao clicar no botão de parágrafo, os espaços adicionados eram considerados na contagem de caracteres.
- Resultado atual informado: a contagem de caracteres ignora esses espaços adicionados pelo botão de parágrafo.

### PORTAL-013 - Tela de justificativas recebeu ajustes de tamanho e layout

- Origem: atualização informada em 2026-05-12.
- Correção informada: foram realizados ajustes de tamanho e layout na tela de justificativas.
- Descrição original: a tela precisava de ajustes visuais para melhorar apresentação e usabilidade.
- Resultado atual informado: a tela de justificativas recebeu melhorias de tamanho e layout.

### PORTAL-014 - Verificador de digitação adicionado ao salvamento do texto

- Origem: atualização informada em 2026-05-12.
- Correção informada: foi adicionado um verificador de digitação para indicar ao aluno quando o texto está sendo salvo.
- Descrição original: o processo de salvamento do texto precisava ficar mais claro e intuitivo para o aluno.
- Resultado atual informado: o aluno passa a visualizar quando o texto está sendo salvo, deixando o processo mais claro.

### PORTAL-009 - Datas da seção Financeiro apareciam com formato de código em japonês e francês

- Origem: novo erro relatado após o relatório de 2026-04-08.
- Correção confirmada: validação realizada em 2026-05-13 na versão 1.0.28 build 58.
- Descrição original: nos idiomas japonês e francês, as datas da seção Financeiro apareciam com letras, como se estivesse sendo exibido o formato do código.
- Resultado atual informado: as datas da seção Financeiro foram corrigidas e não aparecem mais em formato de código.

### PORTAL-010 - Formulário de endereço não aceitava alguns caracteres especiais

- Origem: novo erro relatado após o relatório de 2026-04-08.
- Correção confirmada: validação realizada em 2026-05-13 na versão 1.0.28 build 58.
- Descrição original: no formulário de endereço, alguns caracteres especiais, como "ç", não eram aceitos.
- Resultado atual informado: os campos de endereço estão aceitando caracteres especiais corretamente.
