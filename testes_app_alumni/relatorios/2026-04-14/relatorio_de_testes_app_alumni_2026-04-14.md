Relatório de Testes - App
Alumni - 14/04/2026
Informações Gerais
Data
14 de abril de 2026
Versão testada
1.0.39
Compilação
108
Plataforma
iPhone 15 Pro Max
Resumo Executivo
Durante os testes, foram identificadas falhas relevantes no player de vídeo, no
Picture-in-Picture, na reprodução em segundo plano, na usabilidade em iPhone
e na adaptação de interface para fonte ampliada.
Total de falhas identificadas: 10
Ponto Identificado 01
Título
Encerramento inesperado ao trocar vídeos repetidamente
Ambiente
Aplicativo > Vídeos > Player
Descrição
Ao alternar entre vídeos de forma rápida e repetida, o aplicativo fecha sozinho.
O comportamento foi reproduzido várias vezes. Em alguns testes o
Relatório de T estes - App Alumni - 14/04/2026
1

encerramento ocorreu mais rapidamente, e em outros demorou um pouco
mais, mas foi sempre possível reproduzir.
Passos para reproduzir
- Abrir um vídeo.
- Avançar ou interagir rapidamente.
- Abrir outro vídeo.
- Repetir essa troca várias vezes.
Resultado esperado
O aplicativo deve permanecer estável, mesmo com trocas rápidas entre vídeos.
Resultado obtido
O aplicativo encerra inesperadamente.
Evidências
Prints
Relatório de T estes - App Alumni - 14/04/2026
2

Ponto Identificado 02
Título
Ativação do Picture-in-Picture antes do carregamento trava a interface com
sobreposição duplicada
Ambiente
Aplicativo > Vídeos > Player
Descrição
Quando o vídeo ainda está carregando e o usuário ativa o Picture-in-Picture
antes da conclusão do carregamento, a imagem fica travada no centro da tela,
duplicando a exibição do player e sobrepondo outros elementos da interface.
Relatório de T estes - App Alumni - 14/04/2026
3

Os controles do vídeo deixam de aparecer e a única saída encontrada foi voltar
para a tela anterior.
Passos para reproduzir
- Abrir um vídeo.
- Antes do carregamento terminar, ativar o Picture-in-Picture.
Resultado esperado
O Picture-in-Picture deve iniciar corretamente ou ficar indisponível até o vídeo
estar pronto.
Resultado obtido
A interface fica travada com imagem duplicada e sem controles visíveis.
Evidências
Prints
Relatório de T estes - App Alumni - 14/04/2026
4

Ponto Identificado 03
Título
Picture-in-Picture funciona ao mesmo tempo que a tela original do vídeo
Ambiente
Aplicativo > Vídeos > Player
Descrição
Ao ativar o Picture-in-Picture, a janela flutuante passa a funcionar, mas a tela
original do vídeo também continua funcionando ao mesmo tempo. Além disso,
permanece na tela uma imagem fixa na região central inferior, junto com a
mensagem informando que o vídeo está sendo reproduzido no Picture-in-
Picture. Na prática, ficam duas exibições simultâneas e uma imagem fixa sobre
a interface.
Passos para reproduzir
- Iniciar a reprodução de um vídeo.
- Ativar o Picture-in-Picture.
- Observar a tela original do player e a janela flutuante ao mesmo tempo.
Resultado esperado
Ao ativar o Picture-in-Picture, a reprodução deve migrar corretamente para
esse modo, sem manter a tela original ativa de forma simultânea e sem
sobreposições fixas na interface.
Resultado obtido
O Picture-in-Picture funciona, mas a tela original também continua ativa, com
uma imagem fixa sobre a interface.
Evidências
Prints
Relatório de T estes - App Alumni - 14/04/2026
5

Ponto Identificado 04
Título
Falhas na reprodução em segundo plano e com tela bloqueada em velocidades
1.5x e 2x
Ambiente
Aplicativo > Vídeos > Player > Reprodução em segundo plano
Descrição
Tela desbloqueada
O aplicativo em segundo plano funciona normalmente na velocidade 1x.
Relatório de T estes - App Alumni - 14/04/2026
6

