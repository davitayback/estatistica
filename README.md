
# Resumo de Estatística para Ciência de Dados

Bem-vind@s ao meu resumo de Estatística para Ciência de Dados, com base no Curso de Data Science e Analytics da USP/Esalq com os méritos dos meus Professores Wilson Tarantin e Fávero, que estão entre os maiores Cientistas de Dados do Mundo.

A estatística é fundamental para Ciência de Dados e envolve coleta, organização, análise e interpretação dos mesmos. Ela desempenha um papel crucial na Ciência de Dados, ajudando-nos a tirar conclusões e tomar decisões informadas com base em informações numéricas. Posto isso coloco esse script do meu resumo do Curso Introdutório a Estatística da USP/Esalq.

## 1) Tipos de Variáveis:
As variáveis podem ser qualitativas (categóricas) ou quantitativas (numéricas).

### Qualitativas: 
São variáveis não métricas, atribuem categorias ou classificações de dados 
como gênero, estado civil e escolaridade *(Podem atribuir duas ou mais categorias)*. 
**A análise descritiva de variáveis qualitativas** é feita por meio de tabelas de frequência e gráficos, pois tais variáveis não permitem o cálculo de medidas de posição e dispersão

Escalas Likert, Faixa de renda, Nacionalidade, Estado civil, Escolaridade, Tipo de solo, Vacinado ou não, Tipos de comorbidades.

### Quantitativas: 
São variáveis métricas, atribuem contagem ou mensuração. Sendo discretas (números inteiros) ou contínuas (valores reais).
A análise descritiva de variáveis quantitativas pode ser feita por diversas ferramentas estatísticas, incluindo as medidas de posição e dispersão comoi Idade, Renda (em R$), Quantidade de filhos, Altura da pessoa (em cm), Peso (em kg), Retorno de ações na bolsa, Temperatura do ambiente, Lucro/prejuízo da empresa.

## 2)  Estatística Descritiva:
A análise descritiva é uma etapa crucial para entender os dados. Ela envolve a **criação de tabelas de frequência e gráficos** para variáveis qualitativas, e o cálculo de medidas de posição e dispersão para variáveis quantitativas.

### 1) Tabelas de Frequências: 
Quantidade de ocorrências por categoria
#### - **Qualitativas**
De forma direta, apresenta a quantidade de ocorrências para cada categoria

#### - **Quantitativas**

**Variável discreta**: a análise assemelha-se ao caso da variável qualitativa, ou 
seja, mostra a quantidade de ocorrências para cada valor discreto da variável

**Variável contínua**: é necessária uma categorização inicial por classes ou faixas para, em seguida, apresentar a quantidade de ocorrências em cada categoria gerada.

### 2)  Medidas de Posição: 
- **Média**
- **Mediana**
- **Moda**
- **Percentis**
- **Quartis**
- **Decis**

### 3)  Medidas de Dispersão: 
- **Amplitude**
- **Variância** 
- **Desvio Padrão**
- **Erro Padrão**
- **Coeficiente de Variação.**


**Amplitude** - Apresenta a diferença entre o valor máximo e o valor mínimo de uma variável

**Variância** - Mostra a dispersão das observações de uma variável em torno de sua média

**Desvio padrão** - É uma medida derivada da variância, tornando mais simples a interpretação da dispersão em torno da média -  A variância é definida em termos quadrados, o que dificulta a interpretação

O desvio padrão é a raiz quadrada da variância
• Erro padrão - É o desvio padrão da média da variável
• Sendo que S é o desvio padrão da variável e n o tamanho da amostra
• Quanto maior o tamanho da amostra, menor o erro padrão na estimativa da
média da variável mais precisa é a média estimada

**Coeficiente de variação** - *É uma medida de dispersão relativa*, pois **relaciona o desvio padrão e a média de uma variável**
• Pode ser utilizada para realizar comparações entre amostras, por exemplo
• Quanto menor o CV, mais homogêneos são os valores da variável e mais
concentrados estão os valores em torno da média


### 4) - Medidas de Forma - Assimetria e Curtose: 
- Avaliam distribuição (simétrica, assimétrica, achatada).

**Assimetria**: Local de Concentração da Distribuição
• Curva Simétrica: Média = Mediana = Moda
• Curvas Assimétricas – Direita: tem cauda mais longa à direita Média > Mediana
• Curvas Assimétricas – Esquerda: tem cauda mais longa à esquerda Média < Mediana

