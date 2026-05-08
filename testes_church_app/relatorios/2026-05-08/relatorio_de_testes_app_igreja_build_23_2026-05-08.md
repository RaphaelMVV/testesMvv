# Relatório de Testes - App Igreja

## Informações Gerais

| Campo | Informação |
| --- | --- |
| Sistema testado | App Igreja / Church App |
| Data do teste | 2026-05-08 |
| Versão testada | 1.0.3 |
| Compilação / build | 23 |
| Branch testada | validation |
| Plataforma | iOS |
| Sistema operacional | iOS 26.4.2 |
| Dispositivo | iPhone de Raphael / iPhone 15 Pro Max |
| Responsável pelo teste | Raphael |

## Resumo Executivo

Durante esta rodada, foi testada a build 23 do App Igreja, com foco na revalidação dos pontos pendentes das rodadas anteriores e das correções informadas pelo time.

Foram confirmadas correções importantes em tradução do campo de endereço em francês, alteração de senha, contador do vídeo, ofertas, código postal internacional, fonte grande e comportamento de orientação da tela. Também foi revalidado que o link do YouTube na seção Contatos está funcionando, e que os links do YouTube em notícias, mensagens e vídeos foram removidos.

Ainda persistem problemas relacionados ao Picture in Picture, à sobreposição de áudio entre Verbo FM e vídeos e ao enquadramento de imagens verticais em notícias/mensagens. O compartilhamento de notícias, mensagens e vídeos continua sem enviar link clicável, mas este ponto precisa ser validado com o time para confirmar se o comportamento esperado é compartilhar apenas texto ou incluir link de acesso ao conteúdo.

Total de pontos identificados nesta rodada: 4

## Pontos Identificados

### Ponto Identificado 01

#### Título

Imagem vertical de notícia ou mensagem pode cortar o rosto ao abrir o conteúdo

#### Ambiente

- Aplicativo > Notícias
- Aplicativo > Mensagens

#### Descrição

Ao abrir uma notícia ou mensagem, a imagem muda de formato em relação à visualização anterior. Quando a imagem vertical não está bem enquadrada na parte superior, especialmente quando o rosto da pessoa está mais ao centro, o rosto pode ser cortado ao entrar no conteúdo.

Foi observado que a imagem muda do formato apresentado na tela normal do celular para um enquadramento mais horizontal/paisagem dentro da notícia ou mensagem, causando corte em algumas imagens.

#### Resultado obtido

Imagens verticais podem ficar cortadas ao abrir notícias ou mensagens, principalmente quando o conteúdo importante da foto está no centro.

#### Resultado esperado

A imagem deve manter um enquadramento adequado ao abrir o conteúdo, preservando o rosto ou o elemento principal da foto.

#### Impacto

Prejudica a apresentação visual de notícias e mensagens.

#### Status

Problema persistente.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 02

#### Título

Compartilhamento não envia link clicável do conteúdo

#### Ambiente

- Aplicativo > Notícias
- Aplicativo > Mensagens
- Aplicativo > Vídeos
- Compartilhamento de conteúdo

#### Descrição

Ao compartilhar uma notícia, mensagem ou vídeo, o app envia apenas o título da mensagem/conteúdo e o texto "leia mais no app Verbo da Vida". O compartilhamento não envia um link clicável para que a pessoa acesse diretamente o conteúdo.

Nesta build, os links de YouTube em notícias, mensagens e vídeos foram removidos. Permanece apenas a opção de compartilhar o conteúdo.

#### Resultado obtido

O compartilhamento envia apenas texto, sem link clicável.

#### Resultado esperado

Precisa ser validado com o time. Caso a regra esperada seja permitir acesso direto ao conteúdo compartilhado, o compartilhamento deve incluir um link clicável. Caso a regra seja apenas compartilhar texto informativo, o comportamento atual pode ser considerado esperado.

#### Impacto

Se o link for esperado, o destinatário não consegue acessar diretamente a notícia, mensagem ou vídeo compartilhado.

#### Status

Ponto a validar com o time.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 03

#### Título

Picture in Picture apresenta comportamento incorreto

#### Ambiente

- Aplicativo > Conteúdos em vídeo > Picture in Picture

#### Descrição

