![Covid-19](https://cdn.pixabay.com/photo/2020/03/30/03/20/covid-19-4982910_960_720.jpg)

---
# Projeto Módulo 1 do Bootcamp Data Science 3 - Análise de internações e óbitos do SUS ocorridos de 2008 a 2021
---

Olá! Bem vindo ao meu repositório relativo ao Bootcamp Data Science 3 da Alura! Aqui, na pasta **notebooks**, estará uma analise feita em cima dos dados do SUS de internações e óbitos no Brasil. Abaixo detalherei melhor qual o escopo do projeto, quais dados serão utilizados e como estes servirão como base para minhas conclusões.

## Os dados
---

Neste projeto, estão sendo utilizados dados fornecidos pelo sistema [datasus](http://tabnet.datasus.gov.br/cgi/deftohtm.exe?sih/cnv/qibr.def). Tal sistema fornece ao usuário dados sobre custos, óbitos, internações, tempo de permanência dentre outros, podendo fornecer números em relação a municípios, capitais e demais macroregiões que se encontram integradas ao sistema.

## O Objetivo
---

Após finalização do módulo 1 do Bootcamp, surgiu-me a dúvida se poderia correlacionar dados de internações hospitalares em relação a taxa de óbitos ocorrida no mesmo período. Sendo assim, realizei minha análise com dois *DataSets* distintos.

## Como será feito
---

Para obter o resultado desejado, o presente trabalho utilizou retirada de dados a partir de dois arquivos CSV. Os *DataFrame* criados foram previamente filtrados de modo que apenas as informações relevantes estivessem presentes.

Para plotagem de gráficos, a biblioteca *Matplotlib* foi utilizada de modo a alterar as vizualizações deixando-as claras e objetivas para o leitor.

## Resultados
---

Como resultados foram plotados gráficos comparativos através da ferramenta subplot, onde dados sobre internações eram plotados com sua contraparte de óbitos no mesmo período de tempo. Com isto foi possível realizar análises visuais.

## Conclusões
---

As análises por região nos mostra um padrão a respeito da queda de internações registradas no inicio de 2020 e consequente aumento de óbitos, representando assim a chegada da primeira onda da pandemia. Já para a segunda onda, chegou-se na conclusão que a curva de internações da segunda onda não caiu tal qual a primeira, pois foram construídos hospitais de campanha em todo país o que auxiliou no aumento do número de leitos ocupados. 