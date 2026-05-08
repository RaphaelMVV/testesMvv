# Relatório de Testes - App Igreja

## Informações Gerais

| Campo | Informação |
| --- | --- |
| Sistema testado | App Igreja / Church App |
| Data do teste | 2026-04-27 |
| Versão testada | 1.0.2 |
| Compilação / build | 21 |
| Branch testada | validation |
| Plataforma | iOS |
| Sistema operacional | iOS 26.4.2 |
| Dispositivo | iPhone 15 Pro Max |
| Responsável pelo teste | Raphael |

## Resumo Executivo

Durante esta rodada, foi testada a build 21 do App Igreja, com foco na revalidação dos problemas identificados na build 19 e na observação de possíveis regressões.

A build apresentou melhorias importantes em calendário, ofertas, link do YouTube em Contatos, alteração de senha, código postal internacional, fonte grande e comportamento de orientação da tela. Também foi corrigido o comportamento da notícia em destaque que antes abria sem conteúdo, que agora direciona para o site do Portal Verbo da Vida.

Ainda persistem problemas relevantes relacionados à sobreposição de áudio entre Verbo FM e vídeos, Picture in Picture, compartilhamento sem link do conteúdo, menu contextual em inglês, troca de idioma sem login, Bíblia em português após alteração de idioma e tradução do campo de endereço em francês. Também foram observados novos pontos relacionados à troca de igreja quando o usuário está logado, corte de imagem vertical em notícias/mensagens e quebra de linha no contador do vídeo.

Total de pontos identificados nesta rodada: 10

## Pontos Identificados

### Ponto Identificado 01

#### Título

Verbo FM continua tocando junto com vídeos

#### Ambiente

- Aplicativo > Verbo FM
- Aplicativo > Conteúdos em vídeo

#### Descrição

Ao iniciar a reprodução da Verbo FM e, em seguida, abrir um vídeo para assistir, os dois áudios continuam tocando ao mesmo tempo. O áudio da rádio fica sobreposto ao áudio do vídeo.

#### Passos para reproduzir

1. Abrir o aplicativo.
2. Iniciar a reprodução da Verbo FM.
3. Abrir um conteúdo em vídeo.
4. Iniciar a reprodução do vídeo.
5. Observar se os dois áudios continuam tocando simultaneamente.

#### Resultado obtido

A Verbo FM continua tocando junto com o vídeo, causando sobreposição de áudio.

#### Resultado esperado

Ao iniciar um vídeo, a Verbo FM deve pausar automaticamente ou o aplicativo deve impedir a reprodução simultânea dos dois áudios.

#### Impacto

Prejudica a experiência de consumo de áudio e vídeo, pois o usuário escuta dois conteúdos ao mesmo tempo.

#### Evidências

Prints ou gravações:

- Adicionar evidência, se houver.

### Ponto Identificado 02

#### Título

Picture in Picture apresenta comportamento incorreto

#### Ambiente

- Aplicativo > Conteúdos em vídeo > Picture in Picture

#### Descrição

O vídeo continua apresentando comportamento incorreto ao ativar o Picture in Picture. A imagem original ou ícone permanece na parte superior da tela, enquanto o Picture in Picture aparece abaixo, gerando duplicação visual.

#### Passos para reproduzir

1. Abrir um conteúdo em vídeo.
2. Iniciar a reprodução.
3. Ativar o modo Picture in Picture.
4. Observar o comportamento visual do player.

#### Resultado obtido

O vídeo fica com a imagem original/ícone na parte superior e o Picture in Picture embaixo.

#### Resultado esperado

Ao ativar o Picture in Picture, o vídeo deve ficar apenas na janela flutuante ou seguir um comportamento visual consistente, sem duplicação e sem placeholder indevido.

#### Impacto

Gera inconsistência visual e prejudica o uso do player em Picture in Picture.

#### Evidências

Prints ou gravações:

- Adicionar evidência, se houver.

### Ponto Identificado 03

#### Título

Compartilhamento não envia link do conteúdo

#### Ambiente

- Aplicativo > Notícias
- Aplicativo > Mensagens
- Aplicativo > Vídeos
- Compartilhamento de conteúdo

#### Descrição

Na build 21, o fluxo de compartilhamento foi alterado. As opções anteriores foram removidas e agora o app mantém apenas a ação de compartilhar o conteúdo diretamente pelo aplicativo selecionado.

Apesar da mudança, o compartilhamento ainda não envia o link clicável do conteúdo. A mensagem compartilhada envia apenas o título e o texto "leia mais", mas não inclui um link para a pessoa acessar a notícia, mensagem ou vídeo.

#### Passos para reproduzir

