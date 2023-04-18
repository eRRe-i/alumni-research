---
title: "2. Fundamentação Teórica"
type: chapter
status: "⚠️"
enableToc: false
---
# 2. Fundamentação Teórica

Este capítulo abordará a respeito  dos Graduate Tracking Systems (GTS), iniciando com um breve histórico e a motivação para a existência dos mesmos, o que é preciso levar em consideração ao elaborar um GTS e o estado da arte, com as principais características dos modelos de maior sucesso.

Um dos objetivos parciais deste capítulo é informar quais as principais decisões de design que precisam ser tomadas quando se pensa em um GTS. É comum, no desenvolvimento de um GTS, que algumas decisões não estejam claras para responsável. Questões como:

- quais os objetivos do GTS, ou, quais as perguntas que o GTS busca responder?
- quais as partes interessadas no GTS e quais delas podem fazer uso dos dados?
- quais os tipos de dados que serão necessários para atender aos objetivos do projeto?
- Esses dados estão disponíveis? Estão agregados?

Quanto mais clareza o responsável pelo GTS tem na etapa de design, menos problemas surgirão no momento da implementação.

Ao levantar quais os objetivos, possíveis partes interessadas e quais os dados disponíveis podem abrir novas linhas de atuação para o GTS.

Deste modo, espera-se que esta obra contribua para a contínua discussão sobre a melhoria do sistema através da captura de mais dados, geração de mais inteligência sobre esses dados, a inclusão de novos objetivos e novas partes interessadas, possibilitando, deste modo, a extensão do sistema em uma próxima iteração do desenvolvimento.

## 2.1 O que são Graduate Tracking Systems (GTSs)?

Graduate Tracking Systems, também conhecidos como Graduate Career Tracking Systems (GCTSs) [[bibliografia/sipo2017graduate]], e também Acompanhamento ou Monitoramento de Egressos (SMEs) [[bibliografia/paul2015acompanhamento]] são esforços, incentivados principalmente por governos ou Instituições de Ensino Superior (IESs), em acompanhar seus estudantes egressos. GTSs focam no desenvolvimento de sistemas que, baseados nos dados coletados sobre os estudantes egressos que passaram pelo curso ou universidade, permite traçar, perfis e tendências sobre os egressos a partir dos dados coletados.

Segundo [[bibliografia/gaebel2012tracking]] o monitoramento consiste em informações de "estudantes e graduados a respeito do processo de aprendizado, percepções, emprego, em pelo menos dois momentos no tempo, através de dados no nível individual e agregado, coletados principalmente via processos administrativos e questionários".

É preciso salientar que os GTSs podem variar largamente em suas abordagens e métodos, dependendo de vários fatores como: acesso a dados administrativos, os objetivos definidos no \emph{design} do GTS, a forma de coleta dos dados etc.

Outras vezes, GTSs são moldados pelo contexto nacional ou interinstitucional. Universidades podem agir conjuntamente desenvolver experiências comuns e permitir que os dados interinstitucionais possam ser comparados. Governos nacionais, por sua vez, podem liderar tais esforços, e contribuir para enriquecê-lo com outras bases administrativas. \footnote{O caso das instituições europeias claramente seguem essas duas tendências: sendo moldado tanto pela existência de modelos institucionais de sucesso, como o Alma Laurea; passando por consórcio de instituições com o objetivo de estabelecer práticas comuns e, por fim, com o envolvimento dos estados nacionais em estabelecer bases de dados unificadas no âmbito governamental e a criação de diretrizes gerais para o desenvolvimento de GTSs.} \footnote{Podemos verificar a evolução no esforço das instituições europeias no desenvolvimento de experiências supranacionais nas publicações pesquisadas. Em 2012, a Associação das Universidades Europeias publicou o TRACKIT, provendo informações sobre as experiências de monitoramento de egressos. Em 2020, a Comissão Europeia encomenda \emph{Graduate tracking: a 'how to do it well' guide}, cujo objetivo é auxiliar os governos nacionais a fundamentar e fortalecer suas medidades de monitoramento de egressos. O fato de que tais publicações tenham ocorrido de forma tão recente parece indicar que ainda há um amplo espaço para o desenvolvimento da área}