**Assimetria**: Coeficiente de Assimetria de Fisher:
• g1 = 0 indica curva simétrica
• g1 > 0 indica curva assimétrica positiva (à direita)
• g1 < 0 indica curva assimétrica negativa (à esquerda)

**Curtose**: Achatamento da Curva de Distribuição
• Com a curva normal como referência, é possível observar se as curvas têm menor
dispersão em torno da média ou maior dispersão em torno da média

**Curtose:** Coeficiente de Curtose de Fisher:
• g2 = 0 indica curva com distribuição normal
• g2 > 0 indica curva com distribuição alongada
• g2 < 0 indica curva com distribuição achatada


### Posição, dispersão e forma
**Exercício para aplicação conjunta das medidas**

 Um consumidor está analisando o preço de um produto que deseja comprar. Para gerar mais informações para sua tomada de decisão, ele coleta 100 preços praticados para o produto. Como o “preço” é variável quantitativa, serão realizadas as análises por meio das medidas de posição, dispersão e forma abordadas anteriormente.


## 5) Variáveis Aleatórias e Distribuições de Probabilidade:

5. **Relação entre variáveis**
• Medidas de análises bivariadas
• Muitas vezes, o interesse pode estar na relação entre duas variáveis. Nestes
casos, antes, é importante conhecer o tipo de variável:
• Variáveis qualitativas: análise da associação pelo teste qui-quadrado (χ2)
• Variáveis quantitativas: análise da correlação por meio da covariância e coeficiente de correlação de Pearson

5. **Relação entre variáveis**
• Teste qui-quadrado: variáveis qualitativas
• Inicia-se por meio de uma tabela de distribuição conjunta de frequências, a
tabela de contingência (ou tabela de classificação cruzada) que apresenta as
frequências absolutas observadas para cada par de categorias das variáveis

• **Teste qui-quadrado: variáveis qualitativas**

Em seguida, são identificadas as frequências absolutas esperadas para cada
par de categorias das variáveis

O mesmo cálculo é realizado para cada par de categorias da tabela de contingência,
mantendo-se as respectivas correspondências de linha e coluna no numerador

Posteriormente, são identificados os resíduos para cada par de categorias das
variáveis

Os resíduos são identificados para cada par de categorias da tabela de contingência

Por fim, são calculados os valores χ2 individuais de cada par de categorias

𝝌² = (𝒓𝒆𝒔í𝒅𝒖𝒐)² dividido (𝒇𝒓𝒆𝒒. 𝒂𝒃𝒔𝒐𝒍𝒖𝒕𝒂 𝒆𝒔𝒑𝒆𝒓𝒂𝒅𝒂)

E são somados valores χ2 individuais para obter o valor χ2 total da’ análise

Com base no valor χ2 total, realiza-se o seguinte teste:
• H 0: as variáveis se associam de forma aleatória. • H 1: a associação entre as variáveis não se dá de forma aleatória.
• Dados o nível de significância e os graus de liberdade, se o valor da estatística χ2 for maior do que seu valor crítico, há associação significante entre as duas variáveis (H1)
• Valor crítico da distribuição χ2 com (I – 1) . (J – 1) graus de liberdade

**Exercícios Coeficiente de correlação de Pearson**
 
1 - Um estudo foi realizado com 200 pessoas com o intuito de analisar o comportamento conjunto da variável “operadora de plano de saúde” com a variável “nível de satisfação” do consumidor. O objetivo é analisar se existe a associação estatisticamente significativa entre tais variáveis. 
• Os dados da tabela de contingência obtida a partir da amostra está na planilha suportena aba Associação – Qui².

 **- Coeficiente de correlação de Pearson**

É utilizado para identificar a correlação entre duas varáveis quantitativas

Inicia-se pelo cálculo da covariância entre as duas variáveis e, posteriormente,
obtém-se o coeficiente de correlação de Pearson

2 - Exemplo: O coordenador de um curso deseja analisar se existe correlação entre as notas dos alunos em diferentes matérias. Para tanto, montou um banco de dados com as notas de 30 alunos para as disciplinas de matemática, física e literatura. 

Em seguida, deseja calcular os pares de correlações entre as notas de matemática – física, matemática – literatura e física – literatura. Quais são as correlações de Pearson obtidas?

### Variável Aleatória Discreta: **Assumem valores inteiros**
**As variáveis aleatórias discretas são aquelas que assumem valores inteiros, ou seja, valores isolados. Aqui estão algumas distribuições de probabilidade associadas a variáveis aleatórias discretas:**