1. Abrir uma notícia, mensagem ou vídeo.
2. Acionar a opção de compartilhamento.
3. Escolher um aplicativo de destino.
4. Verificar o conteúdo da mensagem compartilhada.

#### Resultado obtido

A mensagem compartilhada contém o título e "leia mais", mas não contém o link clicável do conteúdo.

#### Resultado esperado

O compartilhamento deve incluir o link do conteúdo para permitir que o destinatário acesse diretamente a notícia, mensagem ou vídeo.

#### Impacto

O compartilhamento perde utilidade, pois o destinatário não consegue acessar diretamente o conteúdo compartilhado.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 04

#### Título

Menu de edição de texto aparece em inglês

#### Ambiente

- Aplicativo > Campos de texto

#### Descrição

Ao tocar em um campo de texto, as opções do menu contextual, como copiar e colar, continuam aparecendo em inglês.

#### Passos para reproduzir

1. Abrir uma tela com campo de texto.
2. Tocar ou pressionar dentro do campo.
3. Observar o idioma das opções do menu contextual.

#### Resultado obtido

As opções do menu contextual aparecem em inglês.

#### Resultado esperado

As opções devem seguir o idioma configurado no aparelho ou no aplicativo.

#### Impacto

Gera inconsistência de idioma na experiência do usuário.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 05

#### Título

Opção de mudar idioma não aparece quando o usuário não está logado

#### Ambiente

- Aplicativo > Acesso sem login
- Aplicativo > Idioma

#### Descrição

Não é possível trocar o idioma do aplicativo quando o usuário não está logado.

#### Passos para reproduzir

1. Abrir o aplicativo sem estar logado.
2. Procurar a opção de troca de idioma.
3. Verificar se a opção está disponível antes do login.

#### Resultado obtido

A opção de troca de idioma não aparece para o usuário deslogado.

#### Resultado esperado

O usuário deve conseguir alterar o idioma antes de realizar login.

#### Impacto

Dificulta o acesso de usuários que precisam usar o aplicativo em outro idioma antes de entrar na conta.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 06

#### Título

Bíblia permanece em português após mudança de idioma

#### Ambiente

- Aplicativo > Bíblia
- Aplicativo > Idioma

#### Descrição

A Bíblia continua sendo exibida em português mesmo após a alteração do idioma do aplicativo.

#### Passos para reproduzir

1. Alterar o idioma do aplicativo.
2. Acessar a seção Bíblia.
3. Verificar o idioma exibido no conteúdo bíblico.

#### Resultado obtido

A Bíblia permanece em português.

#### Resultado esperado

A seção Bíblia deve acompanhar o idioma selecionado no app ou informar claramente que apenas a versão em português está disponível.

#### Impacto

Gera inconsistência de idioma e limita o uso da seção Bíblia para usuários de outros idiomas.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 07

#### Título

Tradução do campo Estado em francês permanece inadequada

#### Ambiente

- Aplicativo > Dados cadastrais / Endereço
- Idioma francês

#### Descrição

No endereço em francês, o campo que deveria ser ajustado para o contexto de "Département" continua aparecendo como "État".

#### Passos para reproduzir

1. Alterar o aplicativo para o idioma francês.
2. Acessar cadastro, perfil ou edição de endereço.
3. Verificar o rótulo do campo equivalente a "Estado".

#### Resultado obtido

O campo permanece com nomenclatura inadequada para o contexto em francês.

#### Resultado esperado

O campo deve usar uma nomenclatura adequada ao contexto de endereço em francês.

#### Impacto

Pode causar ruído de localização e confusão para usuários em francês.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 08

#### Título

Ícone da Home não direciona para troca de igreja quando o usuário está logado

#### Ambiente

- Aplicativo > Home
- Aplicativo > Troca de igreja
- Usuário logado

#### Descrição

Na Home, ao tocar no ícone do Verbo da Vida, na área onde aparece "Bem-vindo" e o nome da igreja, anteriormente o app direcionava para a seleção de igreja. Na build 21, quando o usuário está logado, esse toque não direciona mais para a seleção de igreja.

Foi observado que, quando o usuário não está logado, tocar no ícone do aplicativo ainda direciona para a seleção de igreja. O problema ocorre apenas com usuário logado.

#### Passos para reproduzir

1. Entrar no aplicativo com usuário logado.
2. Acessar a Home.
3. Tocar no ícone do Verbo da Vida na área onde aparece "Bem-vindo" e o nome da igreja.
4. Observar se o app direciona para a seleção de igreja.
5. Repetir o teste sem estar logado.

#### Resultado obtido

Com usuário logado, o toque no ícone não direciona para a seleção de igreja. Sem login, o direcionamento funciona.

#### Resultado esperado

