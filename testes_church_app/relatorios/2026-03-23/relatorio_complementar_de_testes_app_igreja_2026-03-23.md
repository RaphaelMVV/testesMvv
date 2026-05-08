Relatório Complementar de
Testes - App Igreja
Informações do teste
Branch testada: validation
Data do teste complementar final: 23 de março de 2026
Observação geral
Durante esta nova rodada de testes, verifiquei que os problemas reportados
anteriormente continuam acontecendo. Além disso, identifiquei novos pontos
relacionados ao fluxo de cadastro internacional e tradução.
Continuidade dos problemas anteriores
Os erros já reportados anteriormente continuam aparecendo, sem correção
perceptível até o momento, incluindo:
validação de cadastro por e-mail que não conclui
comportamento incorreto do Picture in Picture
Verbo FM tocando junto com vídeos
notícia em destaque abrindo sem conteúdo
link do YouTube com falha no conteúdo em destaque da Home
link do YouTube com falha na seção Contatos
compartilhamento sem envio do link do conteúdo
imagem da notícia cortada no modo paisagem
barra de progresso do vídeo mudando de tamanho
seek rápido pausando o vídeo
tela de ofertas sem dados bancários
texto cortado com fonte grande no iPhone
menu de edição de texto aparecendo em inglês
Relatório Complementar de T estes - App Igreja
1

Novos problemas identificados
1. Cadastro internacional não aceita código postal no formato
do país
No fluxo de cadastro internacional, o campo de código postal continua
funcionando como se fosse um CEP brasileiro.
Na prática:
o campo aceita apenas padrão brasileiro
não aceita formatos internacionais
Relatório Complementar de T estes - App Igreja
2

isso dificulta ou impede o preenchimento correto por usuários de outros
países
2. Tradução do campo de endereço não está no contexto da
língua francesa
No cadastro em francês, o campo “Estado” aparece traduzido como État .
Para o contexto de endereço utilizado no app, esse termo não está no contexto
correto da língua francesa. O esperado seria utilizar uma nomenclatura mais
apropriada ao contexto, como Département .
3. Campo “Bairro” permanece obrigatório em francês
No cadastro em francês, o campo “Quartier” está obrigatório.
Relatório Complementar de T estes - App Igreja
3

Porém, em algumas cidades menores da França, esse tipo de divisão de bairro
não é utilizado da mesma forma. Por isso, deixar esse campo obrigatório pode
dificultar ou até impedir o preenchimento correto do endereço.
O esperado seria:
tornar esse campo não obrigatório em contextos internacionais/franceses,
ou
adaptar a obrigatoriedade conforme o país selecionado
Conclusão
Além de os erros já relatados anteriormente continuarem ocorrendo, esta nova
rodada de testes confirmou problemas adicionais no fluxo de cadastro
internacional e na adaptação de tradução para francês.
Relatório Complementar de T estes - App Igreja
4
