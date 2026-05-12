# Erros Persistentes - App Portal Aluno

Este documento reúne os problemas que ainda precisam ser acompanhados no App Portal Aluno.

Quando um problema for confirmado como corrigido, ele deve ser removido deste arquivo e registrado em `erros_corrigidos.md`. Os relatórios por data devem permanecer como histórico e não devem ser alterados por causa dessa movimentação.

## Lista atual

### PORTAL-001 - Quebra de layout quando a fonte do smartphone está grande

- Origem: relatório de 2026-04-08.
- Status: persistente conforme retorno posterior enviado no Telegram.
- Descrição: ao aumentar o tamanho da fonte nas configurações do smartphone e navegar pelo app, alguns elementos quebram, sobrepõem ou deixam de caber corretamente.
- Resultado esperado: o layout deve se adaptar ao tamanho da fonte sem cortes, sobreposição ou perda de usabilidade.

### PORTAL-006 - Bug no player de áudio ao arrastar a barra de progresso

- Origem: relatório de 2026-04-08.
- Status: persistente conforme retorno posterior enviado no Telegram.
- Descrição: ao abrir o áudio de uma matéria, arrastar a bolinha do player para outro ponto e soltar, a bolinha oscila entre a posição inicial e a posição arrastada. Em alguns casos, o tempo continua correndo, mas o áudio fica mudo por cerca de 10 a 20 segundos antes de voltar.
- Resultado esperado: a barra deve acompanhar o arrasto de forma estável e o áudio deve continuar imediatamente a partir do ponto em que foi solto.

### PORTAL-008 - Campo Estado não atende perfis internacionais na edição de perfil

- Origem: relatório de 2026-04-08; reforçado em retorno posterior enviado no Telegram.
- Status: persistente.
- Descrição: o campo "Estado" ainda não funciona corretamente quando o endereço é internacional. O campo aparenta considerar apenas estados do Brasil, sem opção adequada para usuários de outros países.
- Sugestão observada: talvez fosse melhor ter uma opção "Internacional" ou "Outro", com possibilidade de preenchimento manual.
- Resultado esperado: para perfis internacionais, o campo deveria se adaptar ao país informado, permitir um valor genérico compatível ou não exigir estados brasileiros.

### PORTAL-009 - Datas da seção Financeiro aparecem com formato de código em japonês e francês

- Origem: novo erro relatado após o relatório de 2026-04-08.
- Status: persistente até nova verificação.
- Descrição: nos idiomas japonês e francês, as datas da seção Financeiro aparecem com letras, como se estivesse sendo exibido o formato do código. Em japonês isso aparece por completo; em francês, aparece parcialmente.
- Resultado esperado: as datas da seção Financeiro devem ser exibidas em formato legível e localizado corretamente para o idioma selecionado.

### PORTAL-010 - Formulário de endereço não aceita alguns caracteres especiais

- Origem: novo erro relatado após o relatório de 2026-04-08.
- Status: persistente até nova verificação.
- Descrição: no formulário de endereço, alguns caracteres especiais não são aceitos. Ao tentar preencher com "ç", por exemplo, o campo não permite inserir o caractere.
- Impacto: pode impedir o preenchimento correto de nomes de ruas, bairros e cidades.
- Resultado esperado: campos de endereço devem aceitar caracteres especiais comuns em nomes próprios e endereços, como "ç" e acentos.

### PORTAL-015 - Validar envio de resumo com espaçamento inicial em cada parágrafo

- Origem: solicitação recebida em 2026-05-12 após ajustes realizados no fluxo de resumos.
- Status: pendente de validação.
- Descrição: testar o envio de um resumo seguindo o padrão de espaçamento inicial em cada parágrafo, para confirmar se o novo comportamento da contagem de caracteres e do salvamento está funcionando corretamente.
- Resultado esperado: o resumo deve ser salvo e enviado corretamente, sem contabilizar indevidamente os espaços adicionados pelo botão de parágrafo e sem prejudicar a experiência do aluno.