O usuário logado também deve conseguir acessar a troca de igreja por esse caminho, se essa for a regra esperada do app.

#### Impacto

Impede ou dificulta a troca de igreja para usuários logados.

#### Evidências

Prints ou gravações:

- Adicionar evidência, se houver.

### Ponto Identificado 09

#### Título

Imagem vertical de notícia ou mensagem pode cortar o rosto ao abrir o conteúdo

#### Ambiente

- Aplicativo > Notícias
- Aplicativo > Mensagens

#### Descrição

As imagens horizontais ficam adequadas ao abrir uma notícia ou mensagem. Porém, quando a imagem está em formato vertical e a pessoa da foto está mais ao centro, e não na parte superior, o rosto pode ficar cortado.

#### Passos para reproduzir

1. Abrir uma notícia ou mensagem com imagem vertical.
2. Observar o enquadramento da imagem ao abrir o conteúdo.
3. Comparar com uma notícia ou mensagem que utilize imagem horizontal.

#### Resultado obtido

Em imagens verticais, o enquadramento pode cortar o rosto da pessoa quando ela está mais ao centro da foto.

#### Resultado esperado

A imagem deve ser enquadrada de forma a preservar o conteúdo principal, evitando corte excessivo do rosto ou de elementos importantes.

#### Impacto

Prejudica a apresentação visual de notícias e mensagens.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 10

#### Título

Contador do vídeo quebra linha quando o vídeo não está em tela cheia

#### Ambiente

- Aplicativo > Vídeos
- Player de vídeo fora da tela cheia

#### Descrição

Ao abrir a página de um vídeo, antes de colocar o vídeo em tela cheia, o contador/tempo do vídeo quebra linha. O texto do contador não fica em uma única linha.

#### Passos para reproduzir

1. Abrir um conteúdo em vídeo.
2. Manter o vídeo na posição inicial, sem tela cheia.
3. Observar o contador/tempo do vídeo.

#### Resultado obtido

O contador do vídeo quebra linha.

#### Resultado esperado

O contador do vídeo deve permanecer em uma única linha e com leitura adequada.

#### Impacto

Gera inconsistência visual no player e prejudica o acabamento da interface.

#### Evidências

Prints:

- Adicionar evidência, se houver.

## Pontos Corrigidos ou Melhorados Nesta Rodada

### Notícia principal que antes abria sem conteúdo

A imagem/notícia principal que antes aparecia sem conteúdo agora direciona para o site do Portal Verbo da Vida. O comportamento anterior foi considerado corrigido.

### APP-006 - Link do YouTube na seção Contatos

Na seção Contatos, o link do YouTube agora direciona corretamente ao ser tocado.

### Calendário - Imagem padrão de evento

O calendário foi corrigido. Em vez de aparecer a imagem azul com ícone de calendário, agora aparece a data e o nome do mês.

### Ofertas - Dados bancários e cópia de agência/conta

A tela de ofertas apresenta mais opções e agora permite copiar agência e conta. A área também não aparece mais cortada na parte superior; há uma limitação visual mais clara para evitar o corte.

### APP-019 - Alteração de senha

A alteração de senha foi testada novamente e funcionou nesta rodada.

### Barra de progresso e seek do vídeo

A barra de progresso e o seek do vídeo foram revalidados e permanecem corrigidos.

### Código postal internacional

O código postal está funcionando corretamente.

### Fonte grande no iPhone

Com a fonte grande no iPhone, o app funcionou normalmente, sem os cortes observados anteriormente.

### Orientação da tela

O app não muda mais para orientação horizontal. Ele permanece no padrão vertical/retrato.

## Pontos com Comportamento a Validar

### APP-020 - Discipulado

Na área de Discipulado, não aparece nenhuma turma aberta no momento. Em "Minhas inscrições", o app exibe a mensagem "você ainda não tem inscrições".

Não foi confirmado se esse comportamento é esperado para o usuário testado ou se deveriam existir turmas disponíveis para inscrição.

## Observações Gerais

- Os links/opções de YouTube em notícias, mensagens e vídeos foram removidos ou alterados dentro do fluxo atual. Nesta build, o principal ponto observado é que o compartilhamento não inclui link clicável para direcionamento.
- A troca de igreja apresenta comportamento diferente para usuário logado e deslogado: deslogado direciona para seleção de igreja; logado não direciona.
- Os pontos de barra de vídeo, seek, fonte grande, código postal e orientação de tela foram revalidados e não precisam ser tratados como problemas nesta rodada.

## Conclusão

A build 21 apresenta avanços importantes em relação à build 19, especialmente em Contatos, Calendário, Ofertas, alteração de senha, código postal internacional e comportamento visual com fonte grande.
