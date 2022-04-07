![Covid-19](https://cdn.pixabay.com/photo/2020/03/30/03/20/covid-19-4982910_960_720.jpg)

---
# Projeto Bootcamp Data Science 3 - Criação de modelo preditivo para decisão de ingresso de paciente na UTI após análise de exames
---

Olá! Bem vindo ao meu repositório relativo ao Bootcamp Data Science 3 da Alura! Aqui, na pasta **notebooks**, estará uma análise feita em cima dos dados do [Sírio-Libanês](https://hospitalsiriolibanes.org.br/) de internações em UTI de pacientes após realização de bateria de exames e análise de profissional da saúde. Abaixo detalherei melhor qual o escopo do projeto, quais dados serão utilizados e como estes servirão como base para minhas conclusões.

## Os dados
---

Neste projeto, estão sendo utilizados dados fornecidos pelo hospital [Sírio-Libanês](https://www.kaggle.com/datasets/S%C3%ADrio-Libanes/covid19). O Hospital realizou levantou uma série de dados a respeito de pacientes que foram internados na UTI com caso grave do COVID-19. Cerca de 300 pacientes registraram entrada no hospital e após realização de bateria de exames, foram encaminhados para leitos de UTI ou liberados para realização de tratamento em casa.

## O Objetivo
---

Os dados fornecidos foram coletados em ordem de buscar um modelo preditivo que indique as chances de encaminhar o paciente para o leito de UTI após a realização de primeira bateria de exames. Tal processo decisório necessita ser executado de maneira rápida e com o mínimo de burocracia de modo a evitar piora no estado de saúde do paciente.

Obviamente, a presença do profissional ainda será necessária na realização de *double check* de modo a reafirmar a validade do modelo ou se o mesmo necessita ser corrigido.

## Como será feito
---

Considerando o que foi explanado anteriormente, para criar um modelo decisório para ingresso de pacientes na UTI dados certas variáveis serão realizados os seguintes passos:

- Importação dos dados do Sírio-Libanês;
- Realização de limpeza dos dados;
- Remoção de informações correlacionadas que dificultem o poder decisório do modelo;
- Criação de 5 modelos preditivo;
- Alteração de hiper pârametros para atingir melhor acurácia em cada modelo;
- Apuração de modelo preditivo e salvá-lo para uso futuro;

## Resultados
---

Como resultado, foi encontrado um modelo [Logistic Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html) ajustado com o seguinte hiper parâmetro: 
```
LogisticRegression(solver='newton-cg')
```

assim gerando um AUC médio de **[78,06 ± 0,83] %**  com uma acurácia de **76,99%**.

## Conclusão
---

Este projeto buscou analisar, de maneira simples e direta, o banco de dados disponibilizado pelo hospital [Sírio-Libanês](https://www.kaggle.com/datasets/S%C3%ADrio-Libanes/covid19). Os dados representam um conjunto de pacientes diagnosticados com COVID-19 que passaram por uma bateria de exames, em determinadas janelas de tempo, e foram encaminhados para Unidade de Terapia Intensiva (UTI) do hospital ou liberados para finalização de tratamento em suas casas.

Os dados recebidos foram manipulados com o intuito de gerar uma planilha coesa, completada com dados numéricos e categóricos de modo que os modelos de ML possam ser aplicados. Após a manipulação, foram analisadas e removidas a variáveis correlacionadas, que dificultariam o cálculo do modelo. 

Com isto, o melhor modelo que se adapta as condições foi o **[Logistic Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)** com uma AUC de **78,06%**.

Com ele, foi gerado uma matriz de confusão com **118** verdadeiros Positivos e **153** Verdadeiros negativos. 