- **1 - Distribuição Uniforme Discreta** - Nessa distribuição, todos os valores possíveis têm a mesma probabilidade de ocorrer. Um exemplo é lançar um dado justo, onde cada número de 1 a 6 tem a mesma chance de sair.
- **2 - Distribuição Binomial** - A distribuição binomial é usada quando há um número fixo de tentativas independentes, cada uma com dois resultados possíveis (geralmente chamados de sucesso e fracasso), e estamos interessados no número total de sucessos. Exemplos incluem lançamento de moedas ou testes de sucesso/falha.
- **3 - Distribuição Binomial Negativa** - Similar à distribuição binomial, mas aqui estamos interessados no número de tentativas necessárias para atingir um certo número de sucessos. Isso é relevante em situações como tentar acertar um alvo em tiros consecutivos.
- **4 - Distribuição Poisson** - A distribuição Poisson é usada para modelar o número de eventos raros que acontecem em um intervalo de tempo ou espaço. Exemplos incluem o número de chamadas de emergência em um período de tempo ou o número de acidentes em uma interseção.


### Variável Aleatória Contínua: **Assume qualquer valor real**
**As variáveis aleatórias contínuas podem assumir qualquer valor real em um intervalo. Aqui estão algumas distribuições de probabilidade associadas a variáveis aleatórias contínuas:**
- **1 - Distribuição Normal (Normal Padrão).**
A distribuição normal é amplamente conhecida e representa muitos fenômenos naturais. É caracterizada por sua forma de sino e é completamente determinada por sua média e desvio padrão.
- **2 - Distribuição Qui-Quadrado.**
A distribuição qui-quadrado é usada em testes de hipóteses e para intervalos de confiança relacionados à variância em uma amostra.
- **3 - Distribuição t de Student.**
A distribuição t de Student é frequentemente usada quando as amostras são pequenas e a distribuição normal não pode ser assumida, ou em testes de médias populacionais.
- **4 - Distribuição F de Snedecor.**
A distribuição F é usada em análises de variância (ANOVA) e comparações de variâncias de duas ou mais amostras.



**1 - Distribuição uniforme discreta - Variável aleatória discreta:**
• Todos os possíveis valores têm a mesma probabilidade de ocorrência
• 𝑷 𝑿 = 𝒙𝒊 = 𝟏/n
• Exemplo: As probabilidades dos resultados possíveis ao lançar um dado são:
• P(X=1) = 1/6
• P(X=2) = 1/6
• P(X=3) = 1/6
• P(X=4) = 1/6
• P(X=5) = 1/6
• P(X=6) = 1/6
• O parâmetro n representa a quantidade de possíveis valore

**2 - Distribuição de Bernoulli - Variável aleatória discreta:**
• Os valores da variável podem assumir apenas dois resultados possíveis, sendo
que tais resultados são chamados de sucesso (x=1) ou fracasso (x=0)
• A distribuição de Bernoulli apresenta a probabilidade de sucesso (p) ou de
fracasso (1 – p) quando ocorre apenas um experimento
• 𝑷 𝑿 = 𝒙 = 𝒑𝒙 . (𝟏 - 𝒑)𝟏-𝒙
• Exemplo: A probabilidade (p) de que um candidato seja aprovado (x=1) em um exame para um conselho de classes é de 48%. Se cada candidato só pode realizar o exame uma vez, analise as probabilidades possíveis por meio da distribuição de Bernoulli.
• P(X=1) = (0,48)¹ . (1 – 0,48)0 = 0,48 ou 48%
• P(X=0) = (0,48)0 . (1 – 0,48)¹ = 0,52 ou 52%
• Sendo que X=1 é aprovação e X=0 é a reprovação no exame

**3 - Distribuição binomial - Variável aleatória discreta:**
• A distribuição binomial ocorre quando há (n) repetições independentes do
experimento de Bernoulli e a probabilidade de sucesso (p) é constante em
todas as repetições
• A variável no modelo binomial indica a quantidade de sucessos (k) nas (n)
repetições do experimento


