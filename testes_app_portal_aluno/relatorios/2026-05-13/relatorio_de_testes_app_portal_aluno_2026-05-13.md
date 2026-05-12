# Relatório de Testes - App Portal Aluno

## Informações Gerais

| Campo | Informação |
| --- | --- |
| Sistema testado | App Portal Aluno |
| Data de início | 2026-05-13 |
| Data final / entrega | 2026-05-13 |
| Versão testada | 1.0.28 |
| Compilação / build | 58 |
| Dispositivo | iPhone 15 Pro Max |
| Versão do iOS | 26.5 |
| Responsável pelo teste | Raphael |

## Resumo Executivo

Foi realizada uma nova rodada de validação no App Portal Aluno, versão 1.0.28 build 58, com foco nos problemas persistentes do relatório anterior, nos pontos corrigidos informados posteriormente e nas dúvidas de regra de negócio que ainda estavam abertas.

Durante a validação, dois problemas permaneceram ativos: quebra de layout com fonte grande no smartphone e instabilidade no player de áudio ao arrastar a barra de progresso. Os demais pontos testados foram confirmados como corrigidos, considerados comportamento esperado ou removidos da lista de erros por regra de negócio.

Total de pontos identificados: 2

## Pontos Identificados

### Ponto Identificado 01

#### Título

Quebra de layout quando a fonte do smartphone está grande

#### Ambiente

- App Portal Aluno > iOS 26.5 / TestFlight > Build 58
- Dispositivo: iPhone 15 Pro Max
- Configurações do smartphone com fonte aumentada

#### Descrição

Ao aumentar o tamanho da fonte nas configurações do smartphone e navegar pelo aplicativo, algumas partes da interface continuam desconfiguradas. Foram observados desalinhamentos, quebras visuais e elementos fora do comportamento esperado.

O problema já havia sido identificado em rodada anterior e permaneceu ativo nesta nova validação.

#### Passos para reproduzir

1. Aumentar o tamanho da fonte nas configurações do smartphone.
2. Abrir o App Portal Aluno.
3. Navegar pelas telas principais do aplicativo.
4. Observar o comportamento visual dos elementos da interface.

#### Resultado obtido

Com a fonte grande ativada, algumas áreas do aplicativo continuam quebrando visualmente, com elementos desalinhados ou desconfigurados.

#### Impacto

Prejudica a usabilidade e a acessibilidade do aplicativo para usuários que utilizam fonte ampliada no smartphone.

#### Evidências

Prints:

- Evidência não anexada neste relatório.

### Ponto Identificado 02

#### Título

Player de áudio continua apresentando instabilidade ao arrastar a barra de progresso

#### Ambiente

- App Portal Aluno > iOS 26.5 / TestFlight > Build 58
- Dispositivo: iPhone 15 Pro Max
- Matérias disponíveis > Player de áudio

#### Descrição

Ao abrir o áudio de uma matéria e arrastar a bolinha da barra de progresso para outro ponto, o comportamento instável permanece. A bolinha continua oscilando entre posições e o áudio fica mudo por um período após a ação.

O problema já havia sido identificado em rodada anterior e permaneceu ativo nesta nova validação.

#### Passos para reproduzir

1. Acessar uma matéria com áudio disponível.
2. Iniciar a reprodução do áudio.
3. Arrastar a bolinha da barra de progresso para outro ponto.
4. Soltar a bolinha e observar o comportamento do player.

#### Resultado obtido

A bolinha da barra de progresso continua oscilando após o arrasto. O áudio também fica mudo por algum tempo antes de voltar a reproduzir normalmente.

#### Impacto

Prejudica a experiência do aluno ao consumir aulas ou conteúdos em áudio, especialmente quando tenta avançar ou retornar para um ponto específico da reprodução.

#### Evidências

Prints ou gravação:

- Evidência não anexada neste relatório.

## Validações Confirmadas

Os pontos abaixo foram validados nesta rodada e não devem permanecer como erros em aberto:

- Campo "Estado" na edição de perfil: não é erro. Quando o cadastro está configurado como endereço brasileiro, é esperado que apareçam apenas estados do Brasil. Para usuário internacional, a configuração precisa ser feita no cadastro/liberação do usuário.
- Datas da seção Financeiro em francês e japonês: corrigido. As datas não aparecem mais em formato de código.
- Caracteres especiais no endereço: corrigido. Caracteres como "ç" e acentos estão sendo aceitos.
- Gesto de voltar: funcionando normalmente, sem retornar indevidamente para a tela de login.
- Card "Pagamentos": abre corretamente a área de "Meu Histórico / Financeiro".
- Busca em "Meu Histórico / Acadêmico": reinicia corretamente ao sair e voltar.
- Busca em "Matérias Disponíveis": reinicia corretamente ao sair e voltar.
- Botão de salvar no perfil: está posicionado corretamente na parte inferior e não cobre mais os campos.

## Pontos De Regra De Negócio Validados

Os pontos abaixo foram retirados da lista de dúvidas/validações porque foram confirmados como comportamento esperado ou funcionalidade não ativa:

- Notícias: ao abrir uma notícia, o usuário pode navegar pelo portal conforme comportamento validado.
- Financeiro: pagamentos efetuados sem abertura de comprovante foram considerados resolvidos/validados.
- Matérias disponíveis: é esperado que apenas "Aliança de Sangue" tenha áudio disponível.
- Notícias por idioma: os cards de notícias não precisam mudar de idioma junto com o app, pois a funcionalidade não está ativa.

## Conclusão

O App Portal Aluno versão 1.0.28 build 58 confirmou correções e esclareceu pontos de regra de negócio, mas dois problemas permanecem ativos: quebra de layout com fonte grande e instabilidade no player de áudio ao manipular a barra de progresso.
