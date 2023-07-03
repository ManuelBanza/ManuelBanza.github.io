---
layout: post
title: Refúgios Climáticos - Identificação e Priorização em Lisboa
date: 2023-04-10 00:00:00 +0300
description: Quais os locais mais prioritários para mitigar as ondas de calor? # Add post description (optional)
img: Capa_Refugios.png # Add image post (optional)
tags: [refugiois-climaticos, calor, alteracoes-climaticas, python, lisboa, GIS] # add tag
---

**To directly translate this article to English with Google, please [click here](https://manuelbanza-github-io.translate.goog/refugios-climaticos-lisboa-priorizar/?_x_tr_sl=pt&_x_tr_tl=en&_x_tr_hl=en&_x_tr_pto=wapp)**

# Nota Inicial
No passado dia 11 de Julho de 2022, o partido LIVRE apresentou uma [proposta de recomendação na Assembleia Municipal de Lisboa](https://www.am-lisboa.pt/documentos/1657546422W9xBS2fd2Hh92QY7.pdf), que propunha entre outras coisas, a criação de uma rede de refúgios climáticos na cidade de Lisboa, de forma a mitigar os efeitos causados por ondas de calor. A proposta foi aprovada.

Este artigo é uma tentativa de analisar os factores que se devem ter em conta na criação de refúgios climáticos, e foca-se nos locais que mais difícilmente seriam hoje em dia adaptados para esse efeito, tornando a sua prioridade ainda maior.
A vontade para este artigo surge também pelo exemplo de Barcelona, que liderou o processo de criação de uma rede de refúgios climáticos em escolas, pátios e bibliotecas de forma a baixar a temperatura sentida na cidade. Um exemplo de sucesso que nos deve servir de inspiração para as nossas cidades.

# Introdução
Como resultado das alterações climáticas, a cidade tem sofrido com ondas de calor mais frequentes e intensas, mas também precipitações mais irregulares. Além disso, o aumento do nível do mar pode ameaçar algumas áreas da cidade, especialmente aquelas situadas em áreas baixas ou próximas da costa. Com os efeitos das alterações climáticas a serem cada vez mais visíveis na cidade, e as ondas de calor cada vez mais frequentes durante o ano, é necessário que a cidade encontre medidas de mitigação para o calor que cada vez será mais sentido na cidade.

Uma das medidas identificadas no relatório Focused Adaptation, de 2021, realizado para a rede C40, é a criação de “cooling centers” (cuja tradução literal será “centros de arrefecimento”), locais onde as pessoas se podem refugiar durante ondas de calor, em zonas com vegetação ou locais fechados com de ar condicionado.
Os refúgios climáticos são áreas ou espaços urbanos que proporcionam proteção e conforto para as pessoas em condições climáticas adversas, como o calor extremo. 
Os refúgios climáticos podem ser criados de várias maneiras, como por exemplo:
- Usando árvores, arbustos e outras plantas para criar sombra e refrescar o ar
- Instalando equipamentos de refrigeração, como ventiladores, sistemas de ar-condicionado
ou nebulizadores
- Aproveitamento da sombra natural e a brisa para refrigeração natural

Além de proporcionar conforto e segurança para as pessoas, os refúgios climáticos também podem ajudar a reduzir o consumo de energia, pois as pessoas podem se abrigar nesses espaços em vez de usar aparelhos de ar-condicionado em sua casa, optando por partilhar o recurso.

Desta forma torna-se cada vez mais pertinente criar uma rede de refúgios espalhados pela cidade de Lisboa, que ajude a mitigar as ondas de calor. Para isso é preciso identificar os locais que mais urgência têm na criação de um refúgio tendo em conta vários fatores.

Este artigo procura utilizar os resultados da análise numa perspectiva de ecologia social e urbana. Da transformação de espaços urbanos em comunidades mais sustentáveis promovendo a participação cidadã e o desenvolvimento de soluções que beneficiam tanto o meio ambiente quanto as pessoas que habitam nesse bairro.

# Refúgios climáticos como espaços de convívio
Os refúgios climáticos defendidos nesta análise, caracterizam-se por serem espaços de encontro e convívio. Quando as pessoas têm um lugar para se reunir e conviver, eles são mais propensos a serem usados e aproveitados. Esses espaços podem ter uma série de características que os tornam mais agradáveis e proporcionadores de interações para as pessoas, como bancos, espaços para realizar atividades ao ar livre, jogos, áreas sombreadas e outras instalações que tornam o local um bom lugar para passar o tempo. Além disso, os refúgios climáticos também podem ter elementos de lazer e entretenimento, como brinquedos para crianças.


<center><img src="{{site.baseurl}}/assets/img/01.Exemplos_Refugios.png" width="620" height="400"></center>
<center>Exemplos Refúgios Climáticos em Barcelona, Berlim e Milão</center>


Como podemos então priorizar e selecionar os locais que atualmente mais necessitam de um refúgio climático por não estarem rodeados de espaços verdes, bibliotecas ou outros fatores que possam ajudar a baixar a temperatura? É precisamente o que esta análise vai tentar responder.


# Fatores
Para conhecermos melhor a realidade de Lisboa, precisamos primeiro de mapear pela cidade os fatores que ajudam a entender melhor o efeito do calor, e o que pode ajudar a mitigá-lo. No mapa abaixo é possível visualizarmos o efeito da ilha de calor ao entardecer na cidade de Lisboa:

![Ilha de calor ao entardecer (variação em graus centigrados]({{site.baseurl}}/assets/img/02.ICU.png)
<center>Ilha de calor ao entardecer (variação em graus centigrados</center>


O efeito de ilha de calor é um fenómeno que ocorre em áreas urbanas e que consiste na acumulação de calor nessas mesmas áreas, e em comparação com as áreas rurais circundantes. Isso ocorre devido às diferenças na absorção e reflexão da radiação solar pelos materiais usados na construção das cidades. As áreas urbanas tendem a absorver mais calor do que as áreas rurais, o que leva a temperaturas mais altas nas cidades.
**O efeito de ilha de calor pode ser agravado por vários fatores, incluindo a falta de vegetação e a construção de edifícios e asfalto** que faz aumentar a quantidade de superfícies impermeáveis, o que pode aumentar a retenção de calor nessas zonas. O efeito de ilha de calor urbano (ICU) pode ter sérias consequências para a saúde humana, incluindo desidratação, desmaio e doenças respiratórias.

Como falado anteriormente, algumas das formas de mitigar este efeito e as ondas de calor extremo, é termos na cidade vários jardins, bibliotecas, zonas de refresco com bebedouro, fontes e lagos, que permitam fazer baixar a temperatura na cidade e ajudar o organismo do ser humano a manter-se hidratado em períodos com temperaturas elevadas.
Qual a localização destes pontos na cidade? Será que existe uma relação entre estes locais e as zonas de maior exposição e incidência solar?

Na figura abaixo visualizamos a distribuição espacial destes pontos de interesse:

<iframe src="https://manuelbanza.github.io/Artigos/Refugios_Climaticos/02.2.Refugios_Locais_ICU_Lisboa.html" height="700px" width="100%"></iframe>

Arraste o mapa e clique nos objetos para obter mais informação.
Para ver o mapa maior em versão mobile ou em ecrã completo clique [AQUI](https://manuelbanza.github.io/Artigos/Refugios_Climaticos/02.2.Refugios_Locais_ICU_Lisboa.html)



Como é possível ver na imagem abaixo, temos zonas como a Baixa de Lisboa junto ao rio, que apesar de ser das zonas com maior efeito de ilha de calor, não dispõe de muitos espaços verdes, nem sequer bebedouros que permitam as pessoas refrescarem-se. Esta zona e toda a zona ribeirinha é caracterizada precisamente por estas características, destacando-se assim logo como uma zona prioritária para intervenção.

# Situação Atual
Identificados alguns dos pontos de interesse e características que podem existir num refúgio climático, podemos então calcular quais são as zonas mais críticas da cidade que estão em situação desfavorecida no combate à mitigação dos efeitos de calor das alterações climáticas.

## Proximidade a Jardins e Parques
A primeira análise que podemos recorrer é de calcularmos a distância que certas zonas da cidade estão a pé de pelo menos um jardim. Isto permite identificar que zonas têm pelo menos um jardim a 5, 10 ou mais de 10 minutos.
Para este cálculo foi usada toda a rede pedonal existente na cidade de Lisboa, que foi obtida através da plataforma comunitária OpenStreetMap.
Com esta informação extraímos todos os nós da rede viária e pedonal, que acabam por ser todas as interceções entre pelo menos duas ruas, e calculámos para cada nó o tempo que demoraria a chegar ao jardim ou parque mais próximo. Para esse cálculo, foi considerado como velocidade média os 4km/hora para andar a pé, visto que é o valor mais recorrente em outros estudos identificados.

Após este processo e para facilitar a leitura, todos os nós (interceções) foram agregados em células hexagonais com um raio de 150 metros cada uma. Nessa agregação é feita a média de todos os nós dentro de cada hexágono, e por sua vez é identificado se esse hexágono está a uma distância de um jardim ou parque até 5 minutos a pé, até 10 minutos ou mais de 10 minutos.

![Proximidade a Parques e Jardins]({{site.baseurl}}/assets/img/04.Proximidade_Jardins.png)
<center>Proximidade a Parques e Jardins</center>


Nota: Os hexágonos amarelos indicam que essa zona está em média até 5 minutos a pé, o laranja 10 minutos e o roxo a mais de 10 minutos.

Na imagem acima podemos verificar algumas zonas que estão com a cor roxa, que significa que estão a mais de 10 minutos a pé de pelo menos um jardim ou parque, podendo ser valores piores caso estejamos a falar de uma população mais envelhecida e que acaba por demorar mais a fazer este percurso do que a média da população. Algumas dessas zonas estão na zona norte e sudeste de Lisboa.
No entanto, quando adicionamos a variável de densidade populacional (imagem abaixo) verificamos que a zona norte não é tanto um problema, nem prioritário para haver um refúgio climático, isto porque nesta zona situa-se o aeroporto de Lisboa, não havendo população que resida neste local. Já a zona sudeste ganha maior urgência por ser uma das zonas com maior densidade populacional.

![Proximidade a Parques e Jardins com Densidade Populacional]({{site.baseurl}}/assets/img/05.Proximidade_Jrdins_Pop.png)
<center>Proximidade a Parques e Jardins com Densidade Populacional</center>


Nota: Quanto maior for a altura do hexágono, maior a densidade populacional desse mesmo
hexágono. Zonas com altura elevada e com cor roxa, são zonas com bastante densidade
populacional e que se encontram a mais de 10 minutos a pé de um jardim ou parque.

## Arvoredo
Outro fator importante de analisarmos é também as árvores que estão espalhadas
pela cidade e não apenas os parques e jardins, já que estas têm um papel fundamental para conseguir baixar a temperatura sentida na cidade, como podemos ver na animação abaixo.

<center><img src="{{site.baseurl}}/assets/img/video_arvores_calor.gif" width="600" height="400"></center>

<center>Fonte: Wimberly Allison Tong & Goo</center>

Dessa forma contabilizou-se a distribuição de árvores na cidade.

![Árvores na cidade de Lisboa]({{site.baseurl}}/assets/img/07.Arvores.png)
<center>Árvores na cidade de Lisboa</center>


## Proximidade Bibliotecas
À semelhança do que foi feito para os parques e jardins, também se considerou importante contabilizar as zonas da cidade onde existe bibliotecas até 10 minutos a pé. Estas bibliotecas municipais podem ser refúgios para ondas de calor intensas, dispondo de ar condicionado e espaços protegidos para as horas de mais calor. São ainda importantes em situações de frio e chuvas intensas que cada vez mais acontecerão, e com maior frequência, na cidade de Lisboa.

![Proximidade a bibliotecas municipais]({{site.baseurl}}/assets/img/06.Proximidade_Bibliotecas.png)
<center>Proximidade a bibliotecas municipais</center>


# Seleção de locais
Neste trabalho é proposto uma análise multicritério que usa precisamente a proximidade aos fatores referidos anteriormente para criar uma escala de pontuação (score) que permite identificar os locais onde é mais urgente criar um refúgio climático. Permitindo assim usar os dados para a tomada de decisão, mais concretamente no planeamento urbanístico da cidade de Lisboa.
Para isso é proposto usar 5 fatores com pesos diferentes de importância:

1. Ilha de Calor: Valores do IUC ao entardecer (30%)
2. Proximidade a Jardins e Parques: Distância a pé do jardim ou parque mais próximo (25%)
3. Nº Residentes: População residente em cada BGRI (quarteirão) segundo os CENSOS de 2021
4. Arvoredo: Concentração de nº árvores nas proximidades (15%)
5. Proximidade Bibliotecas: Distância a pé da biblioteca municipal mais próxima (10%)


<center><img src="{{site.baseurl}}/assets/img/08.Score_calculo.png" width="500" height="400"></center>
<center>Score de identificação de zonas prioritárias</center>



Este cálculo foi feito a cada hexágono (H3) que tem aproximadamente cerca de 105 mil m2 (Para mais detalhe consultar a metodologia no fim do artigo). 

Nota: Foram aplicadas normalizações aos dados de cada variável de forma a ser possível criar a escala de pontuação proposta aqui. As variáveis foram normalizadas através do método estatístico MinMaxScaler que permite normalizar os valores das varáveis, criando uma escala entre 0 e 1.

# Resultados
No mapa abaixo é possível verificar quais os locais da cidade, que mais necessidade têm de ter um refúgio climático de forma a combater a mitigar as ondas de calor cada vez mais sentidas na cidade de Lisboa. Para proporcionar o efeito do priorização, apenas foram selecionadas as zonas que têm um score dentro do 3º quartil, ou seja os casos com score mais alto.

<iframe src="https://manuelbanza.github.io/Artigos/Refugios_Climaticos/07.Score_Refugios_H3_Total_clean_read_only.html" height="700px" width="100%"></iframe>

Arraste o mapa e clique nos objetos para obter mais informação.
Para ver o mapa maior em versão mobile ou em ecrã completo clique [AQUI](https://manuelbanza.github.io/Artigos/Refugios_Climaticos/07.Score_Refugios_H3_Total_clean_read_only.html)

Na imagem  abaixo são identificados 6 zonas que iremos explorar com mais atenção. 

![Score com locais com maior necessidade para criar um refúgio climático]({{site.baseurl}}/assets/img/H3_Score_Noted.png)
<center>Score com locais com maior necessidade para criar um refúgio climático</center>


## Baixa (1)

A Baixa de Lisboa, situada perto do rio, é uma das zonas mais turísticas e históricas da cidade. Mesmo estando perto do mar, continua a ser uma das zonas em que se sente mais o efeito de ilha de calor e de falta de árvores que possibilitem a mitigação desse mesmo calor. À semelhança de outras zonas da cidade, é também uma zona com poucos jardins e parques por perto. É, no entanto, uma zona que têm vindo a decrescer no número de residentes, mas onde se situam muitos hotéis e alojamentos.

<center><img src="{{site.baseurl}}/assets/img/Cais.png" width="400" height="400"></center>
<center>Baixa</center>



## Alto São João – Morais Soares (2)
A separação entre a freguesia de Arroios e Penha de França feita pela Rua Morais Soares é o quilometro quadro com mais população de Portugal. É uma zona com vários residentes e no entanto é das zonas da cidade com menos árvores e sem qualquer jardim ou parque de média dimensão que possibilite mitigar as ondas de calor.
É também uma zona muito afetada pelo efeito de ilha de calor, principalmente com as zonas à sua volta.
**Esta situação é aliás sentida em grande parte de Arroios, e muito agravada pela escassez de espaços verdes e àrvores na freguesia.**

<center><img src="{{site.baseurl}}/assets/img/Alto_sao_Joao.png" width="400" height="400"></center>
<center>Alto São João – Morais Soares</center>

## Chelas (3)
Uma das zonas com maior densidade populacional de Lisboa, é também uma das zonas mais historicamente esquecidas da cidade. A necessidade de alojar pessoas vindas de habitações precárias, bem como as políticas de realojamento que se basearam em bairros de habitação social com construções deficitárias do ponto de vista arquitetónico e urbanístico, marcaram para sempre o destino desta zona. A carência de jardins, parques e espaços de convívio, tornam indispensável a criação de refúgios climáticos para a população local.

<center><img src="{{site.baseurl}}/assets/img/Chelas.png" width="400" height="400"></center>
<center>Chelas</center>



## Bairro do Rego (4)
Á semelhança de Chelas, o bairro do Rego é também uma zona com elevada densidade populacional e situada numa zona central de Lisboa. Sendo um bairro residencial, era esperado que houvesse mais jardins, bibliotecas e outros espaços que permitissem mitigar o efeito de ilha de calor. No entanto tal não se verifica.

<center><img src="{{site.baseurl}}/assets/img/Rego.png" width="400" height="400"></center>
<center>Rego</center>


## Parque das Nações (5)
Apesar de esta zona ter vários jardins e bastantes árvores, comparada com outras zonas da cidade, é das zonas que mais sofre o efeito de ilha de calor.
Segundo uma reportagem do jornal “o Público”, esta razão deve-se ao facto de a nova construção feita nesta zona da cidade, na altura da Expo'98, não teve em consideração o impacto ambiental que esses prédios tinham na circulação de ar entre os prédios.
Tratando-se de prédios altos, dificultam ainda mais a circulação de ar. Caminhando entre os prédios do Parque das Nações, as brisas do rio Tejo deixam mesmo de ali chegar. Essa diferença de poucos metros regista aumentos de 2º C.
A acrescentar ao problema atual, é sabido que as alterações climáticas irão ser sentidas de maior forma nesta parte de Lisboa no que toca a ondas de maior calor. Algo que apenas reforça a necessidade de serem criados refúgios e outras medidas.

<center><img src="{{site.baseurl}}/assets/img/Parque_Nacoes.png" width="400" height="400"></center>
<center>Parque das Nações</center>



## Ajuda (6)
Zona residencial com bastante densidade populacional. Apesar de em média se situar a menos de 10 minutos do jardim mais próximo, acaba por por ser bastante afectada pelo efeito de ilha de calor.

<center><img src="{{site.baseurl}}/assets/img/Ajuda.png" width="400" height="400"></center>
<center>Ajuda</center>




# Pesquisa Etnográfica e Cocriação
Os refúgios climáticos só terão um impacto positivo de forma duradoura se forem criados de forma colaborativa e com a participação ativa das comunidades locais.

Um processo de cocriação e pesquisa etnográfica pode ser uma forma eficaz de ouvir as necessidades e desejos das pessoas que residem, trabalham, estudam ou passam pelos locais onde se deseja criar refúgios climáticos. Esse processo deve ser bottom-up, ou seja, deve partir da base, das necessidades e interesses das pessoas, e não impor soluções prontas de cima para baixo. 
É fundamental que esse processo de cocriação também inclua um senso de propriedade compartilhada pelos moradores e utilizadores do local, para que a comunidade tenha um sentimento de pertença e compromisso com o espaço, fomentando sempre que possível a autonomia da população.

**É importante não tentar construir um futuro sobre o que é novo e aparentemente inovador, mas investigar o que já lá está e transformar o que existe numa força de mudança para melhorar o bairro. A grande maioria dos bairros do futuro nas grandes cidade europeias não serão construídas em terrenos verdes, serão adaptados ao tecido social e físico existente.**

Os refúgios podem também ser uma construção colectiva de esperança. A de um imaginário colectivo emancipatório que nos permitirá reclamar o espaço público, criando momentos de proximidade ao mesmo tempo que mitigam as alterações climáticas. 

Ao considerar as necessidades e desejos das comunidades locais, é mais provável que os refúgios climáticos sejam criados de forma mais eficaz e duradoura. Além disso, a participação ativa das comunidades no processo de cocriação pode promover a responsabilização e o envolvimento das pessoas, o que pode aumentar a probabilidade de sucesso a longo prazo dos refúgios climáticos. Vejamos por exemplo [casos como o projeto Sê Bairrista em Marvila](https://amensagem.pt/2023/03/29/vizinhos-bairros-chelas-fizeram-dos-bairros-sitios-mais-bonitos-festival/), que com a ajuda da [Rés do Chão](https://resdochao.org/), associação especializada em arquitectura participada, se conseguiu criar com a população soluções pensadas pela comunidade.

No entanto o mais importante é começar. Mesmo que seja algo pequeno que possa mais tarde evoluir já com aprendizagens obtidas no processo. Como refere o Brian Eno **"Think like a gardener, not an architect: design beginnings, not endings".**


<center><img src="{{site.baseurl}}/assets/img/09.processo_etnografico.png" width="400" height="400"></center>

<center>Processo de Participação (Fonte: EX Collective)</center>

# Conclusões
Este artigo abordou a importância dos refúgios climáticos como uma estratégia de
mitigação das alterações climáticas e como um mobilizador de comunidades e de espaços públicos para o convívio, protegendo as comunidades mais vulneráveis e promovendo a convivência social.

Para identificar os locais mais prioritários para a criação de refúgios climáticos, foi utilizada a ciência de dados, que permitiu avaliar os riscos climáticos e as necessidades das comunidades de forma objetiva e baseada em evidências. A ciência de dados é uma ferramenta fundamental para a tomada de decisão e a priorização de ações, e foi mostrado que é crucial para maximizar o impacto e a eficácia dos refúgios climáticos.

No ínicio do ano ficámos também a saber pelo site [Lisboa Para Pessoas]((https://lisboaparapessoas.pt/2023/01/19/perguntas-a-camara-assembleia-municipal-lisboa/#h-livre-como-esta-o-projecto-dos-refugios-climaticos)) que os departamentos técnicos da Câmara Municipal de Lisboa já estão a trabalhar em formas de mitigar o efeito da ilha de calor através do programa **"Arrefecer a Cidade"**. Sendo um dos locais de intervenção precisamente a zona à volta da Rua Morais Soares, como aqui foi referido.

É importante destacar que os refúgios climáticos não são a única solução para as alterações climáticas, mas são uma peça importante. É necessário continuar a trabalhar em outras medidas de mitigação e adaptação

No entanto, os refúgios climáticos podem ser um poderoso catalisador para mudanças positivas, ao mobilizar as comunidades e os espaços públicos para o convívio e a reflexão sobre as questões climáticas. É fundamental que continuemos a investir em iniciativas como estas, para garantir um futuro mais sustentável e seguro para todos.

A criação destes locais passa também inevitavelmente pela redução do espaço dado ao automóvel (seja de algum estacionamento ou impedimento de circulação em certas ruas) até por não termos atualmente jardins e parques suficientes na cidade. **É importante identificar esta situação como uma questão de saúde pública e não como um assunto partidário**. Se queremos combater as ondas de calor intensas e melhorar a qualidade de vida das pessoas, precisamos de tomar medidas que poderão não ser as mais populares, no entanto, serão elas que farão das nossas cidades espaços de proximidade, bem estar e sustentáveis.

## Próximos passos
Numa futura revisão da análise, seria interessante obter dados da sombra ao longo do dia, de forma a verificar zonas específicas que estão mais expostas ao sol. Além disso seria interessante conseguir averiguar essa sombra por cada jardim, visto que podem existir casos que a existência de um jardim pode não ajudar a mitigar o calor sentido, seja por falta de àrvores, seja pelo espaço não ser convidativo ou pelo mobiliário urbano em si. Um destes casos é o jardim da Alameda entre as freguesias de Arroios e Areeiro.

Esta análise identificou os casos com maior necessidade com base nos atributos selecionados, no entanto, no futuro seria interessante analisar os espaços que hoje são jardins mas ainda não têm as condições de serem considerados um refúgio. Dessa forma, seria interessante criar um conjunto de regras que fazem de um espaço um possível refúgio, bem como o que falta implementar em certos locais para passarem a ser um.

# Metodologia
Os dados foram obtidos através das plataformas de dados abertos da cidade de Lisboa (Geodados, LXI), colecta manual nos casos das bibliotecas e piscinas municipais e ainda através de dados gerados pela comunidade online, como é o caso dos jardins e parques de Lisboa, dataset criado pelo Miguel Monteiro ao qual agradeço a criação e disponibilização.
Esta análise apenas é possível graças à aposta da Câmara Municipal de Lisboa nos dados abertos e que espero que venha ainda a aumentar, bem como os projectos comunitários que cada vez mais ganham terreno.

A unidade de análise geográfica utilizada para este projecto foi o H3 com a resolução 9. O sistema H3 (Hexagonal Hierarchical Spatial Index) é uma das melhores formas de tratar dados geoespaciais devido à sua capacidade de dividir o espaço em hexágonos de forma hierárquica, permitindo uma rápida agregação e filtragem de dados.
Uma das vantagens de uniformizar todos os dados no sistema H3 é a facilidade de comparação e análise de dados geoespaciais de diferentes fontes, pois todos os dados estarão no mesmo formato e com a mesma granularidade. 
Para chegar a essa unidade geográfica isso foram realizadas interpolações espaciais tanto para os dados dos CENSOS (BGRIs) como da ilha de calor.


# Comunicação Social

Este artigo foi reproduzido nos seguintes orgãos de comunicação social:


 [![Mensagem de Lisboa](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAOEAAADhCAMAAAAJbSJIAAAA51BMVEUAAAD///8AhbL5+fn8/Pxzc3Opqane3t4EBASurq4oKCji4uJZWVkABgAJAAMAAQMVNUcagqYHGS7z8/MJAAXQ0NAYfaCQkJBqamrp6ekfHx8agJ5kZGRLS0vW1taYmJhDQ0O2trZPT0+ioqJ7e3sAAA4Ah68Cg7MPDw/BwcEzMzO9vb2Hh4cXFxccHBw6OjowMDAbIig7cIoROEITOVAWTWUYWHkAECQiZIMKGigcRlMIgLMFgrwfcIwQKDwAibIeZXsADRcRNz0feqUWeZAneZkSU2UcYnAogI03Z3cAHiUPERgUAA99CufUAAAHDElEQVR4nO2dC3uaOhiAA4k1okA7tN5tbVW0det2tm7rXOd67M79//+ekwDegaALpOP53ufZOquR7+XLHXQIAQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAALnjpFYadF4HDyilSoNJgzGqaZpGcO223umqDiYVWM6KhGg+uDkpFbrG+jmaj6QazZWiB2n2TuqVpWcODCm6wZt+JPB1ipOLwY3q6KRA0aW2nUXPNPjZUB2eHBranuHSs6U6NklMoxQ11ZFJgqKLCMWi6tAkwTrMkobDDGuqQ5MEH/UmoTm8UB2aNPjIrzn7NXWgOjBp8CyW98cMLT8zOT49M5q57UqXXDq73U1TdUhSYVms7I4ZE9VBSYVX1AbensCdqA5KNhQNNLw2JKwrzcHaYhOWxet1RWX/qOTQEPW15cKCEOf1/ks2nMdvjFbr9cYTgtOxXk6zkkZr/80zYrJqisTZezJY9RvTk17Z8V/llHv9+l3wZPTbBv6der9X3Cx56ZdMQSQyENRbdTb7s1IeSaMfDJz8dWzB7I0weFJAoh2Bq+viuhNbHYTUpumoRMBjbPrrfKKVNp+g3pm+LGG/jZJ1mEGs+LqFQiSpn9u7a2fVvFdtffnztovElVwiLScIffPkemF2J5ELSa/aXYcZ8oKV8In9Op+1boZ7QmN0hf0xo7IVKTJuWZWMMWSBNit7b8dPTI1oOHR1FpTjNb20VzI1WEgdNiwybjZ/h6bRMQaR8r920rjsnhPAzs44u4pa0Fi21l0pHSNUi62ga8nbzfdhBRshi7LQokSrZ1dRKZqySfjmFkbXia2gm3Fu98AlLVlBVo1xljUVscnN6nisphUSpSFgskwFRa1iksyvTg87ZIZD4+1qC4NNVxPmIYhzNWG/c0K2YmPArBlnZchOZbGzfNCI70N3DYkWlOyyBecBBb0N90JGgpyW4dUYirqH1DQeKHa84fsSE1H3u4eD32Y52/cFDRwzloUran1+PSRh57RdFPckN8W4uTL11ws9cqAhr2xdNOZt8GBD1hTrMv1EV32pt2I8hgnqHZr5Jc5YqqHwFYc2Qh+CJ5rjHGfIp0USKcdTnJSPMyTkmCrqgbHUSfhxQaQJwXJnb4KjHZuHnwGTsswkZi8ghmhX0vxepqHctaJql3DKuTfU3ubeUOL2m2qVUPi8NmtDvDluHLSW8l5NQh/EILEhJjbUSK9fLzQa036ZHLSs5ecG106mjUbhYtIkyRZUTvbjYXmwng8b14fN5Gqd9fGu4ndcfdg5uczUEGNn544Fo6clq6jEIcWdewEqjtiRaPv7rmkakmJre1VK+d5iwrVRf28GZjQTGMq7CSRJkEW+77m7zVtOVlFPdi4s8RXnnfDkEIkrKGGImLAVaUi7D7uhca8s3zsNuVQzFZeVN29LYNgIE6SoLw4TO2/CNl0oagqbYoaGXhrCokySxHpoUYrqCQxljRdiw8heTdgSSeSoZghbYknaElEo2Iw8UkmYiH5k2fILMjyJPNJAaNiJKJnggluGhtE3eldERXH0LdTCLcqsDFmSjMgj3YhS2IyOcvBSDDWCo49D47sLovWio+yIanh2OYxbxogMY8Y0YQ3Prh3+jGHMfX8vyDDuZn3RoAaGYAiGYAiGYAiGYAiGYAiGYAiGYAiGYAiGYAiGYJi+YfRlq1/EcHxjxPPmFzdM8HkDaR9JUGVIqW3bliXJIg4Fhr4ZN7SHqThto8JwaFnv3rF2Ztl2Kk7bqMkhOv3tPTItK4tPOCkwRCx5Hxbn98NsPmuoxBChD2fu4uMnZFWRSVOuq0oMbXR65rr65weratE8G549niKLNcZ066oyQ13XXX3xZVjNr+F8rs9m5x8/DVPubpQZjhju7Ovs80MKVpuoy6HHV3f0+M027Wp68zfFhro+b7P+hgmaaVVWxYZz9qfdvh+m2KOqzqE7m+mjs+9PVmr1VLGhy2GKj99ScPNRncP5aM7y6OrPvyOb8mdyZ+gzGp0t7m2TsnlqLg15PdUX7e+svzFzashqqc4b4yvb4iv/HBpyQX3mnj2fVvNpuOpWRz++oFwZ+rnj/cwoGBoX7ftPNv+CN4mjowpD2zN0edZ2kui6i89PfK+xWpWWSXWG4czPH7/xzUbTpJIcX5ohS+OP92wmTk1ZFfWlGc5m7qj9x5ANjTkxdPdgg7+r//kk78KFyDDu0wiisjG7ie+f2x7nu3i/bP/194O0QaMQTyPm/7egDUHhiM/1URNZT6/iePjn3b+yrq79xNscX9Q0Teu/2FZmse7UlDNHVfFFyJbNFKkZB7Wr1WEWl21SwuJ6VpVjhWJzxV/YkLJlYJXPPxl0Fz+FVrZfngwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACCH/wFXCJLPchqmJQAAAABJRU5ErkJggg==)](https://amensagem.pt/2023/04/29/refugios-climaticos-calor-em-lisboa/) &emsp;
  [![Lisboa por Pessoas](data:image/png;base64,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)](https://lisboaparapessoas.pt/2023/06/20/manuel-banza-refugios-climaticos-lisboa/) &emsp; 
