---
layout: post
title: E se as regras do alojamento local fossem ao nível do quarteirão? | Manuel Banza |
date: 2022-04-26 00:00:00 +0300
description: Em Março de 2022 Lisboa decidiu suspender novas licenças de alojamento local por 6 meses. Terminado esse periodo, como podemos criar novas regras com um um maior detalhe e justiça que apenas ao nível da freguesia? # Add post description (optional)
img: heatmap_rnal.png # Add image post (optional)
tags: [alojamento local, lisboa, turismo, hotelaria, licenças, datascience, spatial data science] # add tag
---

Há vários anos que o debate sobre o impacto do alojamento local no sector da habitação em Lisboa tem vindo a ser tema quente, seja em altura de eleições, ou não.
Existem opiniões diferentes sobre a emissão de novas licenças, que dividem os partidos à esquerda e à direita.
Em Março de 2022 os partidos de esquerda juntaram-se para aprovar a [suspensão de novas licenças por um período de 6 meses](https://eco.sapo.pt/2022/03/22/lisboa-aprova-suspensao-de-novos-registos-de-alojamento-local-em-14-freguesias/), em freguesias em que o rácio entre licenças de alojamento local e número de habitações fosse superior a 2.5%, até à entrada em vigor da alteração ao Regulamento Municipal desta atividade.
Nas últimas semanas ficámos também a saber, que esta medida fez aumentar [em 382% face a igual período de 2021 e de 25% em comparação com 2019](https://www.dinheirovivo.pt/economia/alojamento-local-em-lisboa-dispa-382-a-boleia-da-suspensao-de-novos-registos-14777622.html).
Recentemente surgiu também um estudo intitulado ["O Mercado Imobiliário em Portugal”, coordenado pelo economista Paulo Rodrigues, com financiamento pela Fundação Francisco Manuel dos Santos (FFMS)](https://www.publico.pt/2022/04/04/economia/noticia/precos-casas-cairam-9-onde-proibidos-novos-alojamentos-locais-2001068), que indica que a limitação e suspenção de novas licenças feitas no passado em certas zonas com alta pressão turística, teve o efeito de reduzir o preço das casas em 9%. Provando que a suspensão pode ser uma boa ferramenta para ajudar a combater a crise habitacional que existe em Lisboa.

No entanto, limitar uma freguesia por inteiro poderá penalizar certas zonas em que não existe pressão ou procura de alojamento local, bem como o seu contrário, freguesias que não atingem o rácio 2.5% mas que um determinada zona já tem uma pressão turística elevada e superior a 2.5%.

É precisamente por estes últimos desenvolvimentos e limitações do modelo atual, que é necessário criar uma ferramenta com mais detalhe e que ajude na tomada de decisões.

## Como?

De modo a criar regras mais abrangentes e adequadas à realidade de cada bairro de Lisboa, urge uma análise a uma escala mais granular e que represente melhor as diferentes realidades de Lisboa.
Dessa forma nesta análise foi usada a localização de cada licença válida atualmente, bem como os dados provisórios dos CENSOS 2021 ao nível da [BGRI (Base Geográfica de Referenciação de Informação)](https://www.ine.pt/ngt_server/attachfileu.jsp?look_parentBoui=107197&att_display=n&att_download=y). 
Esta base geográfica permite analisar a informação relativa a alojamentos destinados a habitação, e ao nível de quarteirões, dando assim um detalhe importante para esta análise. No final deste artigo falarei das fontes e características destes dados usados.

#### Métricas de Análise
Que métricas podemos então usar para avaliar o impacto do Alojamento Local em cada zona ou bairro específico de Lisboa?
Uma possibilidade, é a relação entre número de alojamentos destinados para habitação, identificados pelos CENSOS 2021, e o número de licenças atribuídas para alojamento local nessa mesma BGRI (semelhante a um quarteirão). Ou seja para x alojamentos de habitação, quantos existem na mesma área para alojamento local, já com licença atríbuida.
De forma a simplificar a análise irei filtrar apenas as BGRI que tiverem um rácio (definido no parágrafo acima) superior a 2.5%, já que foi este o valor que foi usado para a suspensão de licenças nos próximos 6 meses. 
O objetivo deste artigo é apenas iniciar o debate sobre o tema com os dados atualmente disponíveis e em formato de dados abertos. O desejado é que a definição de qual o valor a ser usado, seja os 2.5% ou outro valor, seja o resultado do debate entre toda a população.
Para além desta métrica foram criados outros rácios como se pode verificar na imagem abaixo:

![Rácios]({{site.baseurl}}/assets/img/racios_al.png)

Sendo que uma das coisas que estamos a avaliar é a pressão turística e não apenas o alojamento local, é importante arranjar formas que contabilizem o sector hoteleiro, nomeadamente os empreendimentos turísticos comos os hotéis, neste rácio.
Embora as realidades entre os hotéis e o alojamento local sejam bem distintas, ambos contribuem para a oferta turística da cidade.
Dessa forma decidi criar outra análise que contabilize o número de alojamentos referentes aos hotéis em Lisboa. Sendo que o número de alojamentos corresponderá ao número de quartos que cada hotel tem. Esta é a forma mais correcta para podermos agregar licenças de alojamento local com hotéis, visto que o número de camas irá sempre depender da dimensão de cada um.

## Resultados
#### Hotel vs AL
Atualmente no concelho de Lisboa existem 20.187 licenças atribuídas para alojamento local. Quando olhamos para o número de alojamentos de empreendimentos turísticos este valor é de 22.808.

![Número de Alojamentos]({{site.baseurl}}/assets/img/numero_alojamentos.png)
Dados referentes a Abril de 2022

Ou seja, apesar de serem bem diferentes entre si, vemos que a diferença em unidades de alojamento já não é muito diferente.
O sector do turismo tem sido nos últimos anos um dos sectores que mais emprega trabalhadores, não só em Lisboa mas em Portugal. Este boom turístico foi também, em parte, o que permitiu o crescimento e retoma económica após a crise da década passada.
No entanto é importante fazer uma distinção entre o impacto de um hotel e de um alojamento local. Por um lado os hotéis acabam por empregar mais trabalhadores, contudo não podemos esquecer o impacto que muitos alojamentos locais tiveram na reabilitação de edifícios nos bairros mais históricos, e náo só. Além do potencial para dinamizar o sector de restauração e comércio.


#### Alojamento Local
No gráfico abaixo podemos visualizar as tais BGRI (quarteirões) em que o rácio de licenças de alojamento local sobre o número de alojamentos habitacionais dos CENSOS 2021 é superior a 2.5%. A escala começa no amarelo quase branco nos casos em que o rácio é 2.5%, e à medida que o rácio aumenta o tom passa a ser mais vermelho. Nos casos em que a cor mantém-se igual ao mapa, são as zonas onde o rácio é inferior a 2.5% ou náo existem habitações nos CENSOS 2021.
Neste mapa não foram contabilizados os empreendimentos turísticos mas apenas alojamentos locais.

<iframe src="https://manuelbanza.github.io/mapaarroios.github.io/02_BGRI2021_Licencas_AL_READ_ONLY.html" height="700px" width="100%"></iframe>

Para ver mapa interactivo em versão mobile ou em ecrá completo clique [AQUI](https://manuelbanza.github.io/mapaarroios.github.io/02_BGRI2021_Licencas_AL_READ_ONLY.html)

Exemplo de exploração do mapa:
![Exemplo de exploração do mapa]({{site.baseurl}}/assets/img/gif_01.gif)
Ao clicar ou passar o rato numa área conseguimos obter informação não só do rácio de licenças AL sobre nº de alojamentos, mas também os outros rácios referidos acima.
É também possivel obter informação da licença AL e data de emissão da mesma.

Conseguimos perceber que apesar de freguesias como Campolide e Beato não terem sido abrangidas pela suspensão de licenças, têm zonas onde o rácio é superior a 2.5%. Se pegarmos no exemplo do Beato é fácil de perceber que a maioria dos alojamentos locais estão numa parte da cidade que tem vindo a ser mais frequentada nos últimos anos, tendo por isso já uma pressão turística consideravél.
Por outro lado, vemos que existem freguesias como a Penha de França e Areeiro, que entraram na lista de suspensão, mas que têm várias zonas em que não há pressáo turística, pois esta está concentrada em zonas específicas da freguesia.
Este mapa deve ser sempre analisado em conjunto com os outros rácios e valores, visto que em certos casos, temos zonas que estãoa  vermelho mas que têm muito poucos alojamentos de habitação, atingindo fácilmente um rácio superior a 2.5%, como é o caso de Carnide na zona nordeste de Lisboa.

#### Alojamento Local + Hotelaria
E se considerarmos e adicionarmos os hotéis neste rácio? Teremos valores diferentes?
Na mapa abaixo verificamos que sim:

<iframe src="https://manuelbanza.github.io/mapaarroios.github.io/04_BGRI2021_Licencas_AL_Empreendimentos_Turisticos_read_only.html" height="700px" width="100%"></iframe>

Para ver mapa interactivo em versão mobile ou em ecrá completo clique [AQUI](https://manuelbanza.github.io/mapaarroios.github.io/04_BGRI2021_Licencas_AL_Empreendimentos_Turisticos_read_only.html)

Verificamos assim que o rácio passa a ser bastante mais elevado, como seria expectável, e que zonas com as Avenidas Novas e Estrela passam a ter valores mais expressivos.

Quando analisamos as BGRI com rácios mais elevados, verificamos o top 10 ou mesmo 15, sáo localizadas em apenas 3 Freguesias: Santa Maria Maior, Misericórdia e Santo António. Foram precisamente estas freguesias que mais perderam residentes face a 2011, segundos os dados dos CENSOS 2021 agregados à Freguesia e [possível de visualizar neste artigo.](https://amensagem.pt/2021/08/07/censos-centro-historico-lisboa-perde-oito-mil-habitantes-menos-lares-mais-alojamento-local-turismo/)
Levanta-se assim a questão dos preços das casas nestas zonas terem vindo a sofrer um aumento muito elevado na última década, que fez com que muitos locais deixassem de puder pagar os valores praticados.

#### Média Móvel Espacial
Outra forma de analisarmos os resultados é aplicando a média móvel espacial, também conhecida por spatial lag, usada em Ciência de Dados Geoespaciais. A Média Móvel Espacial pode ser entendida como uma média ponderada de uma variável pelas localizações vizinhas. Ou seja, considera o impacto que as zonas vizinhas têm numa determinada zona, e como influenciam os valores de cada uma delas.
Neste caso, uma BGRI não pode ser analisada isoladamente(o rácio que calculámos), mas sim com as outras BGRI vizinhas com que faz fronteira. 
Dessa forma os rácios passam a ter valores diferentes, inclusive em zonas que não tinham rácios acima de 2.5% ou mesmo qualquer tipo de licença AL, Hotel ou unidade alojamento.
Este tipo de análises devem também ser usadas quando há tomadas de decisões que envolvam informações geográficas.
Abaixo podemos ver o mapa com o Rácio de Licenças AL + Empreendimentos Turísticos sobre o N° de Alojamentos de Habitação, já com a média móvel espacial aplicada e apenas as BGRI com rácios superiores ou iguais a 2.5%:

<iframe src="https://manuelbanza.github.io/mapaarroios.github.io/05_Spatial_Lag_BGRI2021_Licencas_AL_Empreendimentos_Turisticos_read_only.html" height="700px" width="100%"></iframe>

Para ver mapa interactivo em versão mobile ou em ecrá completo clique [AQUI](https://manuelbanza.github.io/mapaarroios.github.io/05_Spatial_Lag_BGRI2021_Licencas_AL_Empreendimentos_Turisticos_read_only.html)

Neste caso vemos que existem diferenças entre BGRI vizinhas, passando a ter valores mais próximos entre si, também por serem precisamente vizinhas e partilharem o impacto. Como é perceptível na zona histórico de Lisboa.
No oposto, vemos casos como na zona perto do aeroporto, que deixam de ter um rácio superior a 2.5%, visto não haver tanta pressão túristica nas zonas vizinhas.

## Próximos passos
Com os dados aqui apresentados, podemos analisar em maior detalhe cada zona da cidade. Estes resultados podem ajudar na definição de novas regras que podem entrar na elaboração das alterações ao Regulamento Municipal desta atividade. Podemos iniciar o debate sobre outros valores para o rácio, outras métricas, ou outras variáveis a adicionar ao cálculo do rácio aqui aplicado. Sem nunca esquecer o que os dados já nos dizem e o que os últimos anos nos disserem. Cabe agora tomar medidas baseadas em factos e que melhorem a qualidade de vida de todos os que vivem e trabalham em Lisboa.
Em breve iremos ainda ter mais dados dos CENSOS 2021 ao nível de BGRI, que permitiram desagregar ainda mais por tipo de habitação e alojamento.
Não devem ser excluídos ainda, outros futuros projectos de emprendimentos turísticos, como hotéis, já em construção, aprovados ou em fase de aprovação por parte do Turismo de Portugal e Câmara Municipal de Lisboa.


## Dados
Para a elaboração desta análise foram usados os seguintes dados:

##### Dados Alojamento Local e Empreendimentos Turísticos
Os dados com a informação geográfica de cada licença foram obtidos através da plataforma de dados abertos desenvolvida pelo Turismo de Portugal, [TravelBI](https://travelbi.turismodeportugal.pt/)

##### CENSOS 2021
Os dados ao nível de cada BGRI, foram obtidos através do site do [INE](http://mapas.ine.pt/download/index2021.phtml), que disponibilizou recentemente esta informação como dados provisórios. Assim que forem disponibilizados os dados definitivos, os mapas e rácios serão atualizados.

Toda a transformação, tratamento de dados, e criação de mapas foi feita e programada exclusivamente em python. Artigo e site feitos em markdown com recurso ao GitHub pages e Jekyll.
Última atualização dos dados a 26 de Abril de 2022.


