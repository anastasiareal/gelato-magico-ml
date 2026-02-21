# Projeto: Previsão de Vendas de Sorvetes com Base na Temperatura


**DESCRIÇÃO GERAL** 


Este repositório contém um projeto de Machine Learning para prever as vendas diárias de sorvetes na sorveteria fictícia "Gelato Mágico", localizada em uma cidade litorânea. O modelo utiliza regressão linear para estimar as vendas com base na temperatura ambiente, ajudando a otimizar a produção e reduzir desperdícios ou perdas de vendas.O projeto foi desenvolvido passo a passo, seguindo um pipeline reprodutível, com foco em treinamento de modelo, gerenciamento com MLflow (exemplo de código), implantação em nuvem (sugestões para AWS Lambda) e visualizações interativas. Dados sintéticos foram gerados para simular cenários reais, e análises adicionais foram incluídas para enriquecer o portfólio.Objetivos Alcançados Treinar um modelo de regressão linear (usando Statsmodels) para prever vendas com base na temperatura.
 ⊹ Gerar e salvar datasets em Excel para reprodutibilidade.
 ⊹ Expandir o arquivo de inputs com frases temáticas para análise qualitativa.
 ⊹ Fornecer códigos para integração com MLflow e implantação em tempo real.

**_Estrutura do Repositórioinputs/:_** Pasta com sentencas.txt, contendo frases exemplo sobre vendas de sorvetes e fatores climáticos (ex.: "O calor intenso atrai mais clientes para sabores refrescantes."). Foram adicionadas múltiplas rodadas de frases para maior variedade, totalizando mais de 30 entradas.
pipeline.py: Script principal que:Gera dados sintéticos (100 amostras de temperatura e vendas, com seed 42 para reprodutibilidade).
Treina o modelo OLS (Ordinary Least Squares).

**_data.csv:_** Arquivo CSV com o dataset gerado (colunas: Temperature, Sales).
data.xlsx: Arquivo Excel equivalente ao CSV, para análise em ferramentas como Microsoft Excel.
**_sales_vs_temp.html:_** Gráfico interativo gerado com Plotly, mostrando scatter plot de vendas vs. temperatura com linha de regressão.


  **INSIGHTS APRENDIDOS**


◆◇◈ A temperatura explica ~90% das variações nas vendas, confirmando a hipótese inicial.
◆◇◈ Dados sintéticos facilitam testes, mas em produção, integrar APIs de clima (ex.: OpenWeather) seria ideal.
◆◇◈ Visualizações interativas com Plotly tornam o portfólio mais atrativo para recrutadores.
◆◇◈ Expansão de frases em sentencas.txt sugere futuras análises com NLP para extrair padrões qualitativos.
◆◇◈ Reprodutibilidade garantida via seeds e salvamento de arquivos permite fácil replicação.




