# Projeto de Análise de Dados - Dengue no Brasil

## Objetivo

Este projeto tem como objetivo analisar a evolução dos casos de dengue no Brasil utilizando técnicas de Análise Exploratória de Dados (EDA). A partir de dados públicos, busca-se identificar padrões temporais e geográficos, contribuindo para a compreensão da distribuição da doença e demonstrando como a análise de dados pode auxiliar na tomada de decisões na área da saúde pública.

---

## Problema

A dengue representa um importante problema de saúde pública no Brasil, causando milhares de casos todos os anos e impactando diretamente a população e o sistema de saúde.

Por meio da análise de dados é possível identificar os estados mais afetados, os períodos com maior incidência da doença e padrões temporais que auxiliam na definição de estratégias de prevenção e combate à dengue.

---

## Fonte dos Dados

Os dados utilizados neste projeto foram obtidos na plataforma **Kaggle**, por meio do conjunto de dados **DENGUE BRASIL**, disponibilizado pelo autor **AI_ML_TSF**.

**Informações da base:**

- Plataforma: Kaggle
- Conjunto de dados: DENGUE BRASIL
- Autor: AI_ML_TSF
- Arquivo utilizado: dengue_brazil.csv
- Período dos dados: 2000 a 2019
- Formato: CSV
- Tipo dos dados: Estruturados
- Método de coleta: Download direto da plataforma Kaggle

Link da base de dados:

https://www.kaggle.com/datasets/ai-ml-tsf/dengue-brasil

Período analisado: janeiro de 2000 a dezembro de 2019.

Os dados apresentam registros mensais de casos de dengue para os estados brasileiros, permitindo análises temporais e comparações entre diferentes regiões do país.
---

## Coleta dos Dados

O conjunto de dados foi obtido por download direto da plataforma Kaggle em formato CSV. Posteriormente, o arquivo foi importado para o Google Colab utilizando a biblioteca Pandas para realização da análise exploratória.

---

## Tratamento e Modelagem

Durante o tratamento dos dados foram realizadas as seguintes etapas:

- Importação da base de dados;
- Verificação de valores nulos;
- Estatísticas descritivas;
- Transformação da base utilizando a função `melt()`, convertendo o formato largo para formato longo;
- Conversão da coluna de datas para o tipo `datetime`;
- Criação da coluna **ano** para facilitar as análises temporais.

Após essas etapas foi gerado o arquivo **dengue_tratado.csv**, utilizado no dashboard do Looker Studio.

---

## Análise Exploratória (EDA)

Durante a análise exploratória foram desenvolvidas as seguintes análises:

- Total de casos por estado;
- Média de casos por estado;
- Evolução temporal dos casos;
- Percentual dos estados com maior número de registros;
- Comparação entre estados com maior e menor incidência.

---

## Principais Insights

A análise permitiu identificar importantes padrões relacionados aos casos de dengue no Brasil.

- São Paulo apresentou o maior número de casos registrados, com **2.535.416 casos**.
- Minas Gerais ficou em segundo lugar, com **2.285.503 casos**.
- Rio de Janeiro ocupou a terceira posição, com **1.412.425 casos**.

Os três estados representam aproximadamente:

- São Paulo: **19,66%**
- Minas Gerais: **17,72%**
- Rio de Janeiro: **10,95%**

dos casos registrados na base de dados.

Também foi identificado que:

- O ano de **2015** apresentou o maior número de casos (**1.700.248 registros**);
- Em seguida aparecem **2019** e **2016**, demonstrando períodos epidêmicos importantes.

Por outro lado, os menores números de casos ocorreram em:

- Rio Grande do Sul
- Santa Catarina
- Roraima
- Amapá

Esses resultados demonstram diferenças importantes na distribuição geográfica da doença.

---

## Dashboard

O dashboard foi desenvolvido utilizando o **Google Looker Studio**.

O painel apresenta:

- Indicadores gerais;
- Ranking dos estados com maior número de casos;
- Evolução temporal dos registros;
- Distribuição percentual por estado.

---

## Tecnologias Utilizadas

- Python
- Pandas
- Matplotlib
- Google Colab
- Google Looker Studio
- GitHub

---

## Conclusão

A análise exploratória permitiu identificar diferenças significativas na incidência da dengue entre os estados brasileiros durante o período de 2000 a 2019.

São Paulo apresentou o maior número de casos registrados (2.535.416), seguido por Minas Gerais (2.285.503) e Rio de Janeiro (1.412.425). Juntos, esses três estados concentram aproximadamente **48,33%** de todos os casos registrados na base de dados, demonstrando uma forte concentração da doença em determinadas regiões do país.

Também foi observado que o ano de **2015** registrou o maior número de casos (1.700.248), seguido por **2019** e **2016**, indicando períodos epidêmicos mais intensos. Em contrapartida, estados como Rio Grande do Sul e Santa Catarina apresentaram os menores registros durante o período analisado.

Esses resultados mostram que a análise de dados é uma ferramenta essencial para identificar regiões prioritárias, acompanhar a evolução da doença ao longo do tempo e subsidiar políticas públicas voltadas ao combate da dengue. A utilização de técnicas de análise exploratória permite transformar dados em informações úteis para apoiar a tomada de decisões baseada em evidências.

Os resultados demonstram que a utilização de técnicas de análise de dados pode contribuir para o planejamento de políticas públicas, distribuição de recursos e definição de estratégias de prevenção da doença.

Além disso, o projeto evidenciou a importância da preparação, transformação e visualização dos dados para apoiar a tomada de decisões baseada em evidências.
