---
layout: post
title: Refúgios Climáticos - Identificação e Priorização em Lisboa
date: 2023-01-01 00:00:00 +0300
description: Quais os locais mais prioritários para mitigar as ondas de calor? # Add post description (optional)
img: Capa_Refugios.png # Add image post (optional)
tags: [refugiois-climaticos, calor, alteracoes-climaticas, python, lisboa, GIS] # add tag
---

# Nota Inicial
No passado dia 11 de Julho de 2022, o partido LIVRE apresentou uma [proposta de recomendação na Assembleia Municipal de Lisboa](https://www.am-lisboa.pt/documentos/1657546422W9xBS2fd2Hh92QY7.pdf), que propunha entre outras coisas, a criação de uma rede de refúgios climáticos na cidade de Lisboa, de forma a mitigar os efeitos causados por ondas de calor. A proposta foi aprovada.

Este artigo serve como tentativa de analisar os factores que se devem ter em conta na criação de refúgios climáticos, e foca-se nos locais que mais difícilmente seriam hoje em dia adaptados para esse efeito, tornando a sua prioridade ainda maior.

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

# Refúgios climáticos como espaços de convívio
Os refúgios climáticos defendidos nesta análise, caracterizam-se por serem espaços de encontro e convívio. Quando as pessoas têm um lugar para se reunir e conviver, eles são mais propensos a serem usados e aproveitados. Esses espaços podem ter uma série de características que os tornam mais agradáveis e proporcionadores de interações para as pessoas, como bancos, espaços para realizar atividades ao ar livre, jogos, áreas sombreadas e outras instalações que tornam o local um bom lugar para passar o tempo. Além disso, os refúgios climáticos também podem ter elementos de lazer e entretenimento, como brinquedos para crianças.


<center><img src="{{site.baseurl}}/assets/img/01.Exemplos_Refugios.png" width="620" height="400"></center>
<center>Exemplos Refúgios Climáticos em Barcelona, Berlim e Milão</center>


Como podemos então priorizar e selecionar os locais que atualmente mais necessitam de um refúgio climático por não estarem rodeados de espaços verdes, bibliotecas ou outros fatores que possam ajudar a baixar a temperatura? É precisamente o que esta análise vai tentar responder.


# Fatores
Para conhecermos melhor a realidade de Lisboa, precisamos primeiro de mapear pela cidade os fatores que ajudam a entender melhor o efeito do calor, e o que pode ajudar a mitigá-lo. No mapa abaixo é possível visualizarmos o efeito da ilha de calor ao entardecer na cidade de Lisboa:

![Ilha de calor ao entardecer (variação em graus centigrados]({{site.baseurl}}/assets/img/02.ICU.png)
<center>Ilha de calor ao entardecer (variação em graus centigrados</center>


O efeito de ilha de calor é um fenômeno que ocorre em áreas urbanas e que consiste na acumulação de calor nessas mesmas áreas, e em comparação com as áreas rurais circundantes. Isso ocorre devido às diferenças na absorção e reflexão da radiação solar pelos materiais usados na construção das cidades. As áreas urbanas tendem a absorver mais calor do que as áreas rurais, o que leva a temperaturas mais altas nas cidades.
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
pela cidade e não apenas os parques e jardins. Dessa forma contabilizou-se a distribuição de árvores na cidade.

![Árvores na cidade de Lisboa]({{site.baseurl}}/assets/img/07.Arvores.png)
<center>Árvores na cidade de Lisboa</center>


## Proximidade Bibliotecas
À semelhança do que foi feito para os parques e jardins, também se considerou importante contabilizar as zonas da cidade onde existe bibliotecas até 10 minutos a pé. Estas bibliotecas municipais podem ser refúgios para ondas de calor intensa, dispondo de ar condicionado e espaços protegidos para as horas de mais calor. São ainda importantes em situações de frio e chuvas intensas que cada vez mais acontecerão, e com maior frequência, na cidade de Lisboa.

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

A Baixa de Lisboa, situada perto do rio, é uma das zonas mais turísticas e históricas da cidade. Mesmo estando perto do mar, continua a ser uma das zonas em que se sente mais o efeito de ilha de calor e de falta de arvores que possibilitem a mitigação desse mesmo calor. À semelhança de outras zonas da cidade, é também uma zona com poucos jardins e parques por perto. É, no entanto, uma zona que têm vindo a decrescer no número de residentes, mas onde se situam muitos hotéis e alojamentos. Sendo que esses fatores não foram contabilizados na análise, acredita- se que se fossem o impacto e score nesta zona da

<center><img src="{{site.baseurl}}/assets/img/Cais.png" width="400" height="400"></center>
<center>Baixa</center>



## Alto São João – Morais Soares (2)
A separação entre a freguesia de Arroios e Penha de França feita pela Rua Morais Soares é o quilometro quadro com mais população de Portugal. É uma zona com vários residentes e no entanto é das zonas da cidade com menos árvores e sem qualquer jardim ou parque de média dimensão que possibilite mitigar as ondas de calor.
É também uma zona muito afetada pelo efeito de ilha de calor, principalmente com as zonas à sua volta.

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
Segundo uma reportagem do jornal “o Público”, esta razão deve-se ao facto de a nova construção feita nesta zona da cidade, na altura da EXPO 90, não teve em consideração o impacto ambiental que esses prédios tinham na circulação de ar entre os prédios.
Tratando-se de prédios altos, dificultam ainda mais a circulação de ar. Caminhando entre os prédios do Parque das Nações, as brisas do rio Tejo deixam mesmo de ali chegar. Essa diferença de poucos metros regista aumentos de 2º C.
A acrescentar ao problema atual, é sabido que as alterações climáticas irão ser sentidas de maior forma nesta parte de Lisboa no que toca a ondas de maior calor. Algo que apenas reforça a necessidade de serem criados refúgios e outras medidas.

<center><img src="{{site.baseurl}}/assets/img/Parque_Nacoes.png" width="400" height="400"></center>
<center>Parque das Nações</center>



## Ajuda (6)
Zona residêncial com bastante densidade populacional. Apesar de em média se situar a menos de 10 minutos do jaridm mais próximo, acaba por por ser bastante afectada pelo efeito de ilha de calor.

<center><img src="{{site.baseurl}}/assets/img/Ajuda.png" width="400" height="400"></center>
<center>Ajuda</center>




# Pesquisa Etnográfica e Cocriação
A criação de refúgios climáticos pode ser uma estratégia eficaz para mitigar as alterações climáticas, protegendo as comunidades mais vulneráveis e promovendo a convivência social. No entanto, é importante lembrar que os refúgios climáticos só terão um impacto positivo de forma duradoura se forem criados de forma colaborativa e com a participação ativa das comunidades locais.

Um processo de cocriação e pesquisa etnográfica pode ser uma forma eficaz de ouvir as necessidades e desejos das pessoas que residem, trabalham, estudam ou passam pelos locais onde se deseja criar refúgios climáticos. Esse processo deve ser bottom-up, ou seja, deve partir da base, das necessidades e interesses das pessoas, e não impor soluções prontas de cima para baixo.

A pesquisa etnográfica pode ser uma ferramenta valiosa nesse processo, pois permite a compreensão profunda das necessidades, hábitos e contextos das comunidades locais. Isso pode incluir entrevistas, grupos de discussão, observação participante e outras técnicas de coleta de dados que permitem aprofundar a compreensão das perspetivas e experiências das pessoas.

Ao considerar as necessidades e desejos das comunidades locais, é mais provável que os refúgios climáticos sejam criados de forma mais eficaz e duradoura. Além disso, a participação ativa das comunidades no processo de cocriação pode promover a responsabilização e o envolvimento das pessoas, o que pode aumentar a probabilidade de sucesso a longo prazo dos refúgios climáticos.


<center><img src="{{site.baseurl}}/assets/img/09.processo_etnografico.png" width="400" height="400"></center>

<center>Processo de Participação (Fonte: EX Collective)</center>

# Conclusões
Este artigo abordou a importância dos refúgios climáticos como uma estratégia de
mitigação das alterações climáticas e como um mobilizador de comunidades e de espaços públicos para o convívio, protegendo as comunidades mais vulneráveis e promovendo a convivência social.

Para identificar os locais mais prioritários para a criação de refúgios climáticos, foi utilizada a ciência de dados, que permitiu avaliar os riscos climáticos e as necessidades das comunidades de forma objetiva e baseada em evidências. A ciência de dados é uma ferramenta fundamental para a tomada de decisão e a priorização de ações, e foi mostrado que é crucial para maximizar o impacto e a eficácia dos refúgios climáticos.

No ínicio do ano ficaḿos também a saber pelo site [Lisboa Para Pessoas]((https://lisboaparapessoas.pt/2023/01/19/perguntas-a-camara-assembleia-municipal-lisboa/#h-livre-como-esta-o-projecto-dos-refugios-climaticos)) que os departamentos técnicos da Câmara Municipal de Lisboa já estão a trabalhar em formas de mitigar o efeito da ilha de calor através do programa **"Arrefecer a Cidade"**. Sendo um dos locais de intervenção precisamente a zona à volta da Rua Morais Soares, como aqui foi referido.

É importante destacar que os refúgios climáticos não são a única solução para as alterações climáticas, mas são uma peça importante. É necessário continuar trabalhando em outras medidas de mitigação e adaptação, incluindo a redução das emissões de gases de efeito estufa, a conservação e restauração de ecossistemas e a promoção de práticas sustentáveis.

No entanto, os refúgios climáticos podem ser um poderoso catalisador para mudanças positivas, ao mobilizar as comunidades e os espaços públicos para o convívio e a reflexão sobre as questões climáticas. É fundamental que continuemos a investir em iniciativas como essas, para garantir um futuro mais sustentável e seguro para todos.

## Próximos passos
Numa futura revisão da análise, seria interessante obter dados da sombra ao longo do dia, de forma a verificar zonas específicas que estão mais expostas ao sol. Além disso seria interessante conseguir averiguar essa sombra por cada jardim, visto que podem existir casos que a existência de um jardim pode não ajudar a mitigar o calor sentido, seja por falta de àrvores, seja pelo espaço não ser convidativo ou pelo mobiliário urbano em si. Um destes casos é o jardim da Alameda entre as freguesias de Arroios e Areeiro.

# Metodologia
Os dados foram obtidos através das plataformas de dados abertos da cidade de Lisboa (Geodados, LXI), colecta manual nos casos das bibliotecas e piscinas municipais e ainda através de dados gerados pela comunidade online, como é o caso dos jardins e parques de Lisboa, dataset criado pelo Miguel a ao qual agradeço a criaçao e disponibilização.
Esta análise apenas é possível graças à aposta da Câmara Municipal de Lisboa nos dados abertos e que espero que venha ainda a aumentar, bem como os projectos comunitários que cada vez mais ganham terreno.

A unidade de análise geográfica utilizada para este projecto foi o H3 com a resolução 9. O sistema H3 (Hexagonal Hierarchical Spatial Index) é uma das melhores formas de tratar dados geoespaciais devido à sua capacidade de dividir o espaço em hexágonos de forma hierárquica, permitindo uma rápida agregação e filtragem de dados.
Uma das vantagens de uniformizar todos os dados no sistema H3 é a facilidade de comparação e análise de dados geoespaciais de diferentes fontes, pois todos os dados estarão no mesmo formato e com a mesma granularidade. 
Para chegar a essa unidade geográfica isso foram realizadas interpolações espaciais tanto para os dados dos CENSOS (BGRIs) como da ilha de calor.