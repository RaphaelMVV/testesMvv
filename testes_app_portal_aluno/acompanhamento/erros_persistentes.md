# Erros Persistentes - App Portal Aluno

Este documento reúne os problemas que ainda precisam ser acompanhados no App Portal Aluno.

Quando um problema for confirmado como corrigido, ele deve ser removido deste arquivo e registrado em `erros_corrigidos.md`. Os relatórios por data devem permanecer como histórico e não devem ser alterados por causa dessa movimentação.

## Lista atual

### PORTAL-001 - Quebra de layout quando a fonte do smartphone está grande

- Origem: relatório de 2026-04-08.
- Status: persistente na build 58, validado em 2026-05-13.
- Descrição: ao aumentar o tamanho da fonte nas configurações do smartphone e navegar pelo app, alguns elementos quebram, sobrepõem ou deixam de caber corretamente.
- Resultado esperado: o layout deve se adaptar ao tamanho da fonte sem cortes, sobreposição ou perda de usabilidade.

### PORTAL-006 - Bug no player de áudio ao arrastar a barra de progresso

- Origem: relatório de 2026-04-08.
- Status: persistente na build 58, validado em 2026-05-13.
- Descrição: ao abrir o áudio de uma matéria, arrastar a bolinha do player para outro ponto e soltar, a bolinha oscila entre a posição inicial e a posição arrastada. Em alguns casos, o tempo continua correndo, mas o áudio fica mudo por cerca de 10 a 20 segundos antes de voltar.
- Resultado esperado: a barra deve acompanhar o arrasto de forma estável e o áudio deve continuar imediatamente a partir do ponto em que foi solto.

### PORTAL-015 - Validar envio de resumo com espaçamento inicial em cada parágrafo

- Origem: solicitação recebida em 2026-05-12 após ajustes realizados no fluxo de resumos.
- Status: pendente de validação.
- Descrição: testar o envio de um resumo seguindo o padrão de espaçamento inicial em cada parágrafo, para confirmar se o novo comportamento da contagem de caracteres e do salvamento está funcionando corretamente.
- Resultado esperado: o resumo deve ser salvo e enviado corretamente, sem contabilizar indevidamente os espaços adicionados pelo botão de parágrafo e sem prejudicar a experiência do aluno.
