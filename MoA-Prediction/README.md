# <p align="center"> 🎲 Bem-vindo ao repositório do projeto MoA Prediction 🎲

[![author](https://img.shields.io/badge/author-gustavolq-blue.svg)](https://www.linkedin.com/in/gustavoquadra/)

Olá! Nesse repositório você irá encontrar o meu projeto final realizado na Imersão de Dados 2021 da Alura. 

- data : Arquivos utilizados como nossa base de dados.
- notebooks : Notebook do projeto realizado

Seja bem-vindo e fique à vontade para interagir!

## Mas Gustavo, o que é a Imersão de Dados da Alura? 🤔
A Imersão de Dados da Alura é um evento organizado pela [Alura](https://www.alura.com.br/), uma plataforma de cursos para diversas áreas dentro da Ciência da Computação, realizado anualmente, sendo essa a terceira edição, voltado para a área de [Ciência de Dados](https://pt.wikipedia.org/wiki/Ci%C3%AAncia_de_dados).

A Imersão de Dados da Alura 2021 ocorreu entre os dias 03/05 e 07/05 e possuiu os seguintes conteúdos :

<b> Aula 01 </b> - Análise de dados, python, pandas e genética.</br>
<b> Aula 02 </b> - Estatísticas, visualização de dados e distribuições. </br>
<b> Aula 03 </b> - Correlações, causalidade e relações entre genes.</br>
<b> Aula 04 </b> - Merge de dados e análise de resultados.</br>
<b> Aula 05 </b> - Storytelling em Data Science.</br>

Para realizar as aulas da Imersão de Dados da Alura, utilizamos o [Google Colaboratory](https://colab.research.google.com/notebooks/intro.ipynb), um serviço de nuvem da Google, onde podemos realizar a criação de Notebooks para realizar a criação de linhas de comandos em Python e textos.

Para finalizar a semana de Imersão de Dados 2021, fomos convidados à realizar um projeto de Ciência de Dados voltado para a área de [Drug Discovery](https://en.wikipedia.org/wiki/Drug_discovery).

Muito feliz em poder compartilhar que esse projeto foi um dos 10 selecionados para ganhar uma bolsa de 100% para a participação no Bootcamp de Ciência de Dados da Alura! 🏆🏆

# <p align="center"> 💻 Sobre o Projeto 💻

<p align="center">
  <img src = "https://mma.prnasia.com/media2/1283775/drug_discovery_pharma_data_science.jpg?p=publish" width = 70%>
</p>

## Introdução
O projeto proposto na Imersão de Dados 2021 foi baseado na competição [Kaggle - Mechanisms of Action (MoA) Prediction](https://www.kaggle.com/c/lish-moa/overview) criado pela [The Connectivity Map](https://clue.io/), um projeto do Broad Institute of MIT e Harvard, do Laboratory for Innovation Science em Harvard (LISH) e da Biblioteca de Fundos Comuns do NIH de assinaturas celulares integradas em rede (LINCS) com o objetivo de avanço no desenvolvimento de medicamentos por meio de melhorias nos algoritmos de previsão do MoA (Mecanismos de Ação).

## Escopo do Projeto

O objetivo do nosso projeto será realizar a previsão da ocorrência ou não de um Mecanismo de Ação (MOA) através da combinação de diferentes experimentos realizados com compostos em culturas celulares, com doses, tratamentos e tempos diferentes. 

Em nossos dados também possuímos os valores de expressões gênicas (processo pelo qual a informação hereditária de um gene, forma uma proteína ou RNA) e viabilidade celular (análise de células em uma cultura celular para verificar a atividade celular) que influenciam na ativação do Mecanismo de Ação (MOA).
 
## Planejamento do Projeto

Para a realização do projeto, seguirei o seguinte planejamento :

<b> 1.</b> Definição do Problema de Negócio </br>
<b> 2.</b> Preparação dos Dados </br>
<b> 3.</b> Análise Exploratória dos Dados </br>
<b> 4.</b> Criação do Modelo de Machine Learning </br>
<b> 5.</b> Otimização do Modelo de Machine Learning </br>
<b> 6.</b> Apresentação do Resultado </br>

## Dados Utilizados no Projeto

Para o projeto, iremos utilizar duas bases de dados, que são :

- dados_experimentos.zip : Dados com os valores de expressão gênica, viabilidade celular, tratamento, dose, tempo para os diferentes experimentos.
- dados_resultados.csv   : Dados com os valores de ativação ou não do Mecanismo de Ação.

# <p align="center"> 💊 Um pouco mais sobre a área de Drug Discovery 💊

A busca por medicamente para o alívio de sintomas e tratamento de doenças talvez seja uma das práticas mais antigas da nossa sociedade, onde acredita-se que a busca por plantas medicinais começou de uma maneira instintiva.

A evidência escrita mais antiga de uso de plantas medicinais tem aproximadamente, 5 mil anos : uma peça de argila escrita em sumério e que tinha 12 receitas com mais de 250 plantas.
Há também o livro chinês “Pen T’Sao”, escrito em 2.500 a.C, que trata de mais de 300 plantas as quais são usadas até hoje na medicina tradicional chinesa.
O conhecimento acumulado que temos hoje sobre quais plantas podem ser venenosas, medicinais ou psicotrópicas se deve à sobrevivência desse conhecimento antigo, que hoje chamamos de “conhecimento tradicional”.

Há também aqueles fármacos que foram descobertos por acaso, como é o caso da Penicilina, descoberta em 1928 por Alexander Fleming. Fleming fazia experimentos com bactérias cultivadas em placas de petri e, sem querer, algumas de suas placas foram contaminadas por fungos. Fleming reparou que as bactérias que estavam próximas dos fungos haviam morrido. Ele então descobriu que o fungo Penicillium rubens tinha propriedades antibióticas. 

Hoje o desenvolvimento de novos fármacos se dá por meio de pesquisas ciêntificas, as quais buscam isolar e purificar compostos de plantas, fungos e microorganismos, elaborar e testar compostos sintéticos ou aprimorar fármacos já conhecidos.

A biotecnologia vem revolucionando a farmacologia. Um exemplo é a insulina, usada no tratamento da diabetes e que antes era extraída de pâncreas de bois e porcos, hoje é extraída de bactérias que produzem a insulina humana por meio da técnica do DNA Recombinante, em que cientistas inseriram o gene humano da insulina no genoma das bactérias. 

No futuro poderemos ter acesso a medicamentos feitos de maneira mais personalizada, de acordo com o genoma e com as características de cada um, conforme os avanços da farmacogenômia. Um exemplo disso foi o medicamento Milasen, desenvolvido especialmente para uma criança com Síndrome de Batten, uma doença rara e de origem genética.

As pesquisas biomédicas estão cada vez mais interdisciplinares e sofisticadas e os dados gerados nesses estudos são cada vez mais volumosos e complexos, tornando a Ciência de Dados essencial no desenvolvimento da farmacologia.