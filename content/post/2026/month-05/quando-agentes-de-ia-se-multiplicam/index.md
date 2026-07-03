---
title: "Quando agentes de IA se multiplicam"
description: "Uma reflexão sobre como os agentes de IA evoluíram e o papel dos MCPs na criação de aplicações inteligentes."
date: 2026-05-26 00:00:00+0000
image: quando-agentes-de-ia-se-multiplicam.jpg
categories:
  - blog
tags:
  - estudo
  - ia
  - machine-learning
  - data-science
---

Até 2 anos atrás, pedir para a Inteligência Artificial criar um código funcional – algo que **realmente funcione** – era um parto. Durante a faculdade no início de 2020, eu brincava com chatbots pedindo para que ajudassem com meus códigos. Mesmo que simples, as IAs nunca acertavam, os arquivos e funções nunca se conectavam e minha solução continuava quebrada.

Recentemente, ao explorar o Bob, o novo agente de IA da IBM, fiquei surpresa. Pedi para que ele criasse um novo agente do zero para traduzir as mensagens que eu mandasse. Claro, eu poderia pedir para que o próprio Bob as traduzisse, mas dessa forma não teria graça.

Bob foi capaz de criar o ambiente, conectar o servidor, as funções e os modelos, além de criar a documentação completa. Fui estudar o que cada arquivo fazia, pois fiquei muito curiosa sobre como tudo aquilo rodou, e consegui entender melhor como um agente de IA funciona por trás das câmeras.

Nesse artigo, viso mostrar um pouco mais da anatomia de uma IA e conectar alguns termos famosos com seu funcionamento prático.

---

## IAs nada mais são do que funções probabilísticas
No meu artigo anterior, explico como Inteligência Artificial não é um conceito novo. Ao dar um pulinho em redes neurais, vimos que o algoritmo retorna o resultado “menos errado” após uma série de cálculos estatísticos. Em suma, um Large Language Model (LLM) – o que comumente chamamos de IA – correlaciona proximidade entre termos.

Ao pesquisar “a cor do céu é…” no ChatGPT por exemplo, o LLM fará uma pesquisa em uma base de dados gigantesca, além de vários cálculos, para retornar o resultado mais provável para o que você está pesquisando: a cor do céu é azul.

A mesma coisa ocorre com números, por exemplo: ao digitar 8 ? 8 = 16, é altamente provável que isso seja uma soma, então a máquina retorna “+” para substituir a interrogação. Esse é o funcionamento básico de qualquer modelo, ele supõe a provável alternativa correta com base em dados disponíveis. É por isso, também, que não podemos confiar cegamente neles.

É importante ressaltar que, neste experimento, fiz apenas um agente criar outro agente, e não uma LLM inteira. Ou seja, o modelo já existe, só foi criada uma camada de aplicação que faz uso desse modelo, traduzindo as mensagens que eu mando.

---

## Mas as IAs não estão mais inteligentes?
Mais ou menos. As Inteligências Artificiais continuam resolvendo questões determinísticas (ou seja, sem margem para o acaso), como realizar cálculos matemáticos ou dizer que dia é hoje. A grande sacada foi um certo equilíbrio entre o determinístico e o probabilístico por meio do conceito de MCP (Model Context Protocol).

Lá para meados de 2024, uma empresa chamada Anthropic (sim, a mãe do Claude) propôs uma ponte entre a linguagem natural (mais próxima dos humanos) e a linguagem “da máquina”, permitindo que uma ação determinística (direta) seja processada por meio de linguagem natural, acarretando em novas possibilidades de funcionamento. Praticamente um passo a passo detalhado para a máquina. Meu colega de IBM, [Glauco Reis](https://www.linkedin.com/in/glaucoreis/), possui um [artigo aqui no LinkedIn](https://www.linkedin.com/pulse/como-o-bob-pensa-glauco-reis-lenif/) explicando MCPs de uma forma simples, vale dar uma olhada!

Um exemplo utilizando nosso caso de uso, a criação do agente tradutor:

> Bob, crie um agente de IA que traduza minhas mensagens. Configure ambiente, modelo e documentação.

Com o MCP, o Bob “quebra” essas instruções usando linguagem natural, acarretando em novas ramificações e possibilidades. Como resultado, a máquina “pensa” em passo a passo detalhado:

1. “Definir o comportamento do tradutor *(quais comportamentos? A máquina decide!)*
2. Empacotar como um serviço A2A
3. Integrá-lo com o framework *(ela decidiu o framework)*
4. Torná-lo configurável e testável *(ela decidiu as configurações com base no ambiente e setup)*
5. Documentar e corrigir o ambiente de execução”

Após o Bob criar o agente de IA, pedi para ele atualizar a documentação, um arquivo markdown simples. Minha mensagem foi apenas: “Insira uma lista de comandos e um passo a passo sobre como iniciar o servidor e o modelo já instalados”.

A resposta do Bob, com um passo a passo detalhado e mais possibilidades:

1. “Atualizei o arquivo com uma seção adicional de início rápido para instalações já existentes.
2. Adicionei um fluxo de trabalho mais curto com três terminais para reutilização após a configuração inicial.
3. Mantive as instruções completas de configuração inicial.
4. O guia de início rápido agora abrange apenas 3 arquivos”

![A resposta do Bob, em linguagem natural](https://media.licdn.com/dms/image/v2/D4D12AQGR1dMVf7OsUw/article-inline_image-shrink_1500_2232/B4DZ5FgS1oIMAQ-/0/1779282554431?e=1782345600&v=beta&t=PqyqN8uClriVq_8Qvzv8fdMHjGc9CHaLu4C3xtM1PNE)

---

## Tá, mas por que isso é tão impressionante?
A grande questão do uso dos MCPs é que, ao utilizá-los, você permite que um MCP chame vários outros MCPs, acarretando em milhões de possibilidades. De todas essas ramificações, como uma máquina é capaz de acertar o suficiente a ponto de rodar um servidor e um modelo sem a interferência técnica de outro ser humano?

O fato de que, até dois anos atrás, não conseguíamos criar códigos com um chatbot que se conectassem de forma funcional; e hoje, em 2026, uma Inteligência Artificial materializar um código do zero na minha frente, com tudo funcionando, me surpreende.

Tudo o que precisei fazer foi digitar uma linha de comando e observar a máquina construir tudo sozinha. Dentre tantas possibilidades, ela retornou apenas 2 erros (que também foram resolvidos por ela mesma), e voilá: nosso agente tradutor nasceu.

![O agente traduzindo a frase que enviei](https://media.licdn.com/dms/image/v2/D4D12AQHkv3JFT1-KHA/article-inline_image-shrink_1500_2232/B4DZ5Fgec0HIAU-/0/1779282602072?e=1782345600&v=beta&t=rrtydEy91qchJ1m8ybkOyiEPkt8C3gB9Nwmf8b-eHj0)

É claro que a IA não faz tudo isso de graça. Todos os prompts que enviamos para a máquina consomem tokens, principalmente os mais subjetivos que abrem ainda mais margem para as MCPs. Mas isso é assunto para outro artigo. Por agora, espero ter conseguido passar um pouco da minha surpresa ao aprender um pouco mais sobre como as IAs funcionam.

Talvez eu seja apenas facilmente impressionável, mas o acaso sempre me fascinou muito.
