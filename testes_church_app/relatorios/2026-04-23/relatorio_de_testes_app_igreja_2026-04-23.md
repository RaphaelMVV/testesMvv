# Relatório de Testes - App Igreja

## Informações Gerais

| Campo | Informação |
| --- | --- |
| Sistema testado | App Igreja / Church App |
| Data de início | 2026-04-15 |
| Data final / entrega | 2026-04-23 |
| Versão testada | 1.0.2 |
| Compilação / build | 19 |
| Plataforma | iOS |
| Sistema operacional | iOS 26.4.1 |
| Dispositivo | iPhone 15 Pro Max |
| Responsável pelo teste | Raphael |

## Resumo Executivo

Durante esta rodada, foram revalidados problemas reportados anteriormente no App Igreja, com foco em vídeo, Picture in Picture, Verbo FM, notícias, compartilhamento, contatos, ofertas, acessibilidade, idioma e campos de cadastro internacional.

Parte dos problemas anteriores foi corrigida, incluindo a barra de progresso do vídeo, o seek rápido, o compartilhamento de notícias, a tela de ofertas, o corte de textos com fonte grande e o problema de imagem no modo paisagem, já que o aplicativo passou a permanecer apenas em modo retrato.

Ainda foram identificados problemas relacionados ao Picture in Picture, sobreposição de áudio entre Verbo FM e vídeos, links do YouTube, menu contextual em inglês, alteração de senha, troca de idioma, Bíblia em português após mudança de idioma e tradução do campo de endereço em francês.

Total de pontos identificados nesta rodada: 12

## Pontos Identificados

### Ponto Identificado 01

#### Título

Picture in Picture apresenta comportamento incorreto

#### Ambiente

- Aplicativo > Conteúdos em vídeo > Picture in Picture

#### Descrição

Ao ativar o Picture in Picture, o vídeo fica aparecendo em duas telas e também permanece um ícone/placeholder fixo na parte superior da tela.

Ao sair da página do vídeo dentro do app, o vídeo para de rodar. Porém, quando o celular é bloqueado, o vídeo continua tocando com a tela bloqueada.

Na tela bloqueada, os controles disponíveis parecem limitados: aparecem as opções de pausar e dar play, mas não aparecem controles para avançar 10 segundos nem a barra/bolinha de progresso.

#### Passos para reproduzir

1. Abrir um conteúdo em vídeo no aplicativo.
2. Iniciar a reprodução.
3. Ativar o modo Picture in Picture.
4. Observar se o vídeo aparece duplicado.
5. Sair da página do vídeo.
6. Bloquear o celular com o vídeo em reprodução.
7. Observar os controles disponíveis na tela bloqueada.

#### Resultado obtido

O vídeo aparece em duas telas no Picture in Picture e permanece um ícone/placeholder fixo na parte superior. Ao sair da página do vídeo, a reprodução para dentro do app, mas ao bloquear o celular o vídeo continua tocando. Na tela bloqueada, aparecem apenas controles básicos de play/pausa.

#### Impacto

Gera inconsistência visual e comportamento confuso no uso do player de vídeo, especialmente ao alternar entre tela do app, segundo plano, Picture in Picture e tela bloqueada.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 02

#### Título

Verbo FM continua tocando junto com vídeos

#### Ambiente

- Aplicativo > Verbo FM
- Aplicativo > Conteúdos em vídeo

#### Descrição

Quando a Verbo FM está em reprodução e o usuário inicia um vídeo, os dois áudios continuam tocando ao mesmo tempo. Não é necessário fazer a ação rapidamente; a sobreposição acontece mesmo em uso normal.

Ao sair do vídeo, foi observado que o vídeo para, mas a Verbo FM também para de tocar depois. Ainda assim, durante a reprodução do vídeo, a rádio e o vídeo ficam tocando juntos.

#### Passos para reproduzir

