---
layout: post
title: Desigualdade de Género na Toponomia de Lisboa
date: 2022-11-19 00:00:00 +0300
description: Quantas ruas têm nome de homem? Existem mais do que ruas ocm nomes de mulheres? # Add post description (optional)
img: logo_dif_genero.png # Add image post (optional)
tags: [desigualdes, gendergap, toponomia, python, lisboa, homem, mulher] # add tag
---

# Introdução

As ruas são uma parte fundamental das nossas cidades e comunidades. Os nomes das ruas são por isso também, uma forma de homenagear e lembrar as pessoas que fizeram contribuições importantes para a nossa sociedade. Infelizmente, as ruas são desproporcionadamente designadas com nomes de homens, refletindo a desigualdade de género que ainda existe em muitas áreas da nossa sociedade. Ações de reequilibrio, nomeadamente através de ruas com nomes de mulheres para reconhecer o importante papel desempenhado pelas mulheres na nossa história e nas nossas cidades.

O aumento de ruas com nomes de mulheres pode ajudar a combater essa desigualdade e reconhecer o importante papel desempenhado pelas mulheres. Isso pode inspirar as mulheres a continuarem a lutar pelos seus direitos e a alcançarem sucesso nas suas carreiras e vidas pessoais. Além disso, pode ajudar a educar as pessoas sobre as mulheres que fizeram contribuições importantes para a nossa sociedade, e inspirar as futuras gerações.

É precisamente por isso que decidi fazer uma análise que tente mostrar a desigualdade que existe, atualmente, na distribuição de ruas com nomes de mulheres quando comparado com ruas com nomes de homem. O mesmo foi feito para jardins, escolas e hospitais na cidade de Lisboa.

# Metodologia e tratamento de dados

Usando dados da toponomia disponíveis pela Câmara Municipal de Lisboa em dados abertos, foi possível adicionar informação sobre a origem e biografia da pessoa que dá nome à rua, ano em que foi dado o nome atual, ou mesmo o nome pela qual era anteriormente conhecida.

Como nem todas as ruas têm um nome referente a uma mulher ou homem, foram classificadas apenas as ruas onde isso era possível. Foram também excluídas ruas que tenham apenas um nome próprio, isto porque torna-se difícil identificar a origem dessa personalidade.
Ruas de homens ou mulheres com apenas um nome próprio não foram contabilizadas (ex: Rua Maria).
Obteve-se assim 3 resultados possíveis para ruas:
- Homem
- Mulher
- N/A (Não aplicável)

# Resultados

## Toponomia

Quando olhamos para distribuição geral das ruas, verificamos que temos praticamente 5 mil ruas no concelho de Lisboa.
Dessas, conseguimos classificar X como sendo ruas com nomes de homens ou mulheres.
Quando olhamos para a distribuição das que conseguimos classificar, este é o cenário:

[INTRODUZIR GRÁFICO PIE]

No mapa abaixo conseguimos visualizar as todas as ruas de Lisboa por género:

<iframe src="https://manuelbanza.github.io/Artigos/Toponomia_DIferenca_Genero/01.Toponomia_Ruas_Genero_read_only.html" height="700px" width="100%"></iframe>