• Exemplo: Em uma indústria, sabe-se que a probabilidade (p) de encontrar peças defeituosas em cada lote produzido é 6,50%. São produzidos 12 lotes (n) da peça por mês. Analise as seguintes probabilidades (k):
a) Qual a probabilidade de encontrar peças defeituosas em 2 lotes no mês?
b) Qual a probabilidade de encontrar peças defeituosas em 4 lotes no mês?
c) Qual a probabilidade de encontrar peças defeituosas em no máximo 2 lotes?
• A planilha para auxílio está na planilha de suporte na aba Distribuição Binomial

**4 - Distribuição binomial negativa - Variável aleatória discreta:**
• Na distribuição binomial negativa, são realizados (x) ensaios independentes
de Bernoulli até que sejam obtidos (k) sucessos
• A probabilidade de sucesso (p) é constante em todos os ensaios realizados
• A variável no modelo binomial negativa indica a quantidade de ensaios (x)
Exemplo: Em um parque de diversões, existe uma máquina em que o jogador deve capturar algum item utilizando os comandos de um braço mecânico. Considere que a probabilidade (p) de que o jogador consiga capturar algum item em cada jogada é 11%. Identifique as seguintes probabilidades:
a) De que o jogador necessite de (x)10 jogadas para capturar (k)3 itens.
b) De que o jogador necessite de (x)20 jogadas para capturar (k)3 itens.
c) De que o jogador necessite de (x)5 jogadas para capturar (k)1 item.
• A planilha para auxílio está na planilha de suporte na aba Distribuição Binomial Negativa

**5 - Distribuição Poisson - Variável aleatória discreta:**

• A distribuição Poisson indica a probabilidade do número de sucessos (k) em
uma determinada exposição contínua
• Exemplos de exposição: tempo e área
• Em que 𝝀 é a taxa média estimada de ocorrência do evento (sucesso) em dada exposição,
Exemplo: Um médico notou que a taxa média de ocorrência (𝝀) de pacientes com certa doença rara em seu consultório é de 2 por ano. Aceitando que esta variável tenha distribuição Poisson, estime:
a) A probabilidade de que o médico receba 1 paciente com a doença em um ano.
b) A probabilidade de que o médico receba 3 pacientes com a doença em um ano.
c) A probabilidade de que o médico não receba pacientes com a doença em um ano.
d) A probabilidade de que o médico receba 10 pacientes com a doença nos próximos 2
anos.
• A planilha para auxílio está na planilha de suporte na aba Distribuição Poisson.


**1 - Distribuição normal padrão - Variável aleatória contínua:**
• É a distribuição Gaussiana, com curva em forma de sino
• Os parâmetros relevantes da distribuição normal são a média (μ) e o desvio
padrão (σ) da variável
• Para obter a normal padrão, transforma-se a variável por meio do Z-score
• A transformação pelo Z-score faz com que a variável passe a ter média = 0 e
desvio padrão = 1 e não altera a distribuição original
Exemplo: valores críticos em uma tabela normal padrão e no Excel

• Exemplo: Um investidor calculou que o retorno médio mensal de uma ação na bolsa de valores foi 2,80%. No mesmo período, o desvio padrão dos retornos da ação foi de 1,20%. Com base na distribuição normal, calcule:
a) A probabilidade de que o retorno da ação seja maior do que 4% ao mês.
b) A probabilidade de que o retorno da ação seja menor do que 3% ao mês.
c) A probabilidade de que o retorno da ação seja negativo.
d) A probabilidade de que o retorno da ação seja maior que 1% e menor que 5% ao mês.
• A planilha para auxílio está na planilha de suporte na aba Distribuição Normal


**2 - Distribuição qui-quadrado (χ2) - Variável aleatória contínua:**
• A distribuição χ2 apresenta curva assimétrica e positiva
• É formada a partir da soma dos quadrados de v variáveis aleatórias
independentes com distribuição normal padrão
**Exemplo:** valores críticos em uma tabela qui-quadrado e no Excel
Exemplo: Um pesquisador em botânica identificou que uma variável de seu estudo segue uma distribuição qui-quadrado e tem 7 graus de liberdade. Com base nestas informações, o pesquisador calculou:

a) A probabilidade de que encontre um valor X>6.
b) A probabilidade de que encontre um valor X<8.
c) O valor de X que faz com que a P(X>x) seja 5%.
d) O valor de X que faz com que a P(X<x) seja 90%.
• A planilha para auxílio está na planilha de suporte na aba Distribuição Qui-Quadrado

