# <p align = "center"> **TalkingData AdTracking Fraud Detection Challenge**
*19/08/2021 -*

[![Github](https://img.shields.io/badge/gustavolq-100000?style=plastic&logo=github&logoColor=white)](https://github.com/gustavolq)
[![linkedin](https://img.shields.io/badge/gustavoquadra-0077B5??style=plasticlogo=linkedin&logoColor=white)](https://www.linkedin.com/in/gustavoquadra)
![R-Language](https://img.shields.io/badge/R-276DC3?style=plastic&logo=r&logoColor=white)

<img src = "https://www.thebeijinger.com/sites/default/files/thebeijinger/event-images/376094/screen_shot_2018-05-29_at_10.08.48_am.png">


Olá! Seja muito bem-vindo ao meu repositório referente ao projeto de detecção de fraude de cliques da TalkingData.

Para realização do projeto utilizei o Jupyter Notebook, um aplicativo open-source que permite a execução de células com códigos e textos, junto com a Linguagem R, uma linguagem estatística muito utilizada para a manipulação, análise e visualização de dados, assim como o desenvolvimento de Machine Learning.

 # **<p align="center"> 💻 Sobre o Projeto 💻**
## **Introdução**
O projeto de detecção de fraudes em cliques foi um desafio proposto na comunidade Kaggle, uma plataforma voltada para Cientistas de Dados e profissionais de aprendizado de máquina, pela empresa chinesa TalkingData no ano de 2018.

Caso você queira verificar o desafio proposto no Kaggle, podes clicar [aqui](https://www.kaggle.com/c/talkingdata-adtracking-fraud-detection) para acessar a página.

## **Objetivo do Projeto**
O objetivo desse projeto será realizar a criação de um modelo de aprendizado de máquina para determinar se um clique em um anúncio é fraudulento ou não.
## **Planejamento do Projeto**
Para a realização do projeto, seguiremos o seguinte planejamento :

<b> 1.</b> Introdução </br>
<b> 2.</b> Definição do Problema de Negócio </br>
<b> 3.</b> Preparação dos Dados </br>
<b> 4.</b> Análise Exploratória dos Dados </br>
<b> 5.</b> Pré-Processamento
<b> 6.</b> Criação do Modelo de Machine Learning </br>
<b> 7.</b> Otimização do Modelo de Machine Learning </br>
<b> 8.</b> Conclusão </br>

## **Dados Utilizados no Projeto**
Os dados utilizados no projeto foram disponibilizados pela TalkingData através da página da competição Kaggle e você pode acessar clicando [aqui](https://www.kaggle.com/c/talkingdata-adtracking-fraud-detection/data).

Iremos utilizar os seguintes dados para o projeto :
- train.csv : Dados de treino com 184.903.891 linhas e 8 colunas.
- test.csv : Dados de teste com 18.790.470 linhas e 7 colunas.

Para melhor organização e poder processar em máquinas com baixa memória RAM irei realizar a divisão do train.csv e test.csv em 5 arquivos menores, sendo :
- train.csv : Dividido em 5 arquivos com 36.980.778 linhas cada
- test.csv : Dividido em 5 arquivos com 3.758.094 linhas cada

Os arquivos separados estarão disponibilizados na pasta [Data]() desse repositório.

# **<p align="center"> Um pouco sobre a TalkingData**

A TalkingData, maior plataforma de Big Data independente da China, cobre mais de 70% dos dispositivos móveis ativos em todo o país, lidando com 3 bilhões de cliques por dia, dos quais 90% são potencialmente fraudulentos. Sua abordagem atual para impedir fraudes de cliques para desenvolvedores de aplicativos é medir a jornada do clique de um usuário em todo o portfólio e sinalizar endereços IP que produzem muitos cliques, mas nunca acabam instalando aplicativos. Com essas informações, eles criaram uma lista negra de IPs e uma lista negra de dispositivos.

Embora bem-sucedidos, eles querem estar sempre um passo à frente dos fraudadores e desejam desenvolver ainda mais a solução a partir da criação de um algoritmo que possa prever se um usuário fará o download de um aplicativo depois de clicar em um anúncio de aplicativo para dispositivos móveis.

Caso você queira saber um pouco mais sobre a TalkingData, podes acessar o site da empresa clicando [aqui](https://www.talkingdata.com/).