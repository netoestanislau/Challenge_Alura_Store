# Challenge_Alura_Store

# Análise de Desempenho das Lojas Alura Store

## Visão Geral do Projeto

Este projeto tem como objetivo analisar o desempenho de quatro lojas fictícias da rede Alura Store, utilizando dados de vendas, avaliações e frete. O principal objetivo é identificar a loja com menor eficiência para auxiliar o Senhor João na decisão de qual unidade vender para iniciar um novo empreendimento.

A análise foi realizada utilizando a biblioteca Pandas para manipulação e análise de dados, e as bibliotecas Matplotlib e Seaborn para a criação de visualizações gráficas.

## Estrutura do Projeto

O projeto consiste em um script Python (executado em um ambiente Colab) que realiza as seguintes etapas:

1.  **Carregamento dos Dados:** Os dados de cada loja são carregados a partir de arquivos CSV hospedados no GitHub, utilizando a função `pd.read_csv()`.
2.  **Análise Exploratória:** Diversas métricas são calculadas e analisadas para cada loja:
    * Faturamento Total (soma da coluna 'Preços').
    * Categorias de produtos mais e menos vendidas (contagem de ocorrências).
    * Média das avaliações dos clientes (média da coluna 'Avaliação').
    * Produtos mais e menos vendidos (contagem de ocorrências).
    * Frete médio (média da coluna 'Frete').
3.  **Visualização de Dados:** Três gráficos distintos são gerados para ilustrar os principais insights da análise:
    * Gráfico de barras comparando o faturamento total e a média de avaliação por loja.
    * Gráfico de dispersão explorando a relação entre o número de vendas e a avaliação média de produtos em uma das lojas.
    * Gráfico de linha mostrando a tendência de faturamento acumulado ao longo das transações em uma das lojas (sob a suposição de ordem temporal).
4.  **Relatório Final:** Um relatório em texto (gerado no Colab) sintetiza as descobertas da análise, justifica a recomendação de qual loja vender e se baseia nos dados e visualizações geradas.

## Como Executar o Projeto

Este projeto foi desenvolvido para ser executado em um ambiente Google Colaboratory. Para reproduzir a análise, siga os passos abaixo:

1.  **Acessar o Google Colab:** Abra um navegador web e acesse o site do [Google Colaboratory](https://colab.research.google.com/).
2.  **Criar um Novo Notebook:** Clique em "Novo notebook".
3.  **Copiar e Colar o Código:** Copie o código Python fornecido (incluindo o carregamento das bibliotecas, o carregamento dos dados, as análises e a geração dos gráficos) e cole nas células do notebook.
4.  **Executar as Células:** Execute as células de código em sequência, clicando no botão de "play" ao lado de cada célula ou usando o atalho `Shift + Enter`.
5.  **Visualizar Resultados:** Os resultados da análise (tabelas impressas e gráficos gerados) serão exibidos na saída das células. O relatório final em texto também será impresso na saída da célula correspondente.

## Dependências

Este projeto utiliza as seguintes bibliotecas Python:

* **Pandas:** Para manipulação e análise de dados tabulares (DataFrames).
* **Matplotlib:** Para criação de gráficos e visualizações básicas.
* **Seaborn:** Para criação de gráficos estatísticos mais avançados e esteticamente agradáveis (construído sobre Matplotlib).
* **Numpy:** Utilizado para operações numéricas, como a criação de arrays para a plotagem de gráficos.

Essas bibliotecas são comumente encontradas em ambientes de ciência de dados, como o Google Colaboratory, e geralmente vêm pré-instaladas. Caso alguma biblioteca não esteja disponível, você pode instalá-la executando o comando `!pip install nome_da_biblioteca` em uma célula do Colab.

## Insights e Resultados Principais

A análise revelou que a **Loja 4** apresenta o menor desempenho em diversos aspectos:

* **Faturamento Total:** Significativamente inferior às demais lojas.
* **Média de Avaliação dos Clientes:** A mais baixa entre as lojas, indicando menor satisfação.
* **Frete Médio:** Tendência a ser mais alto, o que pode impactar a decisão de compra.
* **Desempenho de Produtos:** Não apresenta produtos com vendas excepcionalmente altas e pode ter uma proporção maior de produtos com baixa saída.

Com base nesses insights, o relatório final recomenda que o Senhor João considere a venda da **Loja 4** para iniciar seu novo empreendimento.

## Possíveis Problemas e Soluções

* **Conexão com a Internet:** A execução do código depende de uma conexão estável com a internet para carregar os dados dos URLs fornecidos. Verifique sua conexão caso encontre erros ao carregar os arquivos.
* **Versões das Bibliotecas:** Pequenas diferenças nas versões das bibliotecas podem levar a variações na aparência dos gráficos, mas não devem afetar os resultados da análise em si.
* **Interpretação da "Tendência" de Faturamento:** O gráfico de linha de tendência de faturamento assume uma ordem temporal implícita nos dados, o que pode não ser preciso se os dados não estiverem ordenados cronologicamente. Uma análise mais precisa da tendência de faturamento exigiria uma coluna de data explícita nos dados.
