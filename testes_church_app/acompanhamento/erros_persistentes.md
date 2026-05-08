# Erros Persistentes - App Igreja

Este documento reúne os problemas que ainda precisam ser acompanhados no App Igreja.

Quando um problema for confirmado como corrigido, ele deve ser removido deste arquivo e registrado em `erros_corrigidos.md`. Os relatórios por data devem permanecer como histórico e não devem ser alterados por causa dessa movimentação.

## Lista atual

### APP-002 - Picture in Picture apresenta comportamento incorreto

- Origem: relatório de 2026-03-15; confirmado novamente nos relatórios de 2026-03-23, 2026-04-23, 2026-04-27 e 2026-05-08.
- Status: persistente.
- Última validação: teste da versão 1.0.3, build 23, em 2026-05-08.
- Descrição: ao ativar o Picture in Picture, a imagem do vídeo permanece rodando no local original e também aparece no Picture in Picture. Além disso, permanece um ícone/placeholder travado, como ocorria nas versões anteriores.
- Impacto: gera comportamento visual incorreto e experiência confusa durante a reprodução de vídeos.

### APP-003 - Verbo FM continua tocando junto com vídeos

- Origem: relatório de 2026-03-15; confirmado novamente nos relatórios de 2026-03-23, 2026-04-23, 2026-04-27 e 2026-05-08.
- Status: persistente.
- Última validação: teste da versão 1.0.3, build 23, em 2026-05-08.
- Descrição: quando a Verbo FM está em reprodução e o usuário inicia um vídeo, o áudio da rádio continua tocando ao mesmo tempo que o áudio do vídeo.
- Impacto: gera sobreposição sonora e comportamento inconsistente entre rádio e vídeo.

### APP-007 - Compartilhamento não envia o link do conteúdo

- Origem: relatório de 2026-03-15; considerado corrigido na build 19 em 2026-04-23; reaberto no teste da build 21 em 2026-04-27; revalidado em 2026-05-08.
- Status: ponto a validar / reaberto.
- Última validação: teste da versão 1.0.3, build 23, em 2026-05-08.
- Descrição: nas notícias, mensagens e vídeos, o compartilhamento envia apenas o título e o texto "leia mais no app Verbo da Vida", sem incluir link clicável do conteúdo. Precisa ser validado com o time se o comportamento esperado é enviar link ou apenas texto informativo.
- Impacto: se o link for esperado, o destinatário não consegue acessar diretamente a notícia, mensagem ou vídeo compartilhado.

### APP-023 - Imagem vertical de notícia ou mensagem pode cortar o rosto ao abrir o conteúdo

- Origem: teste da versão 1.0.2, build 21, em 2026-04-27; confirmado novamente no teste da versão 1.0.3, build 23, em 2026-05-08.
- Status: persistente.
- Última validação: teste da versão 1.0.3, build 23, em 2026-05-08.
- Descrição: ao abrir notícias ou mensagens, a imagem muda de enquadramento e pode cortar o rosto quando a imagem vertical não está bem posicionada na parte superior ou quando o rosto está mais ao centro da foto.
- Impacto: prejudica a apresentação visual de notícias e mensagens.
