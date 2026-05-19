# 🏅 Data Science: Bolsa Atleta & O Cenário de Infraestrutura Esportiva e Educacional no Brasil
## 📌 1. Definição do Problema e Objetivos
O fomento ao esporte de alto rendimento no Brasil tem como principal pilar o Programa Bolsa Atleta. Contudo, o desenvolvimento de novos talentos e o acesso à prática esportiva dependem diretamente da base educacional e da infraestrutura disponível nas instituições de ensino.

Este projeto tem como objetivo cruzar e analisar os dados de concessão do Bolsa Atleta com os indicadores de infraestrutura esportiva das escolas brasileiras (Censo Escolar), respondendo a três perguntas de negócio centrais:

Gargalo de Origem: Existe correlação entre as regiões/estados com maior número de beneficiários do Bolsa Atleta e aqueles com melhor infraestrutura esportiva nas escolas públicas e privadas?

Desigualdade no Estímulo: Como as categorias "Estudantil" e "Base" do benefício estão distribuídas em relação ao IDH e à presença de quadras cobertas, laboratórios e pistas de atletismo nos municípios?

Modelagem Preditiva: É possível predizer o volume de atletas de alto rendimento que um município gerará no futuro com base exclusivamente nos seus indicadores de investimento em educação e infraestrutura escolar atual?

## 🛠 2. Tecnologias, Bibliotecas e Fontes de Dados
### Fontes de Dados Utilizadas
Dados Abertos do Ministério do Esporte: Microdados dos contemplados pelo Programa Bolsa Atleta (2020-2026).

INEP / Censo Escolar: Infraestrutura das escolas de educação básica (presença de quadras esportivas, piscinas, salas de dança, etc.).

IBGE: Dados socioeconômicos dos municípios (PIB per capita, população e IDH).

### Stack Técnica
Plaintext
📦 projeto-bolsa-atleta
 ├── Python (Linguagem Principal)
 ├── Pandas & NumPy (Manipulação e Engenharia de Dados)
 ├── Geopandas (Análise Espacial e Mapas de Calor)
 ├── Matplotlib & Seaborn (Visualização Estatística)
 ├── Scikit-Learn (Modelagem Preditiva e Clusterização)
 └── XGBoost / LightGBM (Modelos de Regressão Avançados)
## 🧬 3. Etapas do Processo Analítico
### Fase 1: Integração e Limpeza de Dados (ETL)
Pipeline de Junção: Consolidação de múltiplas saídas anuais do Bolsa Atleta e agrupamento por município através do código IBGE de 7 dígitos.

Tratamento de Dados: Tratamento de valores ausentes (ex: preenchimento de dados de infraestrutura via moda regional) e padronização de nomes de modalidades esportivas.

Engenharia de Features: Criação de taxas normalizadas por 100 mil habitantes (ex: bolsistas_por_100k_hab) para evitar o viés populacional de grandes metrópoles.

### Fase 2: Análise Exploratória de Dados (EDA)
Principais descobertas visuais e estatísticas extraídas durante o processo:

O Limiar da Base: O Censo Escolar aponta que menos de 46% das escolas públicas de educação básica no Brasil possuem quadras esportivas adequadas.

Concentração Regional: Existe uma forte assimetria na categoria Atleta Pódio, fortemente concentrada em estados do Sul e Sudeste, que por sua vez apresentam os maiores percentuais de escolas com infraestrutura de ponta (piscinas, ginásios cobertos).

### Fase 3: Modelagem Preditiva & Clusterização
Para segmentar os cenários brasileiros e prever o sucesso esportivo, foram aplicadas duas abordagens de Machine Learning:

Clusterização (Unsupervised K-Means): Agrupamento dos municípios brasileiros em 4 perfis distintos com base em suas condições escolares estruturais e IDH, identificando "desertos de infraestrutura esportiva".

Regressão (Supervised): Criação de um modelo preditivo para estimar a quantidade de novos bolsistas nacionais/internacionais de uma região. Avaliado utilizando métricas robustas:

RMSE (Root Mean Squared Error): Medição da magnitude do erro das previsões.

R² Score: Percentual da variância dos dados explicado pelas variáveis educacionais.

## 📂 4. Estrutura do Repositório
Organização estrutural para replicação imediata do projeto:

Plaintext
├── data/                  # Armazenamento dos datasets originais (Links/Instruções)
│   ├── raw/               # Dados brutos baixados das fontes oficiais
│   └── processed/         # Dados limpos e unificados prontos para modelagem
├── notebooks/             # Jupyter Notebooks organizados por ordem cronológica
│   ├── 01_data_cleaning.ipynb
│   ├── 02_exploratory_analysis.ipynb
│   └── 03_predictive_modeling.ipynb
├── src/                   # Códigos e scripts de produção (.py)
│   ├── data_pipeline.py
│   └── utils.py
├── README.md              # Documentação principal do projeto
└── requirements.txt       # Dependências e bibliotecas do projeto para instalação
## 🚀 5. Como Executar Este Projeto
Para rodar o pipeline completo em sua máquina local, siga a ordem das tarefas abaixo:

## 📢 6. Conclusões e Insights para Políticas Públicas
Os resultados do modelo apontam que a infraestrutura escolar básica atua como o principal funil para o esporte de alto rendimento no Brasil. Investimentos direcionados à cobertura e reforma de quadras em municípios de vulnerabilidade social apresentam alto potencial de retorno na quantidade de atletas integrando as categorias de base e estudantil em um horizonte de 4 anos, gerando impacto direto no desenvolvimento social e na representatividade esportiva do país.

Desenvolvido por: [Seu Nome]

Contato: [seu-email@provedor.com]

LinkedIn: linkedin.com/in/seu-perfil
