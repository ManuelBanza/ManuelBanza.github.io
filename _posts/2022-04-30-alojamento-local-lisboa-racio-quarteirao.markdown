---
layout: post
title: E se as regras do alojamento local fossem ao nível do quarteirão? | Manuel Banza |
date: 2022-04-26 00:00:00 +0300
description: Em Março de 2022 Lisboa decidiu suspender novas licenças de alojamento local por 6 meses. Terminado esse periodo, como podemos criar novas regras com um um maior detalhe e justiça que apenas ao nível da freguesia? # Add post description (optional)
img: heatmap_rnal.png # Add image post (optional)
tags: [alojamento local, lisboa, turismo, hotelaria, licenças, datascience, spatial data science] # add tag
---

Há já vários anos que o debate sobre o impacto do alojamento local no sector da habitação em Lisboa tem vindo a ser tema quente, seja em altura de eleições, ou fora delas.
Existem opiniões diferentes sobre a emissão de novas licenças, que se dividem à esquerda e à direita dos partidos portugueses.
Em Março de 2022 os partidos de esquerda juntaram-se para aprovar a [suspensão de novas licenças por um período de 6 meses](https://eco.sapo.pt/2022/03/22/lisboa-aprova-suspensao-de-novos-registos-de-alojamento-local-em-14-freguesias/), em freguesias em que o rácio entre licenças de alojamento local e número de habitações fosse superior a 2.5%, até à entrada em vigor da alteração ao Regulamento Municipal desta atividade.
Nas últimas semanas ficámos também a saber, que esta medida fez disparar o [aumento em 382% face a igual período de 2021 e de 25% em comparação com 2019](https://www.dinheirovivo.pt/economia/alojamento-local-em-lisboa-dispa-382-a-boleia-da-suspensao-de-novos-registos-14777622.html).
Para além disso ficámos também a saber que segundo um estudo intitulado ["O Mercado Imobiliário em Portugal”, coordenado pelo economista Paulo Rodrigues, com financiamento pela Fundação Francisco Manuel dos Santos (FFMS)](https://www.publico.pt/2022/04/04/economia/noticia/precos-casas-cairam-9-onde-proibidos-novos-alojamentos-locais-2001068), a limitação e suspenção de novas licenças feitas no passado em certas zonas com alta pressão turística, teve o efeito de baixar o preço das casas em 9%. Provando que a suspensão pode ser uma boa ferramenta para ajudar a combater a crise habitacional que existe em Lisboa.

No entanto, limitar uma freguesia por inteiro poderá penalizar certas zonas em que não existe pressão ou procura de alojamento local, bem como o seu contrário, freguesias que não atingem o rácio 2.5% mas que um determinada zona já tem uma pressão turística elvada e superior a 2.5%

É precisamente sobre estes últimos desenvolvimentos, que é necessário fazer uma análise que englobe um nível de detalhe mais granular que a freguesia e tentará ser feito neste artigo.


## Como?

De modo a criar regras mais abrangentes e adequadas à realidade de cada bairro de Lisboa, urge uma análise a uma escala mais granular e que represente melhor as diferentes realidades de Lisboa.
Dessa forma nesta análise foi usada a localização de cada licença válida atualmente, bem como os dados provisórios dos CENSOS 2021 ao nível da [BGRI (Base Geográfica de Referenciação de Informação)](https://www.ine.pt/ngt_server/attachfileu.jsp?look_parentBoui=107197&att_display=n&att_download=y). 
Esta base geográfica permite analisar a informação relativa a alojamentos destinados a habitação, e ao nível de quarteirões, dando assim um detalhe importante para esta análise, mas protegendo a identidade dos habitantes destes alojamentos. No final deste artigo falarei das fontes e características destes dados usados.

#### Métricas de Análise
Que métricas podemos então usar para avaliar o impacto do Alojamento Local em cada zona ou bairro específico de Lisboa?
Uma que podemos certamente usar, é a relação entre número de alojamentos destinados para habitação, identificados pelos CENSOS 2021, e o número de licenças atribuídas para alojamento local nessa mesma BGRI (quarteirão). Ou seja para x alojamentos de habitação, quantos existem na mesma área para alojamento local, já com licença atríbuida.
De forma a simplificar a análise irei filtrar apenas as BGRI (quarteirões) que tiverem um rácio (definido no parágrafo acima) superior a 2.5%, já que foi este o valor que foi usado para a suspensão de licenças nos próximos 6 meses. 
O objetivo deste artigo é apenas iniciar o debate sobre o tema com os dados atualmente disponíveis e em formato de dados abertos. O desejado é que a definição de qual o valor a ser usado, seja os 2.5% ou outro valor, seja o resultado do debate entre toda a população.
Para além desta métrica foram criados outros rácios como se pode verificar na imagem abaixo:

![Rácios]({{site.baseurl}}/assets/img/racios_al.png)

Sendo que uma das coisas que estamos a avaliar é a pressão turística e não apenas o alojamento local, é importante arranjar formas que contabilizem o sector hoteleiro, nomeadamente os empreendimentos turísticos comos os hotéis, neste rácio.
Embora as realidades entre os hotéis e o alojamento local sejam bem distintas, ambos contribuem para a oferta turística da cidade.
Dessa forma decidi criar outra análise que contablize o número de alojamentos referentes aos hotéis em Lisboa. Sendo que o número de alojamentos corresponderá ao número de quartos que cada hotel tem. Esta é a forma mais correcta para podermos agregar licenças de alojamento local com hoteís, visto que o número de camas irá sempre depender da dimensão de cada um.

## Resultados
#### Hotel vs AL
Atualmente no concelho de Lisboa existem 20187 licenças atribuídas para alojamento local. Quando olhamos para o número de alojamentos de empreendimentos turísticos o número passa a 22808.

![Número de Alojamentos]({{site.baseurl}}/assets/img/numero_alojamentos.png)
Dados referentes a Abril de 2022


<img src="ttps://manuelbanza.github.io/mapaarroios.github.io/numero_alojamentos.png" width="500" height="300" />

Ou seja, apesar de serem bem diferentes entre si, vemos que a diferença em unidades de alojamento já não é muito diferente.
O sector do turismo tem sido nos últimos anos um dos sectores que mais emprega trabalhadores não só em Lisboa mas em Portugal. Este boom turístico após a crise, foi também um dos sectores que permitiu o crescimento e retoma económica.
No entanto é importante fazer uma distinção entre o impacto de um hotel e de um alojamento local, sendo o mais óbvio, o número de empregos que são gerados em cada um.
Um hotel necessita de muitos mais trabalhadores para oferecer o seu serviço, empregando assim um valor superior de funcionários.
Outra vantagem é também ao nível da segurança, visto que a maioria dos hotéis tem durante o dia e noite, seguranças à entrada do hotel, podendo ou não transmitir um sensação de maior segurança na zona em questão.
Com isto não podemos esquecer, o impacto que muitos alojamentos locais tiveram na reabilitação de edifícios nos bairros mais históricos, e náo só, de Lisboa. Além do potencial para dinamizar o sector de restauração e comércio.


#### Alojamento Local
No gráfico abaixo podemos visualizar as tais BGRI (quarteirões) em que o rácio de licenças de alojamento local sobre o número de alojamento habitacionais dos CENSOS 2021 é superior a 2.5%. A escala começa no amarelo quase branco nos casos em que o rácio é 2.5%, e à medida que o rácio aumenta o tom passa a ser mais vermelho. Nos casos em que a cor mantém-se igual ao mapa, são as zonas onde o rácio é inferior a 2.5% ou náo existem habitações nos CENSOS 2021.
Neste mapa não foram contabilizados os empreendimentos turísticos mas apenas alojamentos locais.

<iframe src="https://manuelbanza.github.io/mapaarroios.github.io/02_BGRI2021_Licencas_AL_READ_ONLY.html" height="700px" width="100%"></iframe>

Para ver mapa interactivo em versão mobile ou em ecrá completo clique [AQUI](https://manuelbanza.github.io/mapaarroios.github.io/02_BGRI2021_Licencas_AL_READ_ONLY.html)

![Exemplo de exploração do mapa]({{site.baseurl}}/assets/img/gif_01.gif)

Conseguimos perceber que apesar de freguesias como Campolide e Beato não terem sido abrangidas pela suspensão de licenças, têm zonas onde o rácio é superior a 2.5%. Se pegarmos no exemplo do Beato é fácil de perceber que a maioria dos alojamentos locais estão numa parte da cidade que tem vindo a ser mais frequentada nos últimos anos, tendo por isso já uma pressão turística consideravél.
Por outro lado, vemos que existem freguesias como a Penha de França e Areeiro, que entraram na lista de suspensão, mas que têm várias zonas em que não há pressáo turística, pois esta está concentrada em zonas específicas da freguesia

#### Hotelaria
E se considerarmos os hotéis neste rácio? Teremos valores diferentes?
Na imagem abaixo verificamos que sim:

<iframe src="https://manuelbanza.github.io/mapaarroios.github.io/04_BGRI2021_Licencas_AL_Empreendimentos_Turisticos_read_only.html" height="700px" width="100%"></iframe>

Para ver mapa interactivo em versão mobile ou em ecrá completo clique [AQUI](https://manuelbanza.github.io/mapaarroios.github.io/04_BGRI2021_Licencas_AL_Empreendimentos_Turisticos_read_only.html)

Verificamos assim que o rácio passa a ser bastante mais elevado, como seria expectável, e que zonas com as Avenidas Novas e Estrela passam a ter valores mais expressivos.


## Próximos passos
Com os dados aqui apresentados, podemos analisar em maior detalhe cada zona da cidade. Estes resultados podem ajudar na definição de novas regras que podem entrar na elaboração das alterações ao Regulamento Municipal desta atividade.
Podemos iniciar o debate sobre outros valores para o rácio, outras métricas, ou outras variáveis a adiconar ao cálculo do rácio aqui aplicado.
Não devem ser excluídos ainda, outros futuros projectos de emprendimentos turísticos, como hotéis, já em construção, aprovados ou em fase de aprovação por parte do Turismo de Portugal e Câmara Municipal de Lisboa.



## Dados
Para a elaboração desta análise foram usados os seguintes dados:

###### Dados Alojamento Local e Empreendimentos Turísticos
Os dados com a informação geográfica de cada licença foram obtidos através da plataforma de dados abertos desenvolvida pelo Turismo de Portugal, [TravelBI](https://travelbi.turismodeportugal.pt/)

###### CENSOS 2021
Os dados ao nível de cada BGRI, foram obtidos através do site do [INE](http://mapas.ine.pt/download/index2021.phtml), que disponibilizou recentemente esta informação como dados provisórios. Assim que forem disponibilizados os dados definitivos, os mapas e rácios serão atualizados.

Toda a transformação, tratamento de dados, e criação de mapas foi feita e programada exclusivamente em python.
Última atualização dos dados a 26 de Abril de 2022.


