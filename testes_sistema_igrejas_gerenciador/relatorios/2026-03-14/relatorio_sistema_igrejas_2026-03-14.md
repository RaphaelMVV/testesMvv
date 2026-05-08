Relatório de Testes - Sistema
Igrejas
Ponto Identificado 01
Título
Falha sistêmica em campos de texto com busca contínua, causando erro
interno do servidor
Severidade
Crítica
Ambiente
Administrativo > Avisos
Administrativo > Calendário
Aplicativo > Dízimos e Ofertas
Departamento Infantil > Check-in/Checkout
Gestão de Pessoas > Famílias
Gestão de Pessoas > Aconselhamento
Gestão de Pessoas > Visitantes
Gestão de Pessoas > Membros
Descrição
Durante os testes, foi identificado que o erro não está necessariamente ligado
à quantidade de caracteres digitados, mas ao tempo em que a página
permanece executando buscas de forma contínua enquanto o usuário digita.
Ao manter a digitação ativa por aproximadamente 10 segundos seguidos, às
vezes um pouco mais, o sistema continua processando consultas em tempo
real até que ocorre erro interno do servidor. Em alguns momentos, os
caracteres deixam de aparecer visualmente no campo, embora a digitação
continue sendo processada, perceptível pelo movimento contínuo do cursor.
Em parte dos testes, após atualizar a página, o usuário é redirecionado para a
tela de login e o acesso pode ficar temporariamente indisponível.
Passos para reproduzir
Relatório de T estes - Sistema Igrejas
1

- Acessar um dos módulos afetados.
- Localizar um campo de texto ou busca.
- Começar a digitar continuamente no campo.
- Manter a digitação por aproximadamente 10 segundos, ou um pouco mais,
sem interromper o processo de busca da página.
- Observar o comportamento da interface e o retorno do sistema.
Resultado obtido
A página permanece executando buscas de forma contínua durante a
digitação.
Após alguns segundos de busca contínua, o sistema apresenta erro interno
do servidor.
Em alguns casos, os caracteres deixam de ser exibidos no campo, embora
a entrada continue sendo processada.
Em alguns casos, após atualizar a página, o usuário é redirecionado para a
tela de login.
O login pode ficar temporariamente indisponível por cerca de 1 minuto.
Impacto
Interrupção de uso em múltiplos módulos do sistema.
Indício de falha sistêmica em campos de texto com busca dinâmica.
Risco de indisponibilidade causado por processamento contínuo de
pesquisa durante a digitação.
Comportamento inconsistente da interface, dificultando a percepção do
que está sendo digitado.
Perda de sessão e indisponibilidade temporária de login.
Alto impacto operacional.
Evidências
Prints:
Relatório de T estes - Sistema Igrejas
2

Relatório de T estes - Sistema Igrejas
3

Ocorrência reproduzida também em Calendário , Dízimos e Ofertas , Check-
in/Checkout , Famílias , Aconselhamento , Visitantes  e Membros
Ponto Identificado 02
Título
Avisos permanecem exibidos de forma persistente no dashboard e no sino de
notificações
Severidade
Média
Ambiente
Administrativo > Avisos
Dashboard
Ícone de notificações
Descrição
Relatório de T estes - Sistema Igrejas
4

Após a criação de um aviso, ele passa a ser exibido no dashboard e também
sinalizado no ícone de notificações. Durante os testes, não foi identificada uma
forma clara de fazer esse aviso deixar de aparecer nessas áreas. Mesmo após
interação com o sino de notificações, o indicador visual continua ativo, e o
aviso permanece visível no dashboard de forma persistente.
Passos para reproduzir
- Acessar Administrativo > Avisos .
- Criar um novo aviso.
- Retornar para a página inicial do sistema.
- Observar o dashboard e o sino de notificações.
- Interagir com o sino e verificar o comportamento posterior.
Resultado obtido
O aviso criado permanece sendo exibido no dashboard.
O indicador no sino de notificações continua ativo.
Não há opção clara para dispensar, ocultar ou marcar o aviso como já
visualizado.
O aviso permanece visível de forma contínua, mesmo após interação do
usuário.
Evidências
Prints:
Relatório de T estes - Sistema Igrejas
5

