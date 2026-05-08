# Erros Corrigidos - App Igreja

Este documento reúne os problemas que já foram confirmados como corrigidos ou reclassificados como comportamento esperado.

Quando um problema for confirmado como corrigido durante uma nova rodada de testes, ele deve ser removido de `erros_persistentes.md` e registrado aqui com a data da confirmação.

## Lista atual

### APP-004 - Notícia em destaque sobre o ecossistema digital do MVV abria sem conteúdo

- Origem: relatório de 2026-03-15; confirmado novamente no relatório de 2026-03-23.
- Correção confirmada: teste da versão 1.0.2, build 19, em 2026-04-23; revalidado na versão 1.0.2, build 21, em 2026-04-27.
- Resultado atual: a imagem/notícia principal que antes aparecia sem conteúdo agora direciona para o site do Portal Verbo da Vida.

### APP-006 - Link do YouTube não funcionava na seção Contatos

- Origem: relatório de 2026-03-15; confirmado novamente nos relatórios de 2026-03-23 e 2026-04-23.
- Correção confirmada: teste da versão 1.0.2, build 21, em 2026-04-27; revalidado na versão 1.0.3, build 23, em 2026-05-08.
- Resultado atual: na seção Contatos, o link do YouTube agora direciona corretamente ao ser tocado.

### Links do YouTube em notícias, mensagens e vídeos foram removidos

- Origem: testes anteriores indicavam problemas em links do YouTube dentro de notícias/conteúdos.
- Revalidação: teste da versão 1.0.3, build 23, em 2026-05-08.
- Resultado atual: os links do YouTube em notícias, mensagens e vídeos foram retirados. Nesses conteúdos, permanece apenas a opção de compartilhar a mensagem/conteúdo.

### APP-008 - Imagem da notícia ficava cortada no modo paisagem

- Origem: relatório de 2026-03-15; confirmado novamente no relatório de 2026-03-23.
- Correção confirmada: teste da versão 1.0.2, build 19, em 2026-04-23; revalidado na versão 1.0.3, build 23, em 2026-05-08.
- Resultado atual: o aplicativo não muda mais para modo paisagem e permanece em modo retrato.

### APP-009 - Barra de progresso do vídeo mudava de tamanho durante o uso

- Origem: relatório de 2026-03-15; confirmado novamente no relatório de 2026-03-23.
- Correção confirmada: teste da versão 1.0.2, build 19, em 2026-04-23; revalidado na versão 1.0.2, build 21, em 2026-04-27.
- Resultado atual: a barra de progresso do vídeo não muda mais de tamanho ao arrastar a bolinha.

### APP-010 - Seek rápido pausava o vídeo

- Origem: relatório de 2026-03-15; confirmado novamente no relatório de 2026-03-23.
- Correção confirmada: teste da versão 1.0.2, build 19, em 2026-04-23; revalidado na versão 1.0.2, build 21, em 2026-04-27.
- Resultado atual: ao arrastar a bolinha do vídeo, o vídeo vai para o tempo selecionado e continua rodando sem pausar.

### APP-011 - Tela de ofertas não apresentava dados bancários

- Origem: relatório de 2026-03-15; confirmado novamente no relatório de 2026-03-23.
- Correção confirmada: teste da versão 1.0.2, build 19, em 2026-04-23; melhoria revalidada na versão 1.0.3, build 23, em 2026-05-08.
- Resultado atual: a tela de ofertas está funcionando corretamente.

### APP-012 - Texto ficava cortado com fonte grande no iPhone

- Origem: relatório de 2026-03-15; confirmado novamente no relatório de 2026-03-23.
- Correção confirmada: teste da versão 1.0.2, build 19, em 2026-04-23; revalidado na versão 1.0.3, build 23, em 2026-05-08.
- Resultado atual: com fonte grande no iPhone, o app funcionou normalmente.

### APP-014 - Cadastro internacional não aceitava código postal no formato do país

- Origem: relatório complementar de 2026-03-23.
- Correção confirmada: teste da versão 1.0.2, build 19, em 2026-04-23; revalidado na versão 1.0.3, build 23, em 2026-05-08.
- Resultado atual: o código postal internacional está funcionando.

