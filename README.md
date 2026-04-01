Analise SuperStore
Análise exploratória (EDA) do dataset Sample – Superstore, com foco em vendas e lucro, usando Python, Pandas e visualizações com Matplotlib/Seaborn. O projeto está implementado no notebook: notebook/analise.ipynb.

Objetivo
Investigar o comportamento de Sales (Vendas) e Profit (Lucro) no Superstore e responder perguntas como:

Quais categorias vendem mais?
Qual região é mais lucrativa?
Quais cidades geram mais lucro?
Qual o perfil de clientes por segmento?
Tecnologias e bibliotecas
Python (notebook Jupyter)
pandas
matplotlib.pyplot
seaborn
Dataset
O notebook carrega um CSV em:

txt
data/Sample - Superstore.csv
O dataset possui 9.994 linhas e 21 colunas, incluindo (principais):

Order Date, Ship Date, Ship Mode
Customer Name, Segment
City, State, Region, Postal Code
Category, Sub-Category, Product Name
Sales, Quantity, Discount, Profit
Observação: o notebook lê o CSV com encoding='latin1'.

O que é analisado no notebook
Carga e inspeção dos dados

Leitura do CSV com Pandas
head() para visualizar amostras
info() para tipos e consistência
Vendas por Categoria

Agrupamento por Category somando Sales
Gráfico de barras: “Categoria de Produto Mais Vendida”
Lucro por Região

Agrupamento por Region somando Profit
Gráfico de barras: “Lucro por Região”
Top 5 Cidades com maior lucro

Agrupamento por City somando Profit
nlargest(5) para selecionar as líderes
Gráfico de barras: “Lucro por Cidade”
Distribuição de clientes por Segmento

Segment.value_counts()
Gráfico de pizza: “Clientes que mais compraram” (distribuição por segmento)
Como executar
1) Clonar o repositório
bash
git clone https://github.com/DanielSydinei/Analise-SuperStore.git
cd Analise-SuperStore
2) Criar ambiente (opcional, recomendado)
bash
python -m venv .venv
# Windows
.venv\Scripts\activate
# Linux/Mac
source .venv/bin/activate
3) Instalar dependências
bash
pip install pandas matplotlib seaborn jupyter
4) Garantir o dataset no caminho correto
Verifique se o arquivo existe em:

txt
data/Sample - Superstore.csv
5) Rodar o notebook
bash
jupyter notebook
Abra notebook/analise.ipynb e execute as células.


