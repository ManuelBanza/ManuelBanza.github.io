---
layout: post
title: Desigualdade de Género na Toponomia de Lisboa
date: 2022-11-19 00:00:00 +0300
description: Quantas ruas têm nome de homem? Existem mais do que ruas ocm nomes de mulheres? # Add post description (optional)
img: logo_dif_genero.png # Add image post (optional)
tags: [desigualdes, gendergap, toponomia, python, lisboa, homem, mulher] # add tag
---

# Introdução

As ruas são uma parte fundamental das nossas cidades e comunidades, e os nomes das ruas são uma forma de homenagear e lembrar as pessoas que fizeram contribuições importantes para a nossa sociedade. Infelizmente, a maioria das ruas tem nomes de homens, refletindo a desigualdade de gênero que ainda existe em muitas áreas da nossa sociedade. É importante que existam mais ruas com nomes de mulheres para equilibrar essa desigualdade e reconhecer o importante papel desempenhado pelas mulheres na nossa história e na nossa sociedade.

Existem várias razões pelas quais ainda existe uma grande descrepância entre as ruas com nomes de homens e mulheres. Em primeiro lugar, a história da maioria das sociedades tem sido contada principalmente pelos homens, e é por isso que a maioria das figuras históricas lembradas nas ruas são homens. Além disso, as mulheres enfrentam ainda muitas barreiras e desafios em suas carreiras e vidas pessoais, o que as impede de alcançar o mesmo nível de reconhecimento e sucesso que os homens. Isso faz com que haja menos mulheres a serem lembradas e homenageadas nas ruas.

O aumento de ruas com nomes de mulheres pode ajudar a combater essa desigualdade e reconhecer o importante papel desempenhado pelas mulheres na nossa sociedade. Isso pode inspirar as mulheres a continuarem lutando pelos seus direitos e a alcançarem sucesso em suas carreiras e vidas pessoais. Além disso, pode ajudar a educar as pessoas sobre as mulheres que fizeram contribuições importantes para a nossa sociedade, e inspirar as futuras gerações.

É precisamente por isso que decidi fazer uma análise que tente mostrar a desigualdade que existe na distribuição de ruas com nomes de mulheres quando comparado com ruas com nomes de homem.

Como nem todas as ruas têm um nome referente a uma mulher ou homem, foram classificadas apenas as ruas onde isso era possível. Foram tabém excluídas ruas que tenham apenas um nome próprio, isto porque torna-se difícil identificar a origem dessa personalidade.

# Metodologia e tratamento de dados

Usando dados da toponomia disponíveis pela CML em dados abertos, foi possível adicionar informação sobre a origem ou biografia da pessoa que dá nome à rua, ano em que foi dado o nome atual, ou mesmo o nome pela qual era anteriormente conhecida.

Neste projecto o objetivo é quantificar a diferença que existe entre ruas com nomes de homens e mulheres. Para isso usou-se a informação da toponomia de Lisboa e classificou-se por género.
Para a cliassifcação de homem e mulher, apenas se considerou as que tem um nome possível de identificar. Ruas de homens ou mulheres com apenas um nome próprio (ex: Rua Maria) não foram contabilizadas.
Obteve-se assim 3 resultados possíveis para ruas:
- Homem
- Mulher
- N/A (Não aplicável)

# Resultados

Quando olhamos para distribuição geral das ruas, verificamos que temos praticamente 5 mil ruas no concelho de Lisboa.
Dessas conseguimos classificar X como sendo ruas com nomes de homens ou mulheres.
Quando olhamos para a distribuição das que conseguimos classificar, este é o cenário:

[INTRODUZIR GRÁFICO PIE]

No mapa abaixo conseguimos visualizar as todas as ruas de Lisboa por género:

<iframe src="https://manuelbanza.github.io/Artigos/Toponomia_DIferenca_Genero/01.Toponomia_Ruas_Genero_read_only.html" height="700px" width="100%"></iframe>

Para ver mapa interactivo em versão mobile ou em ecrá completo clique [AQUI](https://manuelbanza.github.io/Artigos/Toponomia_DIferenca_Genero/01.Toponomia_Ruas_Genero_read_only.html)


