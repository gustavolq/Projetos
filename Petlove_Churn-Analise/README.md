# **Análise de Churn - PetLove**

## **1. Introdução**
Esse repositório se refere à etapa de *Business Case* do processo seletivo para a área de dados da empresa Petlove&CO.

A Petlove&CO é a maior plataforma voltada para animais de estimação da América Latina e o papel da empresa é cuidar de toda a experiência do animal de estimação, incluindo a cadeia de suprimentos (Petlove), cuidados de saúde (Vet Smart), gestão empresarial (ERP por Vetus) e cuidados diários (DogHero).

O desafio proposto pela Petlove&CO é nos inserir na equipe de Assinatura, um serviço onde o dono do animal programa a entrega de um conjunto de itens dentro de um período customizado, recebendo descontos e brindes exclusivos para assinantes.

Ao analisar os dados dos últimos meses, apesar das melhorias de usabilidade da plataforma, foi verificado que o Churn (perda de usuário que assinou o serviço de assinatura e o cancelou em algum momento) vem aumentando.

O objetivo da equipe de assinaturas é reduzir a perda de assinantes, ou seja, a diminuição da taxa de churn.

O trabalho será apresentar um resultado final com dois pontos principais :
- **Quais são os aprendizados da análise dos dados?**
- **O que pode ser sugerido para os próximos passos?**

## **2. Sobre os arquivos**
- [analise.ipynb](notebooks/analise.ipynb) = Notebook com a análise + códigos.
- [apresentacao.ipynb](reports/apresentacao.ipynb) = Notebook utilizado para gerar o arquivo [apresentacao.html](reports/apresentacao.html).
- [apresentacao.html](reports/apresentacao.html) = Arquivo HTML com a análise e conclusões.
- [data/data-test-analytics.csv](data/data-test-analytics.csv) = Dados utilizados para a análise.
- [requirements.txt](requirements.txt) = Pacotes utilizados para criar o ambiente virtual Python.

## **3. Instruções para execução local**

### **Instalação do Python**
Para a instalação do Python, basta realizar a instalação do [Anaconda](https://www.anaconda.com/download/) e não esquecer de adicionar o diretório como variável de ambiente.

### **Preparação do ambiente Python**
Com o anaconda instalado, podemos criar um novo ambiente Python, também chamado de ambiente virtual, com o seguinte comando :

```
conda create --name petlove_case --file requirements.txt
```

Esse comando irá realizar a criação do ambiente virtual e a instalação dos pacotes utilizados no projeto, que estão no arquivo [requirements.txt](requirements.txt).

Com isso, você pode realizar a ativação do ambiente virtual com o comando abaixo :

```
conda activate petlove_case
```

E após isso, utilizar o jupyter ou o vscode para verificar a análise do projeto.

## **4. Sobre os Dados**
Os dados foram disponibilizados pela equipe de Engenharia de Dados e estão disponíveis no arquivo [data-test-analytics.csv](data/data-test-analytics.csv).

As informações disponibilizadas no arquivo e a sua descrição são as seguintes:

|Column|Description|
|---|---|
|id|Identificação do cliente|
|created_at|Data de criação da assinatura|
|updated_at|Data da última modificação da assinatura|
|deleted_at|Data de cancelamento da assinatura|
|name_hash|Nome do usuário (criptografado)|
|email_hash|Email do usuário (criptografado)|
|address_hash|Endereço do usuário (criptografado)|
|birth_date|Data de aniversário do cliente|
|status|Status da assinatura|
|version|Versão da assinatura|
|city|Cidade do cliente|
|state|Estado do cliente|
|neighborhood|Bairro do cliente|
|last_date_purchase|Data do último pedido que ocorreu pela assinatura|
|average_ticket|Média de gasto por pedido|
|items_quantity|Média de itens na assinatura|
|all_revenue|Total de receita realizado pelo cliente|
|all_orders|Total de pedidos realizados pelo cliente|
|recency|Tempo desde a última compra do cliente|
|marketing_source|Canal de marketing que converteu a assinatura|

## **5. Resumo da Análise**
Identificamos em nossa análise que clientes provenientes dos canais de marketing Telegram / Whatsapp possui um valor muito próximo de aquisição de clientes (1068) em relação à CRM (1029), porém, possui uma taxa de cancelamentos de 6.18% (segunda maior taxa), contra 4.18% (menor taxa).

Além disso, podemos perceber que existem clientes que estão sendo captados a partir de um canal chamado "None", o que pode ser um erro na captação de dados, e possui a maior taxa de cancelamentos com 6.43%.

Já o canal de marketing Organic Search é o que mais realiza a captação de clientes com 36,99% de clientes vindo desse canal.

Com a análise de regiões e estados, identificamos que a quantidade de clientes por região da amostra de dados é proporcional à quantidade de estados de cada região, o que resulta em uma ordem para maiores clientes em : Nordeste, Norte, Centro-Oeste, Sudeste e Sul.

Algo interessante identificado é que possuem uma alta taxa de cancelamento (5.33%) para Centro-Oeste quando comparado ao Sudeste (4.33%) mesmo com uma quantidade total de clientes muito próxima, mas, talvez isso possa ser explicado pela presença de mais empresas da Petlove na região Sudeste.

Tendo uma visão mais "micro", conseguimos identificar cidades da mesma região que possuem uma taxa de cancelamento muito diferente, por exemplo, Rio Grande do Sul (6.54%) e Santa Catarina (3.24%).

Realizando a análise de dados numéricos, foi possível identificar que a maior quantidade de clientes acaba cancelando a assinatura após 0-49 dias com a assinatura ativa, sendo 62 clientes que representam 12% da amostra fornecida. Também é importante ressaltar que 50% dos cancelamentos ocorreram antes de 322 dias (aproximadamente 10 meses).

A partir da receita realizada pelo cliente, foi identificado uma leve diferença entre os grupos que estão com a assinatura ativa ou pausada (50% dos valores estão em 1.182,818) em relação aos cancelados (50% dos valores estão abaixo de 984,35), mas essa diferença pode ser explicada devido ao tempo que o cliente ficou com a assinatura ativa.

Observando a quantidade de dias desde a última compra do cliente chegamos à identificar que 161 clientes (31% da amostra de dados cancelados) realizaram o cancelamento da assinatura após ficarem de 0 à 49 dias sem realizar uma compra.