1. Abrir o aplicativo.
2. Iniciar a reprodução da Verbo FM.
3. Abrir um conteúdo em vídeo.
4. Iniciar a reprodução do vídeo.
5. Observar se os dois áudios continuam tocando ao mesmo tempo.
6. Sair da página do vídeo e observar o comportamento da Verbo FM.

#### Resultado obtido

A Verbo FM continua tocando junto com o áudio do vídeo. Ao sair do vídeo, a rádio também para de tocar.

#### Impacto

Prejudica a experiência de consumo de áudio e vídeo, causando sobreposição sonora e comportamento inconsistente entre rádio e player de vídeo.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 03

#### Título

Links do YouTube em notícias não funcionam

#### Ambiente

- Aplicativo > Notícias / conteúdos

#### Descrição

Os links do YouTube não funcionam nas notícias. Ao acionar o link, o aplicativo direciona para uma página que informa que o conteúdo está inacessível.

O problema não está mais restrito ao conteúdo em destaque da Home; foi observado como comportamento nos links de YouTube das notícias.

#### Passos para reproduzir

1. Abrir o aplicativo.
2. Acessar uma notícia/conteúdo que tenha link do YouTube.
3. Tocar no link do YouTube.
4. Observar a página de destino.

#### Resultado obtido

O link direciona para uma página informando que está inacessível.

#### Impacto

Impede o acesso correto aos vídeos ou conteúdos relacionados no YouTube.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 04

#### Título

Link do YouTube na seção Contatos não direciona

#### Ambiente

- Aplicativo > Contatos

#### Descrição

Na seção de Contatos, o link do YouTube ainda não funciona. Ao tocar no link, o aplicativo não direciona para nenhum lugar.

#### Passos para reproduzir

1. Abrir o aplicativo.
2. Acessar a seção Contatos.
3. Tocar no link ou botão do YouTube.
4. Observar se algum destino é aberto.

#### Resultado obtido

Nada acontece ao tocar no link do YouTube.

#### Impacto

Prejudica o acesso aos canais oficiais da igreja a partir da tela de contatos.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 05

#### Título

Menu de edição de texto aparece em inglês

#### Ambiente

- Aplicativo > Campos de texto

#### Descrição

Ao tocar em campos de texto e abrir o menu contextual de edição, as opções de copiar, colar e ações relacionadas aparecem em inglês.

#### Passos para reproduzir

1. Abrir uma tela com campo de texto.
2. Tocar no campo.
3. Acionar o menu contextual de edição.
4. Observar o idioma das opções exibidas.

#### Resultado obtido

As opções do menu contextual aparecem em inglês.

#### Impacto

Gera inconsistência de idioma na experiência do usuário.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 06

#### Título

Tradução do campo Estado em francês não está correta ao contexto

#### Ambiente

- Aplicativo > Dados cadastrais / Endereço
- Idioma francês

#### Descrição

No idioma francês, o campo de endereço "Estado" aparece como "État". Para o contexto de endereço na França, essa tradução não se encaixa bem. O termo esperado seria "Département", conforme observado anteriormente.

#### Passos para reproduzir

1. Alterar o aplicativo para o idioma francês.
2. Acessar a área de dados cadastrais.
3. Ir até a parte de endereço.
4. Verificar o nome exibido no campo "Estado".

#### Resultado obtido

O campo aparece como "État".

#### Impacto

Pode causar confusão para usuários em francês, pois o termo não corresponde bem ao contexto de endereço esperado.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 07

#### Título

Imagem padrão do evento no calendário deve ser validada

#### Ambiente

- Aplicativo > Calendário > Eventos

#### Descrição

Na parte de calendário, ao abrir um evento do dia, a imagem exibida é um ícone de calendário com fundo azul. Não foi confirmado se esse comportamento está incorreto, mas o ponto deve ser observado e validado com o time responsável.

#### Passos para reproduzir

1. Abrir o aplicativo.
2. Acessar a seção Calendário.
3. Abrir um evento do dia.
4. Observar a imagem exibida no evento.

#### Resultado obtido

É exibida uma imagem padrão com ícone de calendário e fundo azul.

