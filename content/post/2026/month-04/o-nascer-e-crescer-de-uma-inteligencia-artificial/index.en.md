---
title: "The Rise of an Artificial Intelligence"
description: "Uma visão sobre IA como um objeto de estudo com ciclo de vida, métricas e responsabilidade em projetos de Machine Learning."
date: 2026-04-28 00:00:00+0000
image: o-nascer-e-crescer-de-uma-inteligencia-artificial.jpeg
categories:
  - blog
  - data-science
  - design
  - photography
tags:
  - study
  - ia
  - machine-learning
  - data-science
---

Esses dias meu pai me presenteou com o livro *Uma Biografia da Depressão*, do Christian Dunker. Nele, somos apresentados à depressão como um objeto de estudo que nasce, vive e morre; quando foram seus primeiros diagnósticos, quem são suas “irmãs mais velhas” (melancolia e angústia), e até mesmo elabora uma “entrevista” com a depressão para um entendimento ainda mais lúdico. Ótimo livro, recomendo.

Neste artigo, viso fazer algo parecido: a IA deixa de ser uma “entidade”, muitas vezes atrelada à solução de todos os problemas, e se torna um objeto de estudo com ciclo de vida, metrificação e razão para existir, diferente do que se prega hoje em dia com o *boom* do Machine Learning.

### O DNA de uma IA

