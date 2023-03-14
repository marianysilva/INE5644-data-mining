[![](https://img.shields.io/badge/IBM%20Cloud-powered-blue.svg)](https://cloud.ibm.com)
[![](https://img.shields.io/discord/734849242153222221?logo=discord)](https://discord.gg/yJYmTGDWKH)

# Desafio 01 | Bantotal

- [1. Sobre a Bantotal](#1-sobre-a-bantotal)
  - [1.1. Introdução](#11-introdução)
- [2. Desafio de negócio](#2-desafio-de-negócio)
- [3. Objetivo](#3-objetivo)
- [4. Tecnologias aplicadas](#4-tecnologias-aplicadas)
- [5. Desenvolvimento da solução](#5-desenvolvimento-da-solução)
  - [5.1. Resumo das tarefas](#52-resumo-das-tarefas)
  - [5.2. Desenvolvimento](#53-desenvolvimento)

## Para te ajudar

- [Material de Apoio](#material-de-apoio)

## 1. Sobre a Bantotal

### 1.1. Introdução

Bantotal é a plataforma bancária líder na América Latina, que resolve as operações de
missão crítica das Instituições Financeiras de forma simples e precisa.

A plataforma bancária Bantotal entrou no mercado em 1991 e tornou-se líder na
América Latina. Sua sede se encontra no Uruguai.

### 1.2 Contexto atual

#### Pesquisa indica alta no crescimento de crédito em 2022
- O Volume de empréstimos pessoais contratados por brasileiros teve um aumento de quase 20% em 2021
- O Banco Central (BC) divulgou dados que mostram que os empréstimos feitos por instituições financeiras no Brasil chegaram a R$ 4,711 trilhões, em fevereiro de 2022, com alta de 0,8% em relação a janeiro de 2022.

## 2. Desafio de negócio

Cada vez que um cliente solicita um empréstimo a uma instituição financeira, diversos processos e controles internos são acionados, necessários para a avaliação da solicitação recebida. Desta forma, são analisadas manualmente muitas informações relacionadas com o perfil do cliente, destinos de crédito, atividade de trabalho, rendimentos, condições de habitação, entre outros dados demográficos. Além disso, a instituição utiliza os chamados bureaus de crédito para conhecer o histórico de crédito do cliente, a fim de definir o perfil de crédito do cliente. Em conjunto com outros registros próprios, informações de outros créditos, grau de conformidade e comportamento dos produtos contratados, a instituição aprova um valor a ser emprestado e um prazo para sua devolução ou rejeita a solicitação.

## 3. Objetivo

Realizar uma análise de risco para predizer se um empréstimo a um cliente deve ser feito ou não com objetivo de diminuir prejuizos financeiros devido inadimplencia. 

## 4. Tecnologias aplicadas

Espera-se a utilização de um modelo de Machine Learning capaz de realizar uma classificação. O modelo pode ser desenvolvido usando Jupyter Notebooks. O modelo deverá ser treinado com os conjuntos de dados disponibilizado nesse repositório, contendo dados de clientes de bancos, como dados demográficos, sobre suas contas e sobre o empréstimo que querem realizar.

O uso da linguagem [Python](https://www.python.org/), com [Jupyter Notebooks](https://jupyter.org/).

## 5. Desenvolvimento da solução

### 5.1. Resumo das Tarefas

1. Criar um Jupyter Notebook
2. Importar [os dados do problema](../assets/data);
3. Ler e executar as instruções contidas no [Jupyter Notebook](../notebooks);
4. Alterar, validar e testar o seu modelo de Machine Learning, até estar satisfeito com o resultado;
5. Efetuar a submissão para avaliação na disciplina.

### 5.3. Desenvolvimento

O desafio consiste na elaboração de um modelo de Machine Learning para predição de risco de empréstimo, baseado em informações bancárias. Você deverá explorar os dados, tratá-los, e construir o modelo para predição.

O modelo deve receber como entrada os seguintes dados:

```python
[
  "ID", # Número de identificação do cliente
  "CHECKING_BALANCE", # Saldo em conta corrente do cliente
  "PAYMENT_TERM", # Número de dias que o cliente tem para pagar o empréstimo
  "CREDIT_HISTORY", # Como está a situação de crédito passada do cliente
  "LOAN_PURPOSE", # Motivação do empréstimo
  "LOAN_AMOUNT", # Valor do empréstimo
  "EXISTING_SAVINGS", # Saldo de conta poupança
  "EMPLOYMENT_DURATION", # Quantos anos o cliente está no último emprego
  "INSTALLMENT_PERCENT", # Em quantas parcelas o empréstimo deve ser pago
  "SEX", # Sexo
  "OTHERS_ON_LOAN", # Se existe um fiador ou outro aplicante para o empréstimo
  "CURRENT_RESIDENCE_DURATION", # Anos em que o cliente está vivendo na última casa
  "PROPERTY", # Se o cliente possui alguma propriedade em nome
  "AGE", # Idade
  "INSTALLMENT_PLANS", # Plano de financiamento, podendo ser do banco, externo, ou nenhum
  "HOUSING", # Tem casa própria ou não
  "EXISTING_CREDITS_COUNT", # Número de empréstimos que o cliente já tem
  "JOB_TYPE", # Tipo de emprego: 0 - desempregado, 1 - Não qualificado, 2 - Autônomo, 3 - Qualificado
  "DEPENDENTS", # Número de pessoas com acesso à conta
  "TELEPHONE", # Se o cliente tem telefone cadastrado ou não
  "FOREIGN_WORKER" # Se o cliente trabalha num país externo ao do banco ou não
]
```

E como saída um valor binário que representa se o empréstimo deve ser permitido ou não (0 para não, 1 para sim).

**Atenção**: os dados disponibilizados neste desafio são fictícios, qualquer correlação com a realidade é mera coincidência.

Você pode executar o [Notebook](../notebooks/notebook.ipynb) no seu ambiente de desenvolvimento.

## Material de apoio

- [Documentação do Watson Machine Learning](https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/ml-overview.html)
- [Assuma o controle dos seus dados com o Watson Studio](https://developer.ibm.com/br/articles/overview-e-summary-ibm-watson-studio/)
- [Introdução ao IBM Watson Studio](https://developer.ibm.com/br/articles/introduction-to-ibm-watson-studio/)
- [Introdução ao IBM Cloud Pak for Data](https://developer.ibm.com/br/articles/get-started-with-ibm-cloud-pak-for-data/)
- [Desenvolva modelos de aprendizado de máquina com e sem AutoML](https://developer.ibm.com/br/articles/compare-model-building-with-and-without-automated-machine-learning/)
- [Técnicas de Modelagem Preditiva](https://developer.ibm.com/br/articles/ba-predictive-analytics2/)
- [Desenvolva um modelo preditivo de aprendizado de máquina de forma rápida e fácil com o IBM SPSS Modeler](https://developer.ibm.com/br/tutorials/desenvolva-um-modelo-preditivo-de-aprendizado-de-mquina-de-forma-rpida-e-fcil-com-o-ibm-spss-modeler/)
- [Resolva um problema de negócios e preveja uma inadimplência de empréstimo usando um conjunto de dados de risco de crédito alemão](https://developer.ibm.com/br/patterns/resolva-um-problema-de-negcios-e-preveja-uma-inadimplncia-de-emprstimo-usando-um-conjunto-de-dados-de-risco-de-crdito-alemo/)
- [Visualizar dados com Python ](https://developer.ibm.com/br/patterns/visualize-data-with-python/)
- [Crie um indicador de previsões do mercado de ações](https://developer.ibm.com/br/patterns/predicting-the-stock-market-in-watson-studio/)
- [Gere um notebook Python para modelos de pipeline usando AutoAI](https://developer.ibm.com/br/patterns/autoai-code-generation/)
- [Crie fluxos para analisar e prever dados em tempo real](https://developer.ibm.com/br/patterns/live-streaming-of-iot-data-predictions-using-streaming-analytics/)
- [Crie uma solução preditiva](https://developer.ibm.com/br/articles/ba-predictive-analytics3/)
- [Use uma solução preditiva](https://developer.ibm.com/br/articles/ba-predictive-analytics4/)
- [O que é Análise Preditiva?](https://developer.ibm.com/br/articles/ba-predictive-analytics1/)

Você também pode acessar o Discord oficial da Maratona 2021 para realizar perguntas e/ou interagir com outros participantes: [Discord](https://discord.gg/yJYmTGDWKH).

## License

Copyright 2021 Maratona Behind the Code

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
