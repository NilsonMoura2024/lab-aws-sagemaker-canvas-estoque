# 📊Previsão de Estoque Inteligente na AWS com [SageMaker Canvas] (https://aws.amazon.com/pt/sagemaker/canvas/)

## 📋 Introdução

- Esse projeto visa auxiliar a empresa de flower design Rico Prado Lobo Flores a desenvolver um sistema de previsão de estoque inteligente, utilizando um modelo de machine learning.

## 🎯 Objetivo

- Otimizar a gestão de estoque e reduzir custos operacionais.

## 🚀 Passo a Passo

### 1.Dataset:

- Para assegurar consistência e uma análise abrangente, foram consideradas bases de dados referentes a todo o ano de 2023;
- O dataset foi criado considerando variáveis que podem impactar as vendas ao longo do período, tais como: promoções, dia da semana, eventos, temperatura e estação do ano.

### 2.Pré-processamento dos Dados:

- Limpeza dos Dados: Remoção de valores nulos e inconsistentes;
- Feature Engineering: Criação de novas variáveis baseadas em datas e eventos;
- Normalização: Normalização das variáveis para melhorar a performance do modelo.

### 3.Treinamento do Modelo:

- Tipo de Modelo: Time Series Forecasting (Previsão de Séries Temporais);
- Configuração da Série Temporal:

   a)ID da Série: ID do Produto;

   b)Tipo de Modelo: Selecionado automaticamente pelo SageMaker Canvas.

- Seleção do Modelo: O SageMaker Canvas recomenda automaticamente o tipo de modelo mais apropriado para a análise, utilizando técnicas de AutoML (Automated Machine Learning);
- Objetivo: O modelo foi treinado para prever valores futuros de "Quantidade Vendida" utilizando dados históricos;
- Processo:
  
   a)Análise dos dados de entrada;

   b)Seleção automática do tipo de modelo mais adequado;

   c)Treinamento e otimização do modelo escolhido;

   d)Avaliação da performance do modelo;

   e)Variável Alvo: Quantidade Vendida;

   f)Variáveis de Entrada: Dados históricos de vendas, possivelmente incluindo variáveis como dia da semana, estação do ano, eventos especiais, temperatura do dia e promoções.


@Vantagens da Seleção Automática:

- Elimina a necessidade de conhecimento técnico profundo em seleção de modelos;
- Adapta-se às características específicas dos dados fornecidos;
- Potencialmente testa múltiplos tipos de modelos para encontrar o mais adequado.

@Aplicações Práticas (este modelo pode ajudar a responder questões de negócios como):

- Como as vendas serão afetadas se os preços forem aumentados em 10%?;
- Quanto estoque deve ser pedido para a temporada de festas?.


### 4. Avaliação do Modelo:
   
- As métricas de performance do modelo foram avaliadas utilizando o conjunto de validação. Os resultados são os seguintes:
  
   a)Avg.wQL: 0.074;

   b)MAPE: 0.002;
   
   c)WAPE: 0.015

   d)RMSE: 1.382
   
   e)MASE: 0.016

### 5. Análise e Insights:

- Precisão das Previsões: As métricas MAPE e WAPE indicam que o modelo tem alta precisão nas previsões;
- Erro Médio: O RMSE sugere que o modelo tem um erro médio aceitável, considerando a escala dos dados;
- Desempenho Relativo: O MASE indica que o modelo performa significativamente melhor do que um modelo de referência simples.

### 6. Aplicações Práticas: As previsões geradas pelo modelo podem ser utilizadas para:

- Planejar aumentos de preços e entender seu impacto nas vendas;
- Determinar a quantidade de estoque necessária para períodos de alta demanda, como a temporada de festas.

### 7. Conclusões:

- O modelo desenvolvido para prever o estoque da empresa Rico Prado Lobo Flores mostrou-se altamente preciso e eficiente;
-  As previsões podem ser utilizadas para otimizar a gestão de estoque, reduzir custos e melhorar a eficiência operacional.

### 8. Próximos Passos:

- Validação em Produção: Implementar o modelo em um ambiente de produção e monitorar sua performance;
- Ajustes Futuros: Continuar ajustando o modelo com novos dados e variáveis para melhorar ainda mais a precisão das previsões;
- Integração com Sistemas: Integrar as previsões com o sistema de gestão de estoque da empresa para automação de processos.
  