Porém, na velocidade 1.5x e 2x, quando o aplicativo vai para segundo plano, o
áudio para por alguns segundos, aproximadamente 3 segundos, e depois volta.
Tela bloqueada
Quando o vídeo está em reprodução e a tela é bloqueada, na velocidade 1x
continua funcionando normalmente.
Na velocidade 1.5x, o áudio para por cerca de 20 a 30 segundos e depois volta.
Na velocidade 2x, o áudio não volta.
Se a tela for acesa sem desbloquear, nesse momento o áudio retorna
momentaneamente, mas para novamente logo em seguida.
Em todos esses casos, o vídeo continua contando o tempo normalmente.
Passos para reproduzir
- Abrir um vídeo.
- Alterar a velocidade para 1.5x ou 2x.
- Colocar o aplicativo em segundo plano com a tela desbloqueada.
- Repetir o teste com a tela bloqueada.
Resultado esperado
O áudio deve continuar funcionando normalmente em segundo plano e com a
tela bloqueada em todas as velocidades suportadas.
Resultado obtido
O tempo do vídeo continua correndo, mas o áudio falha ou desaparece
conforme a velocidade e o estado da tela.
Ponto Identificado 05
Título
Credencial digital corta textos quando o tamanho da fonte está ampliado
Ambiente
Aplicativo > Credencial digital
Descrição
Relatório de T estes - App Alumni - 14/04/2026
7

Com fonte maior no dispositivo, parte dos textos da credencial digital fica
cortada tanto na frente quanto no verso, prejudicando a leitura completa das
informações.
Passos para reproduzir
- Aumentar o tamanho da fonte do sistema.
- Abrir a credencial digital.
Resultado esperado
A credencial deve se adaptar a fontes maiores sem cortar informações
importantes.
Resultado obtido
O texto é cortado e não pode ser lido integralmente.
Evidências
Prints
Relatório de T estes - App Alumni - 14/04/2026
8

Relatório de T estes - App Alumni - 14/04/2026
9

Ponto Identificado 06
Título
Seleção de tipo de documento fica com texto cortado quando a fonte está
ampliada
Ambiente
Aplicativo > Perfil > Dados pessoais > Tipo de documento
Descrição
Na seleção do tipo de documento, as opções ficam cortadas quando a fonte do
dispositivo está grande, o que impede a leitura completa e dificulta a escolha
correta do documento. E corta parte do nÚmero do documento quando a letra
está grande.
Relatório de T estes - App Alumni - 14/04/2026
10

Passos para reproduzir
- Aumentar o tamanho da fonte do sistema.
- Acessar Perfil > Dados pessoais > Tipo de documento.
Resultado esperado
As opções devem permanecer legíveis e totalmente visíveis.
Resultado obtido
Os textos são cortados e a seleção fica comprometida.
Evidências
Prints
Relatório de T estes - App Alumni - 14/04/2026
11

Ponto Identificado 07
Título
Perfil e endereço não atendem corretamente cenários internacionais
Ambiente
Aplicativo > Perfil > Endereço
Descrição
O campo de telefone aceita apenas padrão brasileiro, impedindo o cadastro de
números internacionais. Na etapa de endereço, tentativas de cadastro
internacional não foram aceitas, mas sem indicação clara de qual campo
estava inválido. Isso reduz a usabilidade e dificulta o preenchimento correto
para usuários fora do Brasil.
Passos para reproduzir
- Tentar cadastrar telefone internacional.
- Preencher endereço com dados internacionais.
- Enviar o formulário.
Resultado esperado
O formulário deve aceitar formatos internacionais compatíveis ou informar
claramente as restrições e o campo inválido.
Resultado obtido
O telefone internacional não é aceito e o endereço falha sem feedback claro.
Ponto Identificado 08
Título
Barra de progresso apresenta comportamento inconsistente após arrastar o
controle de tempo
Ambiente
Aplicativo > Vídeos > Player
Relatório de T estes - App Alumni - 14/04/2026
12

