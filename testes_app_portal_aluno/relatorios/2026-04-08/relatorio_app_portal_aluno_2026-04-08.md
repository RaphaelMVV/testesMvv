APP PORTAL ALUNO
Relatório de Testes Visuais
Erros Encontrados
1. Quebra de layout quando a fonte do smartphone está grande
Evidência:
Como reproduzir: aumentar o tamanho da fonte nas configurações do
smartphone e navegar pelo app.
Resultado atual: alguns elementos quebram, sobrepõem ou deixam de caber
corretamente.
APP  POR T AL  ALUNO
1

Resultado esperado: o layout deve se adaptar ao tamanho da fonte sem
cortes, sobreposição ou perda de usabilidade.
2. Gesto de voltar leva para a tela de login
Evidência:
Como reproduzir: em uma tela interna, fazer o gesto de arrastar da esquerda
para a direita para voltar.
Resultado atual: o app retorna para a tela de login.
Resultado esperado: o app deve voltar apenas para a tela anterior do fluxo.
3. Card “Pagamentos” direciona para a aba errada
Evidência:
APP  POR T AL  ALUNO
2

Como reproduzir: na Home, tocar no card “Pagamentos”.
Resultado atual: o usuário é levado para “Meu Histórico / Acadêmico”.
Resultado esperado: o usuário deve ser levado para “Meu Histórico /
Financeiro”.
4. Busca em “Meu Histórico / Acadêmico” fica presa ao voltar
Evidência:
APP  POR T AL  ALUNO
3

Como reproduzir: pesquisar uma matéria específica, sair da página e depois
voltar.
Resultado atual: continua aparecendo só a matéria filtrada, mas a barra de
pesquisa fica vazia. A lista só volta ao normal se for feita uma nova pesquisa e
depois apagada.
Resultado esperado: o filtro deve ser limpo ao voltar para a página, ou o texto
pesquisado deve continuar visível na barra.
5. Busca em “Matérias Disponíveis” fica presa ao voltar
Evidência:
APP  POR T AL  ALUNO
4

Como reproduzir: pesquisar uma matéria específica, sair da página e depois
voltar.
Resultado atual: continua aparecendo só a matéria filtrada, mas a barra de
pesquisa fica vazia. A lista só volta ao normal se for feita uma nova pesquisa e
depois apagada.
Resultado esperado: o filtro deve ser limpo ao voltar para a página, ou o texto
pesquisado deve continuar visível na barra.
6. Bug no player de áudio ao arrastar a barra de progresso
Evidência: Não foi possível registrar em uma imagem.
Como reproduzir: abrir o áudio de uma matéria, arrastar a bolinha do player
para outro ponto e soltar.
Resultado atual: a bolinha oscila entre a posição inicial e a posição arrastada.
Em alguns casos, o tempo continua correndo, mas o áudio fica mudo por cerca
de 10 a 20 segundos antes de voltar.
APP  POR T AL  ALUNO
5

Resultado esperado: a barra deve acompanhar o arrasto de forma estável e o
áudio deve continuar imediatamente a partir do ponto em que foi solto.
7. Botão de salvar no perfil cobre os campos
Evidência:
Como reproduzir: entrar na edição do perfil e rolar a tela até os campos
inferiores.
Resultado atual: o botão de salvar fica em cima dos campos e atrapalha o
preenchimento.
Resultado esperado: o botão deve ficar fixo em uma área segura no rodapé,
sem cobrir conteúdo.
8. Campo “Estado” não atende perfis internacionais na edição
de perfil
Evidência:
APP  POR T AL  ALUNO
6

Como reproduzir: acessar a edição de perfil com um usuário internacional, por
exemplo da França, e ir até a parte de endereço/perfil.
Resultado atual: o campo “Estado” aparenta considerar apenas estados do
Brasil, sem opção adequada para usuários de outros países.
Resultado esperado: para perfis internacionais, o campo deveria se adaptar ao
país informado, permitir um valor genérico compatível ou não exigir estados
brasileiros.
Pontos para Validação, Não Sei Se São Erros ou se
Deveriam Funcionar Assim Mesmo
1. Ao abrir uma notícia, o usuário consegue navegar no portal
inteiro
Evidência:
APP  POR T AL  ALUNO
7

Como reproduzir: tocar em um card de notícia na Home.
Resultado atual: o app redireciona para o site do portal, mas não deixa o
usuário restrito à notícia aberta; é possível navegar pelo site inteiro.
Ponto a validar: confirmar se a intenção era abrir apenas a notícia específica
ou realmente permitir navegação completa no portal.
2. Em “Meu Histórico / Financeiro”, tocar em um pagamento
não mostra comprovante
Evidência:
APP  POR T AL  ALUNO
8

Como reproduzir: acessar “Meu Histórico / Financeiro” e tocar em um item de
pagamento efetuado.
Resultado atual: não fica disponível nenhum documento ou comprovante
visível para abertura.
Ponto a validar: confirmar se esses itens deveriam ter comprovante/anexo ou
se são apenas registros informativos.
3. Em “Matérias Disponíveis”, apenas “Aliança de Sangue”
possui áudio
Evidência:
APP  POR T AL  ALUNO
9

Como reproduzir: acessar “Matérias Disponíveis” e abrir as matérias
disponíveis.
Resultado atual: apenas a matéria “Aliança de Sangue” apresenta áudio
disponível.
Ponto a validar: confirmar se isso é limitação de conteúdo cadastrado no
sistema ou se outras matérias também deveriam ter áudio.
4. Notícias não mudam de idioma junto com o app
Evidência:
APP  POR T AL  ALUNO
10

Como reproduzir: alterar o idioma do app e verificar novamente os cards de
notícias.
Resultado atual: os cards continuam em português mesmo após a troca de
idioma.
Ponto a validar: confirmar se as notícias deveriam acompanhar o idioma
selecionado no app ou se o conteúdo é fixo em português.
APP  POR T AL  ALUNO
11
