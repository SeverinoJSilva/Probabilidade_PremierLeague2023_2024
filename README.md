# Calculando Resultado da **Premier League 2023-2024**
__________________________________________________________________________________________________

### Fazendo Previsões dos Resultados dos Jogos da **Premier League temporada 2023 e 2024**.

### Ao baixar um novo arquivo o código pode ser rodado novamente e obter novas probabilidades.

- Fonte dos Dados: https://www.football-data.co.uk/books.php
__________________________________________________________________________________________________

# O presente projeto tem por objetivo:

1. Calcular a probabilidade de resultado dos jogos (vitória da casa, empate e vitória do visitante).

2. A probabilidade de número de gols do jogo (de 0 a 9 gols).

3. A probabilidade da pontuação final da esquipes da Premier League 2023-2024.

________________________________________________________________________________________________________

# Calculando resultados (utilizando a distribuição de Poisson)
​
Vamos fazer o cálculo da probabilidade de Vitória da Casa, Empate e Vitória do Visitante.
__________________________________________________________________________________________________

1. P_Draw - Empate

2. P_Home - Vitória Casa

3. P_Away - Vitória Visitante
__________________________________________________________________________________________________
​
A distribuição de Poisson é uma distribuição de probabilidade discreta que modela o número de eventos raros que ocorrem em um intervalo fixo de tempo ou espaço, dado um taxa média de ocorrência desses eventos. 

Ela é nomeada em homenagem ao matemático francês Siméon Denis Poisson.
​
A lógica por trás da distribuição de Poisson pode ser explicada pelos seguintes pontos-chave:
​
Eventos Raros e Independentes: 

A distribuição de Poisson é apropriada para modelar eventos que são raros e independentes um do outro. 

Eventos raros significam que a probabilidade de mais de um evento ocorrer em um intervalo muito curto de tempo é praticamente nula. 

Além disso, a ocorrência de um evento não afeta a ocorrência de outros eventos.
​
Taxa Média de Ocorrência (λ): A distribuição de Poisson é caracterizada por um único parâmetro, denotado por λ (lambda), que representa a taxa média de ocorrência dos eventos no intervalo considerado. 

Se λ é a média de eventos por unidade de tempo ou espaço, então a distribuição de Poisson modela o número de eventos que ocorrem em uma unidade de tempo ou espaço.
​
Probabilidade de Ocorrência de k Eventos: A função de massa de probabilidade (PMF) da distribuição de Poisson é dada por:
​
P(X = k) = (e^(-λ) * λ^k) / k!,
​
onde:
​
P(X = k) é a probabilidade de exatamente k eventos ocorrerem,

λ é a taxa média de ocorrência,

e é a base do logaritmo natural (aproximadamente 2.71828),

k! é o fatorial de k.

Essa fórmula expressa a probabilidade de exatamente k eventos ocorrerem em um dado intervalo de tempo ou espaço, dado a taxa média de ocorrência λ.
​
Esperança e Variância: A esperança (valor médio) e a variância de uma distribuição de Poisson são ambos iguais a λ. 

Isso significa que, em média, espera-se que o número de eventos observados seja igual à taxa média de ocorrência.
​
A distribuição de Poisson é amplamente utilizada em diversas áreas, como estatística, teoria das filas, teoria de confiabilidade e modelagem de fenômenos naturais, onde eventos raros e independentes são comuns.