Para ver mapa interactivo em versão mobile ou em ecrá completo clique [AQUI](https://manuelbanza.github.io/Artigos/Toponomia_DIferenca_Genero/01.Toponomia_Ruas_Genero_read_only.html)

Ao clicar numa rua podemos fica a saber mais sobre a sua origem, data em que passou a ter esse nome ou até saber qual a designação anterior.

**E qual a distribuição do género ao longo do tempo?**

Pelos dados de toponomia disponíveis no portal de dados abertos, consiguimos ter a data edital da grande parte das ruas aqui analisadas, mas não a sua totalidade. Dessa forma para os que têm data conseguimos fazer uma análise para perceber a distribuição ao longo das últimas décadas:

<iframe src="https://manuelbanza.github.io/Artigos/Toponomia_DIferenca_Genero/ANO_vs_Genero.html" height="700px" width="100%"></iframe>

Como podemos ver o cenário não tem vindo a melhorar significativamente, mesmo quando olhamos para os ultimos anos.

## Jardins e Parques

Quando aplicamos o mesmo raciocínio para os jardins e parques de Lisboa vemos que o cenário é ligeiramente melhor. Se olharmos apenas para os que é possível identificar se o nome é de homem ou mulher, vemos que **17% dos jardins e parques têm nomes de mulheres.**

![Género nos Jardins e Parques]({{site.baseurl}}/assets/img/parques_genero.png)

teste:
![Género nos Jardins e Parques]({{site.baseurl}}/assets/img/parques.svg)


Abaixo o mapa onde é possível explorar por género:

<iframe src="https://manuelbanza.github.io/Artigos/Toponomia_DIferenca_Genero/02.Jardins_Genero_read_only.html" height="700px" width="100%"></iframe>

Para ver mapa interactivo em versão mobile ou em ecrá completo clique [AQUI](https://manuelbanza.github.io/Artigos/Toponomia_DIferenca_Genero/02.Jardins_Genero_read_only.html)


## Escolas

Já na escolas o cenário é ainda melhor. Dos possíveis de classificar,vemos que **25% das escolas têm nomes de mulheres.**
Nas escolas incluímos as do 1º, 2º, 3º ciclo e secundárias.
No total existem 242 escolas distintas com informação georreferenciada no portal de dados abertos da Câmara Municipal de Lisboa.

Abaixo o mapa das escolas com informação do género:

![Género nas Escolas]({{site.baseurl}}/assets/img/escolas_genero.png)


Abaixo o mapa onde é possível explorar por género:

<iframe src="https://manuelbanza.github.io/Artigos/Toponomia_DIferenca_Genero/03.Escolas_Genero_read_only.html" height="700px" width="100%"></iframe>

Para ver mapa interactivo em versão mobile ou em ecrá completo clique [AQUI](https://manuelbanza.github.io/Artigos/Toponomia_DIferenca_Genero/03.Escolas_Genero_read_only.html)


## Hospitais

Por último, foram também analisados os hospitais, tanto públicos como privados (26 no total).
O cenário é bastante semelhante ao dos parques, com **18% dos hospitais em Lisboa a terem nomes de mulheres.**

Abaixo o mapa dos hospitais com informação do género:

![Género nos Hospitais]({{site.baseurl}}/assets/img/hospitais_genero.png)



<iframe src="https://manuelbanza.github.io/Artigos/Toponomia_DIferenca_Genero/04.Hospitais_Genero_read_only.html" height="700px" width="100%"></iframe>

Para ver mapa interactivo em versão mobile ou em ecrá completo clique [AQUI](https://manuelbanza.github.io/Artigos/Toponomia_DIferenca_Genero/04.Hospitais_Genero_read_only.html)


# Conclusão

Como vimos nas visualizações acima, ainda existem poucas ruas, parques, escolas e hospitais com nomes de mulheres quando comparados com os que existem com nomes de homens.
Para além disso, muitos dos nomes de mulheres são nomes de santas ou de rainhas, mais do que nos homens em percentagem de cada género.

No entanto é nas ruas que talvez consigamos alterar esta desigualdade mais rapidamente.
Existem várias razões pelas quais ainda existe uma grande descrepância entre as ruas com nomes de homens e mulheres. Em primeiro lugar, a história da maioria das sociedades tem sido contada principalmente pelos homens, e é por isso que a maioria das figuras históricas lembradas nas ruas são homens. Além disso, as mulheres enfrentam ainda muitas barreiras e desafios nas suas carreiras e vidas pessoais, o que as impede, potencialmente, de alcançar o mesmo nível de reconhecimento e sucesso que os homens. Isso faz com que haja menos mulheres a serem lembradas e homenageadas nas ruas.

O objetivo desta análise foi apenas quantificar esta desigualdade e tentar que se inicíe o debate que é o mais produtivo, o de pensarmos em nomes de mulheres que tiveram um papel importante na cidade ou no país e que aind anão estam nas ruas de Lisboa. 
Que sugestões têm?


# Notas

Todos os dados usados foram obtidos através dos portais de dados abertos disponíveis da Câmara Municipal de Lisboa.O trabalho foi possível graças à aposta que a Câmara de Lisboa tem feito ao longo de vários dados na disponibilização de dados ao público.
Os dados abertos promovem a transparência e a participação cívica, permitindo que os cidadãos acedam facilmente aos dados das suas cidades.




[NOTA- OUTROS GÉNEROS[]