O termo “Inteligência Artificial” é, na realidade, bastante antigo. Como afirma Victor Sobreira no artigo [Um panorama da História da Inteligência Artificial e suas aplicações na pesquisa histórica](https://www.scielo.br/j/vh/a/rBFnX4gCZ4N8fcRt6mjxbFQ/?format=pdf&lang=pt): “Por mais atual que a discussão sobre IA possa parecer, bem como os seus impactos em nossa sociedade contemporânea do século XXI, a reflexão sobre o assunto é tão antiga quanto a própria invenção do computador".

Grande parte disso se dá pelas descobertas de Alan Turing na década de 1950, que desafiou uma máquina a pensar. Lembra-se do filme “Jogo da Imitação”? Pois bem; imagine que no lugar das pessoas, coloca-se uma máquina, e os seres humanos precisam dizer se o terceiro elemento enviando informações é um computador ou não. A questão não é a máquina ser inteligente, mas sim *parecer* inteligente o suficiente para se passar como um ser humano.

Para aprimorar essa “imitação" conceitualizada por Alan Turing, nos baseamos na biologia e adoramos fazer paralelos. Da comparação entre um neurônio nasce o algoritmo Perceptron, que forma a base do conceito de redes neurais.

Imagine que a comunicação entre um neurônio e outro é realizada por milhares de sinapses (na imagem abaixo, os dendritos), que se traduzem como impulsos guiados por um condutor (este sendo o axônio), até o próximo neurônio.

![Article content](https://media.licdn.com/dms/image/v2/D4D12AQEQibQwJn6qnA/article-inline_image-shrink_1500_2232/B4DZ3QWZwsHwAU-/0/1777317027603?e=1782345600&v=beta&t=OsC12tlan_R0LoffbmUjfX5jVN9IDpNQC9w1gHmZ4KM)

Funcionamento de um neurônio

No aprendizado de máquina temos algo relativamente parecido. No algoritmo, as sinapses ocorrem, como na imagem abaixo, entre variáveis X1, X2, Xn; e o lance é encontrar um ponto em comum entre todas elas, para retornar em Y (o final do nosso neurônio) uma única saída.

Difícil, considerando que os dados (ou em nosso exemplo, os impulsos) que o Perceptron recebe são todos diferentes. Como isso pode se traduzir em apenas uma única saída? E como sabemos que essa **única saída** é a menos errada?

![Article content](https://media.licdn.com/dms/image/v2/D4D12AQE1dJHHAcz8Pw/article-inline_image-shrink_1000_1488/B4DZ3QW0dyI4AQ-/0/1777317136991?e=1782345600&v=beta&t=0VtS92FNXcXMEO-Zpw4PDqu1f_ATW7hNoU_0OAdzuxw)

Funcionamento de um Perceptron

É por isso que nosso neurônio fará dezenas de cálculos na bolinha azul (representado pelo sinal de sigma) e ponderará esses cálculos probabilísticos na função f(S), para retornar apenas uma saída provável em Y. Todos esses cálculos são feitos de maneira muito rápida.

Mas como sabemos que essa saída provável é a menos errada? Afinal, estamos trabalhando com probabilidade e estatística. O Perceptron visa diminuir as chances de erro. Para isso, utiliza o conceito de retro-propagação (backpropagation), recalculando tudo o que ele fez até agora, várias vezes, até retornar um ponto onde o erro dos “impulsos”, ou variáveis, seja mínimo.

![Conceito de backpropagation](https://media.licdn.com/dms/image/v2/D4D12AQGg1wSaS8rebw/article-inline_image-shrink_1000_1488/B4DZ3QXC0HG8AU-/0/1777317195854?e=1782345600&v=beta&t=Mpwm1tEgjKpMtKQsLA7L5tgoq-oTu7cdaBIE2QEkEeY)


Com isso, nascem os primeiros conceitos de aprendizagem de máquina e redes neurais. É com essa tentativa e erro que a máquina aprende, com cálculos, pesos e resultados anteriores. Não é mágica, por mais que pareça e seja mais fácil acreditar nisso, né?

### Essa família é muito unida

Diferente de nós, seres humanos, a IA necessita de uma justificativa para nascer e viver. Ou pelo menos *deveria*, porque ninguém quer usar um tanque de guerra para matar uma formiga. Dito isso, antes de parir nossa Inteligência Artificial, temos nossa “obstetra”: a Análise de Dados.

> É por meio da análise de dados que entenderemos em quais condições nossa IA nascerá, quais problemas ela resolverá e os principais casos de uso afetados por ela.

Por exemplo: eu, como executivo da Netflix, analisei que o acesso à plataforma está baixo e quero evitar o churn de clientes. Com base nos números, podemos colocar uma IA que recomende mais filmes de comédia apenas com os atores que o usuário mais gosta. Dessa forma, poderemos reter clientes e aumentar o interesse com o catálogo.

A análise de dados apresentou o problema. Caso o uso de Inteligência Artificial seja justificável e bom o suficiente para nossa situação, a mãe, Ciência de Dados, entra em jogo. É por meio dela que vamos parir nossa IA e seguiremos uma *pipeline*, um processo.

Temos algumas ramificações na área de Machine Learning quanto ao tratamento dos dados. É importante que entendamos a função de cada uma na pipeline antes de colocar nossa IA no mundo.

O Engenheiro de Dados prepara todo o ambiente por meio da limpeza e tratamento dos dados. É como se fosse a doula cuidando da sala de parto para receber a mãe. Essa área mexe mais com os dados crus e operações em banco de dados, sejam eles estruturados ou não. Se almeja essa área, prepare-se para mexer com **muito** SQL.

O Cientista de Dados, junto do Engenheiro, começam o desenvolvimento de um modelo preditivo de aprendizagem de máquina, que é o que conhecemos como Inteligência Artificial. Para o Cientista estão as responsabilidades de treinar e testar o modelo, entendendo se ele minimiza os erros, como vimos anteriormente.

Com nossa IA no mundo, começam as idas ao médico para acompanhar se está tudo bem. Esse trabalho fica a encargo do Engenheiro de Machine Learning, que cuidará da automação, deploy, curadoria dos dados e monitoramento do modelo, utilizando ferramentas como Spark e Data Lakes.

![Ciclo de vida de uma IA](https://media.licdn.com/dms/image/v2/D4D12AQEd3M_C6PIqFg/article-inline_image-shrink_1000_1488/B4DZ3U4OP6HkAQ-/0/1777393002981?e=1782345600&v=beta&t=JBnKX_fTGvOY333gP6sGFd23wRsy91Q3uhq7lOn5H9w)


De forma mais sucinta, o roadmap de um projeto de IA, como explicou [Laura Damaceno de Almeida](https://www.linkedin.com/in/laura-data-talks/) no meetup da [CODECON](https://www.linkedin.com/company/codecon-event/) em Março deste ano, conta com 5 macro etapas de estruturação.

1. Pesquisa: entendimento do problema. Analista de dados, estou falando com você!;
2. Riscos e alternativas: quais riscos o modelo pode ter? Quais os impactos e o que podemos fazer para mitigá-los? Geralmente, é feito pela equipe de negócios;
3. Fluxo de testes: vamos saber se nosso modelo funciona como o esperado se testarmos muito. É a vez dos Cientistas entrarem em ação;
4. Rotulamento humano: um-de-nós vai analisar e ver se a IA não está alucinando. O Engenheiro de Machine Learning vai liderar essa parte;
5. Comparação com performance humana: cálculo de métricas, compreender como está a performance do nosso modelo e armazenamento em um banco de dados. Um trabalho em conjunto do Engenheiro de Machine Learning, passando para o Engenheiro de Dados novamente.

### Vida escolar de uma IA

Nosso projeto cresceu! Assim como o acompanhamento da vida escolar de um ser humano, aplicamos métricas e validações para entender se nossa IA está se comportando da maneira devida. É importante fazer isso pois dados ficam obsoletos, e dados obsoletos geram análises enviesadas, impactando o negócio. Quanto mais liberdade seu modelo tem, maior precisa ser o acompanhamento.

Alguns exemplos de métricas são:

- Experiência (o usuário teve que formular várias vezes a mesma pergunta para o modelo entender?);
- Confiabilidade (as respostas são plausíveis?);
- Negócio (retenção de usuários/clientes, aumento de produtividade…);
- Técnicas (desempenho do modelo e *accuracy* dos resultados, por exemplo).

O uso das métricas depende do objetivo de cada modelo. Cada projeto é único!

É importante ressaltar que o estudo com a IA não termina quando vai para produção. Temos algumas validações que podem ser feitas para garantir que o modelo é confiável. Essa parte está mais presente na Engenharia de Machine Learning, como comentamos há pouco. Chamamos de tríade da validação, composta pelo teste unitário, pela avaliação por agente (o qual chamamos de “Juiz"), e pela avaliação humana.

O teste unitário visa avaliar o nível de confiabilidade da informação que a IA retorna para o usuário, além de garantir que o resultado siga o formato esperado. A avaliação por agente (o Juiz) ocorre logo após o teste unitário e garante que a IA não extraiu informações incorretas. Por fim, temos a avaliação humana, que acontece em espaçamentos maiores de tempo. O humano avaliará o nível de concordância entre o Juiz e a IA, e garantirá que as informações estão de acordo com o esperado.

![Os 3 testes de validação](https://media.licdn.com/dms/image/v2/D4D12AQFN1v6nsMgRPw/article-inline_image-shrink_1000_1488/B4DZ3U4Vk4HwAQ-/0/1777393033690?e=1782345600&v=beta&t=VUZh5MXNxTWW266ssBcK8dFlcGV7FYB0zHvDLL7XryQ)


---

### Você precisa mesmo de uma IA no seu projeto?

Antes de iniciar um projeto envolvendo Inteligência Artificial, tenhamos em mente que a fase de pesquisa e o mapeamento de riscos são de suma importância. Eu disse, no início deste artigo, que ninguém quer usar um tanque de guerra para matar uma formiga. Muitas vezes, os problemas que identificamos com a Análise de Dados não são suficientes para justificar o uso de uma IA, gastos com armazenamento, API, banco de dados e mão de obra qualificada – sendo que, muitas vezes, poderia ser resolvido com uma simples árvore de decisão. Não é à toa que um dos maiores desafios do campo de IA atualmente seja reduzir os custos financeiros e ambientais com hardware e memória.

A avaliação de desempenho é algo que muitas pessoas pecam ao desenvolver projetos de Machine Learning. Não basta colocar a IA no mundo; se você não cuidar dos dados com carinho, facilmente se tornam obsoletos e comprometem seu negócio. Por isso, temos 3 perguntas que podem te ajudar nessa jornada:

- Como estamos avaliando nosso sistema de IA? Estamos fazendo as perguntas corretas?
- Quais métricas indicam que ele funciona bem?
- O que acontece quando ele erra?

Com todo esse *boom* sobre IA no século XXI, é de suma importância que entendamos que um modelo de Machine Learning não nasce pronto. Ele possui três pilares: boas métricas, monitoramento, e talvez o mais importante: responsabilidade com o que está sendo entregue.

---

### Desventuras em projetos reais de Inteligência Artificial

Para fechar, trouxe uma mini-entrevista com a Laura Damasceno durante o meetup da Codecon. No momento das dúvidas, quisemos muito saber como funcionam os projetos de Machine Learning no dia a dia.

**Laura, como você avalia o momento certo de adotar a estratégia de um agente de IA, por conta de todo esse hype?**

A parte da pesquisa, o primeiro passo, faz a gente entender o problema de negócio. Se for, por exemplo, para conferir a tendência de compra de um cliente, poderia muito bem ser um *boolean* ou uma árvore de decisão. Dito isso, se usarmos IA, seria um canhão para algo relativamente simples. Utilizar IA é caro, demanda mais tempo e gastos com API, armazenamento… muitas vezes uma simples árvore de decisão resolveria. Gosto de dar no mínimo duas sugestões para o cliente, pois muitas vezes não é necessária uma Inteligência Artificial.

**Como você lida quando a IA alucina muito?**

Geralmente tentamos resolver com Engenharia de Prompt, porque talvez a pergunta possa ser melhorada. Se não resolver, então talvez tenhamos que reformular o modelo, e aí é mais complicado.

**Qual a história mais cabulosa que você já viu de quando um agente não foi bem manipulado?**

Durante um projeto, a IA analisava diferentes imagens. Em determinado momento, perguntamos se existia fogos de artifício nas fotos de uma loja. Toda vez ela respondia que sim, tinham fogos de artifício lá dentro!

Quando os humanos checaram durante a validação, não enxergamos fogos de artifício nenhum. Era uma farmácia.

**Dentro do ambiente de startup, como balancear esse brilho da curiosidade com a pressão?**

Eu tenho a parte de formação acadêmica muito forte, gosto de testar muito, e o mercado tem um tempo diferente. Mesmo assim, para balancear, eu costumo selecionar uma parte pequena porém significativa de amostras na fase de testes. Dessa forma, elas permanecem diversas e eu consigo entender padrões e vieses de forma mais confiável.

**Que conselho você daria para Laura de uns anos atrás que estava iniciando em dados?**

Não tenha medo de errar. Tenta, veja se é pra você. Não tenha medo de lidar com erros. A área de IA tem N caminhos para seguir, e o ponto principal é não perder sua essência e a alegria.

Temos que errar e descobrir problemas para inovar sobre eles. Não tenha medo de testar, experimentar, propor coisas novas. Não perca sua essência.

![Eu e Laura no meetup da Codecon](https://media.licdn.com/dms/image/v2/D4D12AQGNGPij8RM30A/article-inline_image-shrink_1000_1488/B4DZ3QYblrHkAQ-/0/1777317562597?e=1782345600&v=beta&t=RoWcO1nU5DljGFiI1Xgj06W_EOzIm5EpJC5ogYrD_x8)


Foi muito divertido estudar sobre o tema para essa News, que contou com ótimas aulas do meu mentor, [Bruno Rafael Matiucci](https://www.linkedin.com/in/bruno-matiucci-data-scientist/), e conversas com a própria Laurinha. Obrigada por tanto conhecimento compartilhado e toda paciência ao longo dessa jornada. Vocês são incríveis!

Tem algum assunto específico que você tem vontade de entender sobre IA? Coloque sua sugestão nos comentários, e nos vemos em breve. Até logo :)

---

### Referências e créditos

[Redes Neurais Artificiais: o perceptron - Jorge Centeno](https://docs.ufpr.br/~centeno/p_iarha/pdf/aula008_perceptron.pdf)

[Mãos à obra: aprendizado de máquina com Scikit-Learn, Keras & TensorFlow - Aurélien Géron](https://www.amazon.com.br/M%C3%A3os-obra-aprendizado-Scikit-Learn-inteligentes/dp/8550815489)

[Um panorama da História da Inteligência Artificial e suas aplicações na pesquisa histórica - Victor Sobreira](https://www.scielo.br/j/vh/a/rBFnX4gCZ4N8fcRt6mjxbFQ/?format=pdf&lang=pt)