#### Impacto

Não foi classificado como erro nesta rodada. Pode ser comportamento esperado quando o evento não possui imagem própria cadastrada.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 08

#### Título

Lista de igrejas apresenta apenas Campina Grande

#### Ambiente

- Aplicativo > Selecionar igreja / Buscar igreja

#### Descrição

Na tela de seleção de igreja, aparece apenas a igreja de Campina Grande. Ao buscar por qualquer outra igreja, nenhum outro resultado é exibido.

Não foi confirmado se esse comportamento é proposital ou se existe uma limitação de cadastro/disponibilidade, mas o ponto deve ser validado com o time responsável.

#### Passos para reproduzir

1. Abrir o aplicativo.
2. Acessar a tela de selecionar igreja.
3. Observar a lista inicial de igrejas.
4. Buscar por outras igrejas.
5. Verificar os resultados exibidos.

#### Resultado obtido

Apenas a igreja de Campina Grande aparece na seleção. Ao buscar por outras igrejas, não são exibidos resultados.

#### Impacto

Pode impedir que usuários de outras igrejas selecionem corretamente sua unidade, caso a lista deva apresentar mais opções.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 09

#### Título

Opção de mudar idioma não aparece quando o usuário não está logado

#### Ambiente

- Aplicativo > Acesso sem login
- Aplicativo > Configurações / idioma

#### Descrição

Quando o usuário não está logado, a opção para mudar o idioma do aplicativo não aparece. Com isso, não é possível alterar o idioma antes de entrar em uma conta.

#### Passos para reproduzir

1. Abrir o aplicativo sem estar logado.
2. Procurar a opção de alterar idioma.
3. Verificar se a opção está disponível.

#### Resultado obtido

A opção de troca de idioma não aparece para o usuário deslogado.

#### Impacto

Pode dificultar o acesso de usuários que precisam usar o aplicativo em outro idioma antes de realizar login.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 10

#### Título

Alteração de senha retorna erro mesmo com dados corretos

#### Ambiente

- Aplicativo > Perfil / Alterar senha

#### Descrição

Na tela de alteração de senha, ao informar a senha atual correta, preencher a nova senha e repetir a nova senha corretamente, o aplicativo exibe erro de dados de entrada inválido ao tentar salvar.

#### Passos para reproduzir

1. Acessar o aplicativo com usuário logado.
2. Abrir a área de alteração de senha.
3. Informar a senha atual correta.
4. Informar a nova senha.
5. Repetir a nova senha corretamente.
6. Tocar em salvar.

#### Resultado obtido

O aplicativo exibe a mensagem de erro "dados de entrada inválido".

#### Impacto

Impede ou dificulta a alteração de senha pelo usuário.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 11

#### Título

Discipulado não exibe matérias disponíveis para inscrição

#### Ambiente

- Aplicativo > Discipulado > Minhas inscrições / matérias

#### Descrição

Na área de Discipulado, não aparecem matérias em "Minhas inscrições" nem matérias disponíveis para inscrição.

Não foi confirmado se isso é erro ou se depende de cadastro/liberação de conteúdo para o usuário, mas o comportamento deve ser validado.

#### Passos para reproduzir

1. Acessar o aplicativo com usuário logado.
2. Abrir a área de Discipulado.
3. Acessar "Minhas inscrições".
4. Verificar se aparecem matérias ou opções de inscrição.

#### Resultado obtido

Não aparecem matérias nem opções de inscrição.

#### Impacto

Pode impedir o usuário de visualizar ou realizar inscrições em matérias, caso existam conteúdos disponíveis.

#### Evidências

Prints:

- Adicionar evidência, se houver.

### Ponto Identificado 12

#### Título

Bíblia permanece em português após mudança de idioma

#### Ambiente

- Aplicativo > Bíblia
- Aplicativo com idioma alterado

#### Descrição

Ao mudar o idioma do aplicativo, a Bíblia continua sendo exibida em português. O conteúdo não acompanha o idioma selecionado no aplicativo.