[[bibliografia/sipo2017graduate]], em seu esforço para identificar tendências em um amplo espectro de experiências internacionais, identifica essas tendências nas práticas de GTSs: uma abordagem \emph{top-down} orientada a políticas governamentais, abordagem  \emph{top-down} orientada a políticas educacionais, e soluções tradicionais baseadas interações em pesquisas institucionais fracamente gerenciadas". \footnote{Embora não esteja evidenciado no trabalho de Sipos, é entendimento deste trabalho que tais abordagem por ora se entrelacem.}


## 2.2 Histórico e Motivações para o desenvolvimento de GTS

A motivação para o desenvolvimento de GTSs parece advir de dois fatores. O primeiro foram as mudanças quantitativas e organizacionais no ensino superior, junto a pressões do mercado de trabalho impulsionaram tais mudanças em especial a partir da década de 60-70.

A massificação pela busca do diploma de ensino superior, juntamente com a inserção de instituições privadas colocou uma forte pressão sobre as instituições financiadas pelo estado a respeito da qualidade dos alunos, o que, por sua vez, faz com que o mercado e as instituições tenham a preocupação a performance dos graduados no mercado de trabalho. [[bibliografia/sipo2017graduate]]

Os estados nacionais, por sua vez, tem a preocupação de acompanhar e assegurar a qualidade das instituições de ensino para justificar o financiamento governamental. [[bibliografia/sipo2017graduate]].

[[bibliografia/gaebel2012tracking]] corrobora esse raciocínio, justificando a importância do monitoramento atestando que: "com a participação crescente da educação superior, a empregabilidade e entrada no mercado de trabalho torna-se um critério mais importante para avaliar o provisionamento da educação superior" (p. 8).


(Talvez fundamentar melhor como essas mudanças têm acontecido??)

Embora as universidades tenham mantido sua posição de prestígio no mercado, houve um declínio no entendimento do papel da universidade \footnote{um marco deste movimento foi o Processo de Bolonha, em especial o comprometimento com a aplicação de um sistema de garantia de qualidade, onde as iniciativas de GTSs se inserem}, de um modelo clássico de ensino para um modelo de massa, com a criação de cursos online massivos e a redução da interação professor-aluno em uma economia baseada em criação de valor.


Para [[bibliografia/paul2015acompanhamento]]: "o conjunto desses elementos, que fazem do ensino superior um universo cada vez mais complexo num contexto evolutivo de trabalho, exige um sistema de informação confiável e transparente quanto ao seu modo de funcionamento e seus resultados. Essas informações são necessárias tanto para entender o funcionamento social do sistema como para ajudar os poderes públicos, famílias e os estudantes a definirem suas opções em termos de financiamento e de carreira".

Logo, o segundo fator que colabora para o interesse em GTSs é o desenvolvimento das Tecnologias de Informação e Comunicação. 

Esses dois fatores explicam a retomada dos estudos com pesquisas dos egressos observada por [[bibliografia/paul2015acompanhamento]], antes realizadas por sociólogos e economistas e, hoje em dia, consolidados em políticas de garantia de qualidade de educação superior e criação de bases de dados nacionais como métrica dessa política e dispositivos nacionais que apoiam a pesquisa continuada, com forte apoio de sistemas de informação. 

Em alguns casos, tais medidas significaram a adequação das IES às exigências de prestação de contas 


## 2.3 Objetivos de um GTS

Os trabalhos de [[bibliografia/gaebel2012tracking]] e [[bibliografia/tracking2020EU]], parecem indicar um esforço presente nas universidades europeias em fomentar uma cultura de monitoramento de egressos, bem como um esforço conjunto para coletar dados comparáveis entre as IES na Europa.

## 2.4 Principais características de um GTS

Esta seção é responsável por mostrar as principais características e decisões a serem tomadas ao considerar o desenvolvimento de um GTS. Os objetivos, o público que se deseja atender e as restrições que o projeto tem servem como o ponto de partida para a decisão por quais características o modelo escolhido terá. Isso, associado com o que é desenvolvido na literatura sobre GTS. Este capítulo lida com a definição das decisões do caso de negócio e decisões operacionais, sobre que tipo de coleta de dados. Este tema está inserido principalmente nas seções 2 e 3 de [[bibliografia/tracking2020EU]]