Ponto Identificado 03
Título
Mensagens de carregamento e ausência de dados permanecem em inglês em
diferentes módulos do sistema
Severidade
Média
Ambiente
Administrativo > Avisos
Administrativo > Calendário
Aplicativo > Dízimos e Ofertas
Departamento Infantil > Check-in/Checkout
Gestão de Pessoas > Aconselhamento
Gestão de Pessoas > Visitantes
Gestão de Pessoas > Membros
Observação
Relatório de T estes - Sistema Igrejas
6

O problema não foi identificado em Gestão de Pessoas > Famílias .
Descrição
Durante os testes, foi observado que, enquanto a pesquisa está em execução,
o sistema exibe a mensagem Loading items... , e quando não há resultados
encontrados, exibe No data available . Essas mensagens permanecem em inglês,
independentemente do idioma selecionado no sistema.
Passos para reproduzir
- Acessar um dos módulos afetados.
- Utilizar um campo de pesquisa da tela.
- Observar a mensagem exibida enquanto os dados estão sendo carregados.
- Realizar uma busca sem resultados.
- Observar a mensagem exibida quando não há dados encontrados.
Resultado obtido
Durante a pesquisa, o sistema exibe Loading items... .
Quando não há resultados, o sistema exibe No data available .
As mensagens permanecem em inglês mesmo com o sistema configurado
em outro idioma.
Evidências
Prints:
Relatório de T estes - Sistema Igrejas
7

Ponto Identificado 04
Relatório de T estes - Sistema Igrejas
8

Título
Campo de data e hora apresenta valor de exemplo com aparência de dado já
preenchido
Severidade
Baixa
Ambiente
Formulários de cadastro
Exemplo observado em Nova Turma
Descrição
Ao abrir o formulário para cadastro de um novo item, o campo de data e hora
apresenta um valor visível por padrão, como 12:30 . Embora esse valor funcione
apenas como exemplo visual, ele se parece com um dado já preenchido no
campo. Isso pode induzir o usuário a acreditar que a informação já foi inserida
corretamente, quando na prática o sistema ainda considera o campo
obrigatório e não preenchido.
Passos para reproduzir
- Acessar uma tela de cadastro, como Nova Turma .
- Localizar o campo de data e hora.
- Observar que um horário aparece visivelmente dentro do campo.
- Tentar prosseguir sem preencher manualmente o valor.
Resultado obtido
O campo exibe um valor visual que parece preenchimento real.
O usuário pode interpretar que não precisa informar o dado.
Mesmo com esse valor aparente, o sistema continua tratando o campo
como vazio.
Evidências
Prints:
Relatório de T estes - Sistema Igrejas
9

Ponto Identificado 05
Título
Menus Perfil  e Configurações  direcionam para a mesma página
Severidade
Baixa
Ambiente
Menu do usuário
Opções Perfil  e Configurações
Descrição
Durante os testes, foi observado que os menus Perfil  e Configurações  levam
para a mesma página. Embora isso não impeça o uso do sistema, a navegação
fica ambígua, pois os dois itens aparentam ter finalidades diferentes, mas
executam o mesmo comportamento.
Passos para reproduzir
- Acessar o menu do usuário.
- Clicar na opção Perfil .
- Observar a página aberta.
- Retornar ao menu do usuário.
- Clicar na opção Configurações .
- Comparar o destino das duas opções.
Resultado obtido
Relatório de T estes - Sistema Igrejas
10

As opções Perfil  e Configurações  levam para a mesma tela.
Não há distinção prática entre os dois menus.
A interface sugere funcionalidades diferentes, mas o comportamento é
idêntico.
Evidências
Prints:
Relatório de T estes - Sistema Igrejas
11

Relatório de T estes - Sistema Igrejas
12