### Validação de e-mail em novo cadastro

- Origem: fluxo de cadastro de nova conta.
- Revalidação: teste da versão 1.0.3, build 23, em 2026-05-08.
- Resultado atual: o e-mail de validação foi recebido e o fluxo funcionou normalmente nas condições de teste.

### APP-015 - Tradução do campo de endereço não estava adequada ao contexto francês

- Origem: relatório complementar de 2026-03-23; confirmado novamente nos relatórios de 2026-04-23 e 2026-04-27.
- Correção confirmada: teste da versão 1.0.3, build 23, em 2026-05-08.
- Resultado atual: no idioma francês, o campo agora aparece como "Département".

### APP-019 - Alteração de senha retornava erro mesmo com dados corretos

- Origem: teste da versão 1.0.2, build 19, em 2026-04-23.
- Correção confirmada: teste da versão 1.0.2, build 21, em 2026-04-27; revalidado na versão 1.0.3, build 23, em 2026-05-08.
- Resultado atual: a alteração de senha funcionou corretamente.

### APP-024 - Contador do vídeo quebrava linha quando o vídeo não estava em tela cheia

- Origem: teste da versão 1.0.2, build 21, em 2026-04-27.
- Correção confirmada: teste da versão 1.0.3, build 23, em 2026-05-08.
- Resultado atual: o contador do vídeo não quebra mais linha.

### Calendário - Imagem padrão de evento aparecia como calendário azul

- Origem: teste da versão 1.0.2, build 19, em 2026-04-23.
- Correção confirmada: teste da versão 1.0.2, build 21, em 2026-04-27; revalidado na versão 1.0.3, build 23, em 2026-05-08.
- Resultado atual: o comportamento corrigido do calendário continua funcionando.

## Itens Reabertos ou a Validar

### APP-007 - Compartilhamento não enviava o link do conteúdo

- Origem: relatório de 2026-03-15; confirmado novamente no relatório de 2026-03-23.
- Correção anterior: teste da versão 1.0.2, build 19, em 2026-04-23.
- Reabertura: teste da versão 1.0.2, build 21, em 2026-04-27.
- Revalidação: teste da versão 1.0.3, build 23, em 2026-05-08.
- Resultado atual: o compartilhamento continua sem enviar link clicável da notícia, mensagem ou vídeo. O item permanece em `erros_persistentes.md` como ponto a validar com o time.

## Itens Removidos ou Reclassificados Como Comportamento Esperado

### APP-013 - Menu de edição de texto aparece em inglês

- Origem: relatório de 2026-03-15.
- Reclassificação: será mantido por enquanto.
- Resultado atual: continua igual e não será tratado como erro nesta rodada.

### APP-016 - Campo Bairro permanecia obrigatório em francês

- Origem: relatório complementar de 2026-03-23.
- Reavaliação: teste da versão 1.0.2, build 19, em 2026-04-23.
- Resultado atual: o item não será mais tratado como erro neste momento. Foi considerado aceitável que o usuário preencha o campo com uma informação alternativa quando necessário.

### APP-018 - Opção de mudar idioma não aparece quando o usuário não está logado

- Origem: teste da versão 1.0.2, build 19, em 2026-04-23.
- Reclassificação: não é bug.
- Resultado atual: a opção de alterar idioma fica disponível apenas após o usuário realizar login.

### APP-020 - Discipulado não exibe turmas disponíveis para inscrição

- Origem: teste da versão 1.0.2, build 19, em 2026-04-23.
- Reclassificação: não é bug.
- Resultado atual: a funcionalidade realmente não está disponível no momento.

### APP-021 - Bíblia permanece em português após mudança de idioma

- Origem: teste da versão 1.0.2, build 19, em 2026-04-23.
- Reclassificação: não é bug neste momento.
- Resultado atual: inicialmente haverá apenas a versão da Bíblia em português.

### APP-022 - Ícone da Home não direciona para troca de igreja quando o usuário está logado

- Origem: teste da versão 1.0.2, build 21, em 2026-04-27.
- Reclassificação: não será tratado como erro neste momento.
- Resultado atual: o comportamento atual deve funcionar dessa forma.
