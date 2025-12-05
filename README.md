# 📓 Pipeline ELT - Análise do Cenário das Mulheres na Tecnologia

Este projeto apresenta um pipeline ELT(Extract, Load, Transform), criado para reunir e analisar dados sobre a presença das mulheres no mercado global de tecnologia.

Desenvolvido para o Desafio de Dados da WoMakersCode, este pipeline integra múltiplas fontes de dados e emprega ferramentas de transformação e orquestração para simular um ambiente real de engenharia de dados, com o objetivo de gerar insights sobre a atuação feminina no mercado de tecnologia.

---
## 🛠 Tecnologias Utilizadas

- **Python** - Linguagem principal do projeto  
- **Pandas** - Manipulação, limpeza e tratamento inicial dos dados  
- **SQLite** - Data Warehouse local para armazenamento na camada *Raw*  
- **dbt** - Transformações, padronização e modelagem dos dados (*Staging* e *Data Mart*)  
- **Prefect** - Orquestração e monitoramento do fluxo ELT  
- **Logging** - Registro de eventos e erros da pipeline  
- **Requests** - Consumo de APIs externas  
- **Microsoft Power BI** - Construção do dashboard analítico final  
---
## 📂 Fontes de Dados

- **CSV** – Kaggle Survey 2022, filtrada exclusivamente para participantes do gênero feminino  
- **API REST** – REST Countries, com dados geográficos e demográficos  
- **SQL** – Base fictícia com informações de participantes do Bootcamp  
- **JSON** – Arquivo com habilidades categorizadas por área de atuação  
---

## 🏗 Arquitetura do Projeto

1. Extração e Carga – Python
- Coleta e ingestão de dados em múltiplos formatos (CSV, API REST, banco SQL e JSON).

2. Data Warehouse – SQLite
- Armazenamento dos dados brutos na camada **Raw Data**.

3. Transformação – dbt
- Processos de limpeza, padronização e modelagem.  
- Estruturação das camadas:
  - **Staging**
  - **Data Mart**

4. Orquestração – Prefect
- Automação do fluxo ELT com monitoramento e tolerância a falhas.

5. Visualização – Power BI
- Dashboard final contendo as análises.
---
## 🚀 Como Executar o Projeto

O notebook foi desenvolvido para rodar com facilidade no Google Colab, onde toda a estrutura necessária é criada automaticamente.

✔️ Requisitos

  - Conta Google
  
  - Acesso ao Colab

📌 Instruções

  - Abra ou envie o arquivo .ipynb para o Google Colab.

  - Execute a primeira célula para instalar as dependências:

        !pip install pandas prefect dbt-sqlite requests

  - Siga a ordem das células, que incluem:

    - Configurações iniciais
    
    - Funções de extração
    
    - Criação do projeto e modelos dbt
    
    - Execução do fluxo orquestrado pelo Prefect

## 📊 Dashboard Interativo

<img width="1013" height="564" alt="image" src="https://github.com/user-attachments/assets/9d1a2e86-31a9-4f3b-b51d-49cb94cd4ffd" />


## Perguntas de Negócio Respondidas

Com a modelagem final (dim_desenvolvedoras), é possível investigar:
  - Quantidade de mulheres participantes da Pesquisa do Kaggle em 2022
  - Média salarial (em dólares) por anos de experiência
  - Bancos de dados mais utilizados
  - Utilização das principais linguagens de dados (Python, SQL e R)
  - Quantidade de mulheres do Brasil e das Américas
--- 
✒️ Autores

WoMakersCode 


Tandara Jesus dos Santos

---
📘Projeto criado para fins educacionais.