**3 - Distribuição t de Student - Variável aleatória contínua:**
• A distribuição t de Student é parecida com a distribuição normal padrão, ou
seja, tem formato de sino e é simétrica em torno da média
• Por outro lado, a distribuição t de Student tem caudas mais longas e isso
permite valores mais extremos
• Uma aplicação da distribuição t de Student é o teste de hipóteses para médias
• Exemplo: valores críticos em uma tabela t de Student e no Excel

**Exemplo:** O gestor do controle de qualidade de uma empresa identificou que uma variável relevante para seu controle apresenta distribuição t de Student e tem 7 graus de liberdade. Quais são suas análises nas situações:
a) A probabilidade de que encontre T > 2,5.
b) A probabilidade de que encontre T < - 2,5.
c) A probabilidade de que encontre T>-1 e T<2.
d) O valor de T para que P(T>t) = 5%.
• A planilha para auxílio está na planilha de suporte na aba Distribuição t Student.


**4 - Distribuição F de Snedecor - Variável aleatória contínua:**
• Uma aplicação comum da distribuição F (distribuição de Fischer) ***é a análise
de variâncias***
• Tem distribuição de probabilidades assimétrica e positiva quando os graus de liberdade v
1 e v2 são pequenos
• Exemplo: valores críticos em uma tabela F de Snedecor e no Excel

• **Exemplo:** Um cientista de dados está avaliando uma variável com distribuição
F de Snedecor. Tal variável apresenta 17 graus de liberdade no numerador e
28 graus de liberdade no denominador. Determine:
a) A probabilidade de que encontre X > 1,5.
b) A probabilidade de que encontre X < 1,0.
c) A probabilidade de que encontre 2<X<3.
d) O valor de F para que P(X>x) = 5%.


Testes de Hipóteses
• Finalidade
• Em certos casos, podemos estar interessados em testar características sobre
parâmetros populacionais como a média e o desvio padrão (variância)
• Dada a impossibilidade de obter os dados sobre a população, utilizamos as
amostras da população
• Para testar o parâmetro de interesse por meio de amostras, utilizamos os
testes de hipóteses estatísticas

• Teste bilateral (bicaudal)
• No teste bilateral, para um parâmetro θ, o interesse é testar:
• H
0: θ = θ0 (hipótese nula)
• H
1: θ ≠ θ0 (hipótese alternativa)
• O objetivo ***é verificar se o parâmetro é estatisticamente diferente de certo valor de interesse
• É necessário definir o nível de significância (α) desejada para a análise

• Teste unilateral à esquerda
• No teste unilateral à esquerda, para um parâmetro θ, o interesse é testar:
• H 0: θ = θ0 (hipótese nula)
• H 1: θ < θ0 (hipótese alternativa)
• O objetivo é analisar se o parâmetro é estatisticamente menor do que certo
valor de interesse

• Teste unilateral à direita
• No teste unilateral à direita, para um parâmetro θ, o interesse é testar:
• H 0: θ = θ0 (hipótese nula)
• H 1: θ > θ0 (hipótese alternativa)
• O objetivo é verificar se o parâmetro é estatisticamente maior do que certo
valor de interesse

Tipos de erros
• Possíveis erros na tomada de decisão
• Erro tipo I: rejeitar a hipótese nula (H0) quando ela é verdadeira
• Erro tipo II: não rejeitar a hipótese nula (H0) quando ela é falsa
• As decisões corretas são:
• Rejeitar H0 quando ela é falsa
• Não rejeitar H0 quando ela é verdadeira

Significância do teste
• Nível de significância do teste
• O nível de significância (α) indica a probabilidade de rejeitar H0 quando ela é
verdadeira, ou seja, a probabilidade de cometer o erro tipo I
• Alguns níveis de significância recorrentemente utilizados:
• α = 1%
• α = 5%
• α = 10%
• O nível de confiança do teste é definido como 1 – α

P-valor e teste de hipótese
• P-valor e nível de significância
• Uma forma de testar estatisticamente a hipótese é comparando o valor da
estatística calculada nos dados com o valor crítico para o nível de significância
• Também é possível obter o p-valor para a estatística calculada e, em seguida,
compará-lo ao nível de significância escolhido
• Se p-valor < nível de significância (α) rejeita-se H0
• Se p-valor > nível de significância (α) não rejeita H0
• O p-valor é a probabilidade associada ao valor da estatística calculada

1 - Teste Z para médias de uma amostra
• Aplicado quando o desvio padrão populacional é conhecido e a distribuição
da variável é normal (ou utilizando grandes amostras)
• A estatística do teste é:
• A distribuição relevante para os valores críticos é a normal padrão

