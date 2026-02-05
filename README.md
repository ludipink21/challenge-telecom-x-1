  #  Projeto Challenge-Telecom-X-1 
# Análise de Churn (ETL & EDA)
        
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-blue?style=for-the-badge&logo=python&logoColor=white)

Este projeto foi desenvolvido como um desafio de análise de dados para a empresa fictícia **Telecom X**. O objetivo principal foi realizar o processo de ETL (Extração, Transformação e Carga) e uma Análise Exploratória de Dados (EDA) para entender os motivos da alta evasão de clientes (Churn).

##  Objetivo do Projeto
Transformar dados brutos (JSON) em insights estratégicos para ajudar a equipe de Data Science a reduzir o índice de cancelamentos, que atualmente impacta o faturamento da empresa.



##  Etapas do Pipeline (ETL)

### 1. Extração (Extract)
* Coleta de dados brutos via API em formato JSON.
* Utilização da biblioteca `requests` para acesso ao repositório remoto.

### 2. Transformação (Transform)
* **Desaninhamento (Flattening):** Conversão de objetos JSON complexos em um DataFrame estruturado.
* **Limpeza:** Remoção de registros com valores nulos ou vazios na coluna alvo `Churn`.
* **Tipagem:** Conversão de colunas numéricas (como `Total Charges`) que estavam formatadas como texto.

### 3. Análise Exploratória (EDA)
* Cálculo da taxa de Churn geral da base.
* Visualização de correlação entre o **Tipo de Contrato** e a **Evasão**.



##  Principais Insights
* **Taxa de Churn:** 26.54% dos clientes cancelaram o serviço.
* **Fator Crítico:** Clientes com contrato **mês a mês** representam a grande maioria das evasões.
* **Fidelidade:** Clientes em contratos de 1 ou 2 anos possuem uma taxa de retenção drasticamente superior.

##  Como Executar
1. Clone o repositório.
2. Certifique-se de ter o `pandas`, `seaborn` e `matplotlib` instalados.
3. Execute o arquivo Jupyter Notebook ou cole o código no Google Colab.

Desenvolvido porLudimila Rodrigues  durante o desafio de análise de dados.
