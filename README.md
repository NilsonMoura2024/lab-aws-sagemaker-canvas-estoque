# Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/sagemaker/canvas/)

## Visão Geral

- Desenvolver sistema de previsão de estoque inteligente para a empresa de flower design Rico Prado Lobo Flores, utilizando modelo de machine learning com o SageMaker Canvas da AWS.
  
## Objetivos 

- Otimizar gestão de estoque, reduzir custos operacionais e melhorar a eficácia, eficiência e rentabilidade do negócio.

## Benefícios

- Tomada de decisão mais ágil, assertiva e estratégica baseada em dados, aumentando a eficiência e competitividade no mercado.
  
## Principais Características

- Análise Abrangente: Incorpora dados de vendas de 2023, incluindo promoções, eventos e tendências sazonais;
- Tecnologia Avançada: Aproveita as capacidades de AutoML do SageMaker Canvas para otimizar a seleção e treinamento do modelo;
- Resultados Precisos: Fornece previsões de estoque precisas para melhorar a tomada de decisão.

## Metodologia

- Criação do Dataset: Dados coletados e processados para incluir as variáveis relevantes;
- Treinamento do Modelo: Utilizamos o AWS SageMaker Canvas para treinar o modelo de previsão;
- Avaliação das Métricas: As métricas de performance do modelo incluem RMSE, MAPE, Avg. wQL, WAPE e MASE.

# Descrição detalhada do projeto (passo a passo):

## 1.Dataset:

- Para assegurar consistência e uma análise abrangente, foram consideradas bases de dados referentes a todo o ano de 2023;
- O dataset foi criado levando em conta variáveis que podem impactar as vendas ao longo do período, tais como: promoções, dia da semana, eventos, temperatura e estação do ano.

## 2.Pré-processamento dos Dados:

- Limpeza dos Dados: Remoção de valores nulos e inconsistentes;
- Feature Engineering: Criação de novas variáveis baseadas em datas e eventos;
- Normalização: Normalização das variáveis para melhorar a performance do modelo.

## 3.Treinamento do Modelo:

Tipo de Modelo: Selecionado automaticamente pelo SageMaker Canvas.
- Tipo de Modelo: Time Series Forecasting (Previsão de Séries Temporais);
- Configuração da Série Temporal:

   a) ID da Série: ID do Produto;

   b) Tipo de Modelo: Selecionado automaticamente pelo SageMaker Canvas.

- Seleção do Modelo: O SageMaker Canvas recomenda automaticamente o tipo de modelo mais apropriado para a análise, utilizando técnicas de AutoML (Automated Machine Learning);
- Objetivo: O modelo foi treinado para prever valores futuros de "Quantidade Vendida" utilizando dados históricos;
- Processo:
  
   a) Análise dos dados de entrada;

   b) Seleção automática do tipo de modelo mais adequado;

   c) Treinamento e otimização do modelo escolhido;

   d )Avaliação da performance do modelo;

   e )Variável Alvo: Quantidade Vendida;

   f)Variáveis de Entrada: Dados históricos de vendas, possivelmente incluindo variáveis como dia da semana, estação do ano, eventos especiais, temperatura do dia e promoções.


* Vantagens da Seleção Automática:

- Elimina a necessidade de conhecimento técnico profundo em seleção de modelos;
- Adapta-se às características específicas dos dados fornecidos;
- Potencialmente testa múltiplos tipos de modelos para encontrar o mais adequado.

* Aplicações Práticas (este modelo pode ajudar a responder questões de negócios como):

- Como as vendas serão afetadas se os preços forem aumentados em 10%?
- Quanto estoque deve ser pedido para a temporada de festas?


## 4. Avaliação do Modelo:
   
- As métricas de performance do modelo foram avaliadas utilizando o conjunto de validação. Os resultados são os seguintes:
  
   a) Avg.wQL: 0.074

   b) MAPE: 0.002
   
   c) WAPE: 0.015

   d) RMSE: 1.382
   
   e) MASE: 0.016

## 5. Análise e Insights:

- Precisão das Previsões: As métricas MAPE e WAPE indicam que o modelo tem alta precisão nas previsões;
- Erro Médio: O RMSE sugere que o modelo tem um erro médio aceitável, considerando a escala dos dados;
- Desempenho Relativo: O MASE indica que o modelo performa significativamente melhor do que um modelo de referência simples.

## 6. Aplicações Práticas: As previsões geradas pelo modelo podem ser utilizadas para:

- Planejar aumentos de preços e entender seu impacto nas vendas;
- Determinar a quantidade de estoque necessária para períodos de alta demanda, como a temporada de festas.

## 7. Conclusões:

- O sistema de previsão de estoque desenvolvido mostrou-se altamente preciso e eficiente;
-  As previsões geradas podem ser utilizadas para otimizar a gestão de estoque, reduzir custos operacionais e melhorar a eficiência e rentabilidade do negócio;
-  A tomada de decisões baseada em dados permitirá à empresa ser mais estratégica, responder mais rapidamente e de forma mais assertiva às demandas do mercado, aumentando sua competitividade.

## 8. Próximos Passos:

- Implementação em Produção: Colocar o sistema de previsão de estoque em um ambiente de produção e monitorar continuamente sua performance;
- Refinamento Contínuo: Ajustar e aprimorar o modelo com novos dados e variáveis para aumentar a precisão das previsões;
- Integração de Sistemas: Incorporar as previsões ao sistema de gestão de estoque da empresa para automatizar processos e facilitar a tomada de decisões;
- Treinamento da Equipe: Capacitar os colaboradores para interpretar e utilizar efetivamente os insights gerados pelo sistema;
- Avaliação de Impacto: Medir e analisar o impacto do sistema na eficiência operacional, redução de custos e rentabilidade do negócio.

## 9. Referências:

-  [Documentação do SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)


  