O Picture in Picture continua apresentando o mesmo problema. Ao ativar a funcionalidade, a imagem do vídeo permanece rodando no local original e também aparece no Picture in Picture. Além disso, permanece um ícone/placeholder travado, como ocorria nas versões anteriores.

#### Resultado obtido

O vídeo fica rodando simultaneamente no local original e na janela de Picture in Picture, com ícone/placeholder ainda travado.

#### Resultado esperado

Ao ativar o Picture in Picture, o vídeo deve ser exibido de forma consistente, sem duplicação visual e sem placeholder indevido.

#### Impacto

Gera comportamento visual confuso no player de vídeo e prejudica a experiência de uso do Picture in Picture.

#### Status

Problema persistente.

#### Evidências

Prints ou gravações:

- Adicionar evidência, se houver.

### Ponto Identificado 04

#### Título

Verbo FM continua tocando junto com vídeos

#### Ambiente

- Aplicativo > Verbo FM
- Aplicativo > Conteúdos em vídeo

#### Descrição

Ao iniciar a Verbo FM e depois abrir um vídeo, a rádio continua tocando junto com o vídeo. O problema permanece igual ao observado anteriormente.

#### Resultado obtido

A Verbo FM e o áudio do vídeo tocam ao mesmo tempo.

#### Resultado esperado

Ao iniciar um vídeo, a rádio deve pausar automaticamente ou o aplicativo deve impedir a sobreposição de áudio.

#### Impacto

Prejudica a experiência de consumo de áudio e vídeo, causando sobreposição sonora.

#### Status

Problema persistente.

#### Evidências

Gravações:

- Adicionar evidência, se houver.

## Pontos Corrigidos ou Revalidados Nesta Rodada

### Endereço em francês

O campo de endereço foi corrigido. No idioma francês, agora aparece como "Département".

### Calendário

O comportamento corrigido do calendário continua funcionando.

### Alteração de senha

A alteração de senha foi testada e funcionou corretamente.

### Contador do vídeo fora da tela cheia

O contador do vídeo foi corrigido e não quebra mais linha.

### Ofertas

A tela de ofertas está funcionando corretamente.

### Código postal internacional

O código postal internacional está funcionando.

### Fonte grande no iPhone

Com fonte grande no iPhone, o app funciona corretamente.

### Orientação da tela

O app permanece travado em modo retrato e não troca a orientação.

### Link do YouTube em Contatos

O link do YouTube na seção Contatos está funcionando corretamente.

### Links do YouTube em notícias, mensagens e vídeos

Os links do YouTube foram removidos desses conteúdos. Permanece apenas a opção de compartilhamento.

### Validação de e-mail em novo cadastro

A validação de e-mail em novo cadastro foi testada novamente. O e-mail de validação foi recebido e o fluxo funcionou normalmente nas condições de teste.

## Pontos Reclassificados Como Comportamento Esperado

### Troca de igreja com usuário logado

Não será tratado como erro neste momento. O comportamento atual deve funcionar dessa forma.

### Menu contextual de texto em inglês

Continua igual e será mantido por enquanto, conforme decisão anterior do time.

### Demais comportamentos já definidos como não bug

Permanecem como comportamento esperado nesta rodada:

- Lista de igrejas mantendo Campina Grande.
- Alteração de idioma disponível apenas após login.
- Discipulado indisponível no momento.
- Bíblia inicialmente apenas em português.

## Observações Gerais

- A rodada confirma que algumas correções importantes da build 23 estão funcionando.
- Os principais problemas persistentes continuam concentrados em vídeo, áudio e imagens de notícias/mensagens.
- O compartilhamento sem link clicável precisa de decisão do time para definir se será tratado como bug ou regra atual do produto.

## Conclusão

A build 23 apresenta avanço em relação às rodadas anteriores, principalmente na correção do campo de endereço em francês, alteração de senha, contador do vídeo, ofertas, código postal, fonte grande e estabilidade da orientação em modo retrato.

Ainda é necessário acompanhar os problemas persistentes de Picture in Picture, sobreposição de áudio entre Verbo FM e vídeos e enquadramento de imagens verticais. O compartilhamento de conteúdos deve ser validado com o time para confirmar se a ausência de link clicável é comportamento esperado ou ponto a corrigir.
