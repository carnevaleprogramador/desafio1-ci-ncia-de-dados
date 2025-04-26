# 📊 Análise de Dados de Vendas de Lojas

## 🛒 Desafio - Alura Store - Análise de Lojas
Este projeto realiza uma análise exploratória de dados de vendas de quatro lojas, utilizando a biblioteca Pandas para manipulação de dados e Matplotlib para visualização. O objetivo é fornecer insights sobre o faturamento, as vendas por categoria, a média de avaliação dos clientes, os produtos mais e menos vendidos e o frete médio de cada loja.

## 🔍 Visão Geral do Projeto
O script Python (`.ipynb`) realiza as seguintes etapas:

1. **Importação de Dados:** Carrega os dados de vendas de cada loja a partir de arquivos CSV hospedados no GitHub.
2. **Análise de Faturamento:** Calcula o faturamento total de cada loja, o faturamento médio e visualiza a distribuição do faturamento entre as lojas através de um gráfico de barras.
3. **Análise de Vendas por Categoria:** Combina os dados de todas as lojas, calcula o faturamento por categoria em cada loja e apresenta essa informação em um gráfico de barras lado a lado.
4. **Análise da Média de Avaliação:** Calcula a média das avaliações de compra para cada loja e exibe essa informação em um gráfico de barras.
5. **Análise de Produtos Mais e Menos Vendidos:** Identifica o produto com maior e menor quantidade vendida em cada loja.
6. **Análise de Frete Médio:** Calcula o custo médio de frete para cada loja.
7. **Análise Geográfica das Vendas:** Utiliza as coordenadas de latitude e longitude apresentadas nos dados para visualizar a distribuição geográfica das vendas, o faturamento por localização e a distribuição das avaliações.

## ⬇️ Instalação
Para executar este projeto, você precisa ter o Python instalado em seu ambiente. Além disso, as seguintes bibliotecas são necessárias:

- **Pandas**: Para manipulação e análise de dados tabulares.
- **Matplotlib**: Para criação de gráficos e visualizações.
- **NumPy**: Embora não seja explicitamente importado no código fornecido, o Matplotlib é frequentemente utilizado internamente para transações numéricas.

Você pode instalar essas bibliotecas usando o pip, ou gerenciador de pacotes do Python. Abra seu terminal ou prompt de comando e execute o seguinte comando:

pip install pandas matplotlib
## 📌 Dependências
As seguintes bibliotecas Python são dependências deste projeto:

pandas (>= 1.0.0): Utilizado para leitura e manipulação dos dados das lojas a partir de arquivos CSV hospedados em URLs.

matplotlib (>= 3.0.0): Empregada para gerar gráficos de barras que visualizam o faturamento por loja, as vendas por categoria e a média de avaliação das lojas.

numpy (>= 1.18.0): Usado internamente pelo Matplotlib para cálculos numéricos, como o cálculo da média de faturamento para a linha de referência no gráfico.

## ⚙️ Execução no Google Colab
O Google Colab é um ambiente Jupyter Notebook hospedado na nuvem que permite executar o código Python sem a necessidade de configuração local. Para executar este projeto no Colab, siga estes passos:

Abra o Google Colab: Acesse https://colab.research.google.com/ no seu navegador.

Crie um novo notebook: Clique em "Novo notebook" no canto inferior direito da tela.

Copie e cole o código: Copie todo o código Python fornecido e cole em uma célula de código no seu notebook do Colab.

Execute como células: Execute como células de código sequencialmente, clicando no botão "play" (executar) ao lado de cada célula ou pressionando Shift + Enter. O Colab já possui as bibliotecas Pandas e Matplotlib pré-instaladas, então você não precisa executar o comando !pip install novamente, a menos que necessite de versões específicas ou outras bibliotecas adicionais.

## 💡 Explicação do Código
O código Python realiza as seguintes etapas de análise:

Importação dos Dados
python
Copiar
Editar
import pandas as pd

url1 = "[URL_DO_ARQUIVO_LOJA_1]"
url2 = "[URL_DO_ARQUIVO_LOJA_2]"
url3 = "[URL_DO_ARQUIVO_LOJA_3]"
url4 = "[URL_DO_ARQUIVO_LOJA_4]"

loja1 = pd.read_csv(url1)
loja2 = pd.read_csv(url2)
loja3 = pd.read_csv(url3)
loja4 = pd.read_csv(url4)

loja1.head()
Análise de Faturamento
python
Copiar
Editar
faturamento_loja1 = loja1['Preço'].sum()
faturamento_loja2 = loja2['Preço'].sum()
faturamento_loja3 = loja3['Preço'].sum()
faturamento_loja4 = loja4['Preço'].sum()

faturamento_total = faturamento_loja1 + faturamento_loja2 + faturamento_loja3 + faturamento_loja4
faturamento_medio = faturamento_total / 4

print(f"Faturamento médio das lojas: R${faturamento_medio:,.2f}")
Análise de Vendas por Categoria
python
Copiar
Editar
vendas_por_categoria_loja1 = loja1.groupby('Categoria do Produto')['Preço'].count()
vendas_por_categoria_loja2 = loja2.groupby('Categoria do Produto')['Preço'].count()
vendas_por_categoria_loja3 = loja3.groupby('Categoria do Produto')['Preço'].count()
vendas_por_categoria_loja4 = loja4.groupby('Categoria do Produto')['Preço'].count()
## 🚚 Frete Médio por Loja
python
Copiar
Editar
frete_medio = lojas.groupby('Loja')['Frete'].mean()

print("\nFrete Médio por Loja:")
frete_medio
## ⚠️ Possíveis Problemas e Soluções
Durante a execução do projeto, alguns problemas podem surgir:

Erro ao acessar as URLs dos arquivos CSV: Se as URLs estiverem incorretas, o Pandas não conseguirá ler os dados.

Solução: Verifique se as URLs estão corretas.

Erro de importação de bibliotecas: Se o Pandas ou Matplotlib não estiverem instalados corretamente, ocorrerá um erro de importação.

Solução: Execute pip install pandas matplotlib.

## ✨ Observações
Os dados foram disponibilizados como parte de um desafio de ciências de dados da Alura.

## 🤝 Contribuições
Contribuições para este projeto são bem-vindas. Sinta-se à vontade para proporcionar melhorias ou enviar pull requests com suas modificações.

## 💾 Licença
Este projeto não possui uma licença específica definida. O uso e distribuição devem seguir as políticas dos dados originais e as diretrizes de uso do GitHub.

## 👩‍💻 Sobre o Autor
Desenvolvido por Felipe Vianna [LinkedIn](https://www.linkedin.com/in/felipe-carnevale-069a60362)