#### Passos para reproduzir

1. Alterar o idioma do aplicativo.
2. Acessar a seção Bíblia.
3. Verificar o idioma exibido no conteúdo da Bíblia.

#### Resultado obtido

A Bíblia continua em português mesmo após a mudança de idioma do aplicativo.

#### Impacto

Gera inconsistência de idioma e limita o uso da seção Bíblia por usuários que utilizam o aplicativo em outros idiomas.

#### Evidências

Prints:

- Adicionar evidência, se houver.

## Pontos Corrigidos Nesta Rodada

### APP-004 - Notícia em destaque sobre o ecossistema digital do MVV

O comportamento anterior foi alterado. Os destaques agora aparecem como banners em tamanho adequado para visualização e não são mais clicáveis como antes. Foi observado, por exemplo, um banner do calendário MVV. Com isso, o problema anterior de abrir a notícia em destaque sem conteúdo foi considerado resolvido.

### APP-007 - Compartilhamento não enviava o link do conteúdo

O compartilhamento agora está funcionando. Ao compartilhar uma notícia, o app envia o link e um resumo do conteúdo.

### APP-008 - Imagem da notícia ficava cortada no modo paisagem

O aplicativo não muda mais para o modo paisagem e permanece apenas em modo retrato. Por isso, o problema anterior da imagem cortada no modo paisagem foi considerado resolvido.

### APP-009 - Barra de progresso do vídeo mudava de tamanho durante o uso

A barra de progresso do vídeo não muda mais de tamanho ao arrastar a bolinha. O comportamento está estável.

### APP-010 - Seek rápido pausava o vídeo

Ao arrastar a bolinha do vídeo, o vídeo vai para o tempo selecionado e continua rodando sem pausar. O problema foi considerado resolvido.

### APP-011 - Tela de ofertas não apresentava dados bancários

A tela de ofertas agora apresenta os dados bancários. O problema foi considerado resolvido.

### APP-012 - Texto ficava cortado com fonte grande no iPhone

Com a fonte grande no iPhone, o corte de texto observado anteriormente não ocorreu nesta rodada. O comportamento foi considerado resolvido.

### APP-014 - Cadastro internacional não aceitava código postal no formato do país

O código postal internacional foi revalidado e está funcionando. O problema anterior foi considerado resolvido nesta rodada.

## Pontos Removidos da Lista de Erros

### APP-016 - Campo Bairro obrigatório em francês

O campo "Bairro" obrigatório em francês foi reavaliado e não será mais tratado como erro neste momento. Foi considerado aceitável que o usuário preencha o campo com uma informação alternativa quando necessário.

## Observações Gerais

- O aplicativo não muda mais para orientação horizontal. Ele permanece em modo retrato. Isso foi tratado como observação e também resolve o problema anterior relacionado à imagem da notícia no modo paisagem.
- O comportamento do Picture in Picture precisa ser validado com o time responsável, especialmente em relação ao que deve acontecer ao sair da página do vídeo, deixar o app em segundo plano e bloquear o celular.
- A imagem padrão dos eventos no calendário deve ser validada para confirmar se é comportamento esperado quando o evento não possui imagem cadastrada.
- A listagem de igrejas deve ser validada para confirmar se apenas Campina Grande deve aparecer nesta versão.
- A ausência de matérias no Discipulado deve ser validada para confirmar se depende de cadastro/liberação de conteúdo para o usuário.

## Conclusão

O aplicativo apresentou avanços importantes em relação aos problemas anteriores, especialmente em compartilhamento, ofertas, barra de progresso de vídeo, seek do vídeo, fonte grande e comportamento em modo paisagem.

Ainda existem pontos relevantes a corrigir, principalmente no Picture in Picture, na sobreposição de áudio entre Verbo FM e vídeos, nos links do YouTube, no menu contextual em inglês, na alteração de senha, na Bíblia após mudança de idioma e na tradução do campo de endereço em francês.
