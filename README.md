# Análise de dados - COVID-19
O objetivo deste repositório é realizar uma análise preditiva da evolução dos casos de infecção da COVID-19 no Brasil.

Duas fontes de dados foram utilizadas: as duas foram retiradas do Kaggle (https://www.kaggle.com/datasets/sudalairajkumar/novel-corona-virus-2019-dataset) em momentos diferentes, então uma delas (df1) contém informações do dia 22/01/2020 até 19/05/2020 (df1) e a outra (df2) está um pouco mais atualizada e possui registros até o dia 29/05/2021 (df2).

Com isso foi possível realizar uma análise preditiva a partir dos dados do df1 e da ferramenta Prophet, que é utilizada para previsões de séries temporais, e comparar o resultado com as observações reais (df2), meramente a título de curiosidade.

**A análise e a comparação foram realizadas da seguinte forma:**

\- Para a predição, foi considerado que 16 milhões de brasileiros se infectariam (este número foi escolhido apenas para igualar a escala e facilitar a comparação visual dos gráficos; qualquer outro valor, desde que considere o número da população a ser predita, poderia ser inserido). Na Imagem1 (Predições de casos confirmados no Brasil) a linha em vermelho representa os números reais, que serviram de base para treino do modelo, e a linha em azul representa a predição do número de infectados. 

No cenário descrito acima, a curva se achataria em outubro/2020, após 16 milhões de brasileiros serem infectados.

![Predições de casos confirmados no Brasil](https://github.com/isabela-rossetti/analise_de_dados_covid/blob/main/Imagem1.png)


\- Já nos dados reais representados na Imagem2 (Casos confirmados no Brasil – Até novembro/2020) podemos observar que em outubro/2020 o número de infectados era de aproximadamente 5 milhões e não havia achatamento na curva.

![Casos confirmados no Brasil – Até novembro/2020](https://github.com/isabela-rossetti/analise_de_dados_covid/blob/main/Imagem2.png)

\- No último gráfico, Imagem3 (Casos confirmados no Brasil – Até maio/2021), podemos observar que a marca de 16 milhões foi registrada em 23/05/2021. O achatamento da curva não foi detectado até essa data e o número de casos continuou subindo (lembrando que os dados analisados neste projeto registraram informações até o dia 29/05/2021).

![Casos confirmados no Brasil – Até maio/2021](https://github.com/isabela-rossetti/analise_de_dados_covid/blob/main/Imagem3.png)