Teste Z para médias de uma amostra
• Exemplo: Um fabricante de caixas de papelão deseja verificar se a quantidade de papelão que está sendo utilizada em cada caixa do tipo 1 está de acordo com seu padrão histórico, pois existem indícios de que o consumo aumentou. Historicamente, são utilizados, em média, 100 g de papelão em cada caixa e o desvio padrão é de 12g. Coletou-se uma amostra para verificar se a média atual é maior do que a média histórica.
• A amostra coletada está na planilha suporte na aba Teste Z médias.


 2 - Teste t para correlações – vai usar o desvio padrão amostral
• Após estimado o coeficiente de correlação (r) entre as variáveis quantitativas,
é possível testar a significância do parâmetro estimado
• Estatística do teste:
• A distribuição relevante é a t de student com n-2 graus de liberdade

• Teste t para correlações
• Exemplo: Voltando ao exemplo da correlação entre as notas dos alunos, agora o objetivo é avaliar se as correlações obtidas para as amostras de notas são significantes. O coordenador utilizou o nível de significância de 5% para suas análises.
• Os dados estão na planilha suporte na aba Correlação de Pearson

3 - Teste qui-quadrado para uma amostra
• Aplicado quando a variável assume duas ou mais categorias (K) e o objetivo é
verificar se há diferenças entre as frequências observada (O) e esperada (E)
• A estatística do teste é:
• A distribuição relevante é a qui-quadrado com k-1 graus de liberdade

• Exemplo: Uma loja deseja verificar se a quantidade vendida em cada dia da semana varia em função do dia da semana. Os dados para as vendas em cada dia de uma semana escolhida aleatoriamente foram tabulados. Neste caso, o objetivo é testar se a frequência observada e esperada são iguais ou se são diferentes. (Fonte: Fávero e Belfiore, 2017, Cap. 8)

4 - Teste F para comparação de variâncias (quantitativa)
• Aplicado para comparar as variâncias de duas amostras independentes
• A estatística do teste é:
• A distribuição relevante é a F de Snedecor, com n-1 graus de liberdade no
numerador e n-1 graus de liberdade no denominador

Teste F para comparação de variâncias
• Exemplo: Uma empresa de logística está analisando qual entre duas rotas oferece a melhor previsibilidade para o horário de entrega ao seu maior cliente. Foram coletados dados sobre o tempo de entrega durante 35 dias para cada rota. O diretor de logística deseja testar a hipótese que a rota B tem maior variabilidade no tempo de entrega, comparativamente à rota A.
• Os dados estão na planilha suporte na aba Teste F Variâncias

• Intervalo de confiança para a média
• Quando obtemos a estimativa para a média populacional a partir de uma
amostra, também podemos construir seu intervalo de confiança, isto é, um
intervalo de valores possíveis para o parâmetro populacional
• É necessário estabelecer o nível de confiança da análise (por exemplo, 95%)

• Exemplo: Um engenheiro coletou uma amostra de 25 peças saídas da linha de montagem e encontrou que o tamanho médio foi de 47cm e o desvio padrão foi 1cm. Qual é o intervalo de confiança com 95% para esta média estimada?
• Os dados estão na planilha de suporte na aba Intervalo de Confiança – Média

• Teste t para comparação de médias em
duas amostras independentes
• Para comparar as médias de duas amostras independentes de uma mesma
população por meio do teste t, antes é necessário comparar as variâncias
populacionais dos dois grupos
• Por exemplo, antes pode ser feito um teste F para comparação das variâncias
• O cálculo da estatística t e graus de liberdade depende: se as variâncias
populacionais forem diferentes ou se são homogêneas
• Teste t para comparação de médias em
duas amostras independentes
• Estatística T para variâncias populacionais diferentes
• Teste t para comparação de médias em
duas amostras independentes
• Estatística T para variâncias populacionais homogêneas

• Teste t para comparação de médias em
duas amostras independentes
• Exemplo: Em uma indústria, o gerente de produção fez um levantamento com 30 medições da temperatura (em °C) dos dois principais fornos da linha de produção que produzem os produtos do mesmo tipo. Destas, 15 medições foram do forno A e 15 medições foram para o forno B. O objetivo é verificar se a temperatura média está consideravelmente diferente entre os fornos.
• Os dados estão na planilha suporte na aba Teste t Duas Amostras Indep
