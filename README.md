🌱 Agrofit Case
  Projeto de análise de dados do Agrofit com foco em exploração, tratamento, modelagem e visualização de dados do mercado de defensivos agrícolas.

📌 Objetivo
  Este projeto tem como objetivo analisar dados de produtos formulados registrados no Agrofit, gerando insights estratégicos sobre:
  
  Empresas e titulares
  Produtos e categorias
  Relação produto × pragas
  Panorama do mercado de defensivos agrícolas

📂 Estrutura do Projeto
  agrofit-case/
  │
  ├── data/
  │   ├── bruto/
  │   │   └── agrofitprodutosformulados.csv
  │   │
  │   └── tratado/
  │       ├── agrofit_limpo.csv
  │       ├── dim_empresa.csv
  │       ├── dim_produto.csv
  │       ├── dim_titular.csv
  │       └── fato_produto_praga.csv
  │
  ├── power bi/
  │   ├── AgrofitCase.pbix
  │   └── backgrounds/
  │
  ├── src/
  │   ├── 01_eda.ipynb
  │   ├── 02_limpeza_padronizacao.ipynb
  │   ├── 03_enriquecimento.ipynb
  │   └── 04_visualizacao.ipynb
  │
  └── README.md

🔄 Pipeline do Projeto

O projeto segue uma pipeline clássica de dados:

1. 📊 Análise Exploratória (EDA)

  Notebook: 01_eda.ipynb
  
  Entendimento inicial dos dados
  Identificação de inconsistências
  Análise de distribuição e padrões
  2. 🧹 Limpeza e Padronização
  
  Notebook: 02_limpeza_padronizacao.ipynb
  
  Tratamento de valores nulos
  Padronização de textos
  Normalização de campos
  3. 🧠 Enriquecimento dos Dados
  
  Notebook: 03_enriquecimento.ipynb
  
  Criação de dimensões analíticas:
  Empresas
  Produtos
  Titulares
  Construção de tabelas fato
  4. 📈 Visualização
  
  Notebook: 04_visualizacao.ipynb
  
  Geração de gráficos e insights
  Apoio para construção do dashboard
  📊 Modelagem de Dados
  
  O projeto utiliza um modelo dimensional (estilo Star Schema):
  
  Dimensões:
  dim_empresa
  dim_produto
  dim_titular
  Fato:
  fato_produto_praga
  📉 Dashboard (Power BI)
  
  Arquivo: power bi/AgrofitCase.pbix
  
  O dashboard apresenta:
  
  Visão geral do mercado
  Análises estratégicas
  Insights sobre produtos e empresas
  Relação entre produtos e pragas
  🛠️ Tecnologias Utilizadas
  Python (Pandas, NumPy, Matplotlib/Seaborn)
  Jupyter Notebook
  Power BI
  CSV como fonte de dados

▶️ Como Executar
 1. Clone o repositório:
    git clone <repo-url>
    cd agrofit-case

2.Instale as dependências:
  pip install pandas numpy matplotlib seaborn jupyter

3.Execute os notebooks na ordem:
  01 → 02 → 03 → 04

4.Abra o dashboard no Power BI:
  power bi/AgrofitCase.pbix

💡 Possíveis Melhorias
  Automatização do pipeline (ETL)
  Integração com banco de dados
  Deploy de dashboard online
  Criação de API para consulta dos dados
  Uso de ferramentas como Airflow ou dbt
  