Descrição
Ao arrastar a bolinha da barra de progresso para mudar o tempo do vídeo, em
alguns casos a reprodução continua normalmente e em outros o vídeo fica
pausado. O comportamento é inconsistente.
Passos para reproduzir
- Reproduzir um vídeo.
- Arrastar o controle de tempo para outro ponto da mídia.
Resultado esperado
Após o ajuste do tempo, o player deve apresentar comportamento consistente.
Resultado obtido
O vídeo às vezes continua e às vezes permanece pausado.
Evidências
Prints
Relatório de T estes - App Alumni - 14/04/2026
13

Ponto Identificado 09
Título
Barra de progresso em tela horizontal fica muito próxima da área de gesto do
iPhone
Ambiente
Aplicativo > Vídeos > Player em tela horizontal
Descrição
Quando o vídeo está na horizontal, a área central inferior da barra de progresso
fica próxima demais da região usada pelo iPhone para alternar ou minimizar
aplicativos. Isso dificulta ou impede o ajuste do tempo nessa área, porque o
gesto do sistema operacional é acionado no lugar da interação com o player.
Relatório de T estes - App Alumni - 14/04/2026
14

Passos para reproduzir
- Abrir um vídeo em modo horizontal.
- Tentar ajustar o tempo na região central inferior da barra.
Resultado esperado
O usuário deve conseguir arrastar a barra de progresso sem conflito com os
gestos do sistema.
Resultado obtido
O aplicativo é minimizado ou ocorre troca de app em vez de avançar o vídeo.
Evidências
Prints
Ponto Identificado 10
Título
Botão de compartilhar não executa nenhuma ação
Ambiente
Aplicativo > Vídeos > Player
Descrição
Relatório de T estes - App Alumni - 14/04/2026
15

Ao tocar no botão de compartilhar, há retorno visual de toque, mas nenhuma
ação é iniciada. Não abre a tela de compartilhamento nem ocorre qualquer
feedback funcional.
Passos para reproduzir
- Abrir um vídeo.
- Tocar no botão de compartilhar.
Resultado esperado
O sistema deve abrir as opções de compartilhamento do dispositivo ou um
fluxo equivalente.
Resultado obtido
O botão aparenta receber o toque, mas não faz nada.
Evidências
Prints
Relatório de T estes - App Alumni - 14/04/2026
16

Ponto Identificado 11
Título
Áudio do vídeo anterior continua tocando junto com o áudio do novo vídeo
Ambiente
Aplicativo > Vídeos > Player
Descrição
Ao trocar vídeos rapidamente, em um dos testes o áudio do vídeo anterior
continuou sendo reproduzido mesmo após a abertura do novo vídeo. Com isso,
os dois áudios passaram a tocar simultaneamente, embora apenas um vídeo
estivesse visível em reprodução na tela.
Relatório de T estes - App Alumni - 14/04/2026
17

Passos para reproduzir
- Abrir um vídeo.
- Avançar o vídeo para o meio ou para outra parte.
- Trocar rapidamente para outro vídeo.
- Repetir esse processo algumas vezes.
Resultado esperado
Ao trocar de vídeo, o áudio do vídeo anterior deve ser encerrado
imediatamente, mantendo apenas o áudio do vídeo atual.
Resultado obtido
O áudio do vídeo anterior continua tocando junto com o áudio do novo vídeo.
Ponto Identificado 12
Título
Opções de copiar e colar aparecem em inglês nos campos de texto
Ambiente
Aplicativo > Campos de texto
Descrição
Ao tocar em um campo de texto e abrir o menu contextual do sistema, as
opções relacionadas a copiar e colar aparecem em inglês, em vez de seguir o
idioma esperado da aplicação ou do dispositivo.
Passos para reproduzir
- Abrir qualquer tela com campo de texto editável.
- Tocar no campo para abrir o menu contextual.
- Observar as opções exibidas.
Resultado esperado
As opções do menu contextual devem aparecer no idioma esperado para o
usuário.
Relatório de T estes - App Alumni - 14/04/2026
18

Resultado obtido
As opções de copiar e colar aparecem em inglês.
Evidências
Prints
Relatório de T estes - App Alumni - 14/04/2026
19
