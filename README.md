📊 Análise de Dados de Vendas de Lojas
🛒 Desafio - Alura Store - Análise de Lojas
Este projeto realiza uma análise exploratória de dados de vendas de quatro lojas, utilizando a biblioteca Pandas para manipulação de dados e Matplotlib para visualização. O objetivo é fornecer insights sobre o faturamento, as vendas por categoria, a média de avaliação dos clientes, os produtos mais e menos vendidos e o frete médio de cada loja.

🔍 Visão Geral do Projeto
O script Python ( .ipynb ) realiza as seguintes etapas:

1. Importação de Dados:
Carrega os dados de vendas de cada loja a partir de arquivos CSV hospedados no GitHub.

2. Análise de Faturamento:
Calcula o faturamento total de cada loja, o faturamento médio e visualiza a distribuição do faturamento entre as lojas através de um gráfico de barras.

3. Análise de Vendas por Categoria:
Combina os dados de todas as lojas, calcula o faturamento por categoria em cada loja e apresenta essa informação em um gráfico de barras lado a lado.

4. Análise da Média de Avaliação:
Calcula a média das avaliações de compra para cada loja e exibe essa informação em um gráfico de barras.

5. Análise de Produtos Mais e Menos Vendidos:
Identifica o produto com maior e menor quantidade vendida em cada loja.

6. Análise de Frete Médio:
Calcula o custo médio de frete para cada loja.

7. Análise Geográfica das Vendas:
Utiliza as coordenadas de latitude e longitude apresentadas nos dados para visualizar a distribuição geográfica das vendas, o faturamento por localização e a distribuição das avaliações.

⬇️ Instalação
Para executar este projeto, você precisa ter o Python instalado em seu ambiente. Além disso, as seguintes bibliotecas são necessárias:

Pandas: Para manipulação e análise de dados tabulares.

Matplotlib: Para criação de gráficos e visualizações.

NumPy: Embora não seja explicitamente importado no código fornecido, o Matplotlib é frequentemente utilizado internamente para transações numéricas.

Você pode instalar essas bibliotecas usando o pip (ou gerenciador de pacotes do Python). Abra seu terminal ou prompt de comando e execute o seguinte comando:

bash
Copiar
Editar
pip install pandas matplotlib
📌 Dependências
As seguintes bibliotecas Python são dependências deste projeto:

pandas (>= 1.0.0): Utilizado para leitura e manipulação dos dados das lojas a partir de arquivos CSV hospedados em URLs.

matplotlib (>= 3.0.0): Empregada para gerar gráficos de barras que visualizam o faturamento por loja, as vendas por categoria e a média de avaliação das lojas.

numpy (>= 1.18.0): Usado internamente pelo Matplotlib para cálculos numéricos, como o cálculo da média de faturamento para a linha de referência no gráfico.

⚙️ Execução no Google Colab
O Google Colab é um ambiente Jupyter Notebook hospedado na nuvem que permite executar o código Python sem a necessidade de configuração local. Para executar este projeto no Colab, siga estes passos:

Abra o Google Colab: Acesse https://colab.research.google.com/ no seu navegador.

Crie um novo notebook: Clique em "Novo notebook" no canto inferior direito da tela.

Copie e cole o código: Copie todo o código Python fornecido e cole em uma célula de código no seu notebook do Colab.

Execute como células: Execute como células de código sequencialmente, clicando no botão "play" (executar) ao lado de cada célula ou pressionando Shift + Enter. O Colab já possui as bibliotecas Pandas e Matplotlib pré-instaladas, então você não precisa executar o comando !pip install novamente, a menos que necessite de versões específicas ou outras bibliotecas adicionais.

💡 Explicação do Código
O código Python realiza as seguintes etapas de análise:

1. Importação dos Dados:
python
Copiar
Editar
import pandas as pd
url1 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science/main/base-de-dados-challenge-1/loja_1.csv"
# Carregar dados para outras lojas de forma similar
2. Análise do Faturamento:
Calcula o faturamento total de cada loja somando os valores da coluna Preço.

3. Análise de Vendas por Categoria:
Agrupa os dados de cada loja pela coluna Categoria do Produto e calcula o número de vendas em cada categoria.

4. Análise da Média de Avaliação:
Calcula a média das avaliações de compra para cada loja.

5. Análise de Produtos Mais e Menos Vendidos:
Identifica os produtos mais e menos vendidos de cada loja.

6. Análise de Frete Médio:
Calcula o custo médio de frete para cada loja.

⚠️ Possíveis Problemas e Soluções
Durante a execução do projeto, alguns problemas podem surgir:

Erro ao acessar as URLs dos arquivos CSV:

Problema: Se as URLs dos arquivos CSV estiverem incorretas, o Pandas não conseguirá ler os dados.

Solução: Verifique se as URLs estão corretas e acessíveis.

Erro de importação de bibliotecas:

Problema: Se as bibliotecas Pandas ou Matplotlib não estiverem instaladas corretamente, erros de importação ocorrerão.

Solução: Execute o comando pip install pandas matplotlib.

Problemas com a exibição de gráficos:

Problema: Em alguns ambientes, os gráficos gerados pelo Matplotlib podem não ser exibidos corretamente.

Solução: No Google Colab, os gráficos são exibidos automaticamente. Se estiver no Jupyter, use %matplotlib inline para garantir que os gráficos apareçam.

✨ Observações
Os dados foram disponibilizados como parte de um desafio de ciências de dados da Alura.

O projeto foi desenvolvido com o objetivo de aprimorar a análise e visualização de dados de vendas.

🤝 Contribuições
Contribuições para este projeto são bem-vindas. Sinta-se à vontade para propor melhorias ou enviar pull requests com suas modificações.

💾 Licença
Este projeto não possui uma licença específica definida. O uso e distribuição devem seguir as políticas dos dados originais e as diretrizes de uso do GitHub.
