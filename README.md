# Análise e Previsão de Crédito com Regressão Linear

Projeto de Machine Learning desenvolvido no Google Colab para estimar o valor de empréstimos concedidos com base no perfil financeiro do cliente.

## Objetivo do projeto
Construir um modelo de regressão capaz de prever a variável contínua `valor_emprestimo` a partir de atributos socioeconômicos.

##  Estrutura dos Dados (`base_credito.csv`)
* **`idade`**: Idade do cliente 
* **`renda_mensal`**: Renda mensal em reais 
* **`score_credito`**: Pontuação de crédito 
* **`historico_pagamentos`**: Percentual de pagamentos em dia
* **`valor_emprestimo`**: Valor concedido/estimado (Variável Alvo) 

## Tecnologias Utilizadas
* Python 3
* Google Colab
* Pandas, Matplotlib & Scikit-learn

## Etapas Desenvolvidas
1. Carregamento e visualização dos dados
2. Identificação das variáveis de entrada e da variável alvo
3. Análise inicial dos dados e visualização gráfica
4. Divisão dos dados em treinamento e teste
5. Criação e treinamento do modelo de Regressão Linear
6. Geração de previsões
7. Avaliação do modelo utilizando MAE e MSE
8. Comparação entre valores reais e previstos
9. Previsão do valor de empréstimo para um novo cliente
10. Análise dos resultados e limitações do modelo

## Avaliação e Resultados
 **Métricas Utilizadas:**

MAE (Erro Absoluto Médio): Indica o erro médio em reais entre a previsão e a realidade.

MSE (Erro Quadrático Médio): Avalia a precisão penalizando com mais rigor os erros de maior magnitude.

## Desempenho no Conjunto de Teste:
O modelo atingiu um MAE de R$ 3.001,04, demonstrando que as estimativas se mantêm, em média, a uma distância de cerca de 3 mil reais do valor real concedido.

A validação gráfica (Gráfico de Dispersão: Real vs. Previsto) reforçou a boa aderência da Regressão Linear, mostrando que as previsões acompanham a trajetória real dos dados ao longo de todas as faixas de valo

## OBS
Vale ressaltar que todos os valores obtidos são estimativas baseadas no histórico da base de dados utilizada. Na prática, o desempenho do modelo pode oscilar se ele for aplicado a dados com distribuições diferentes ou a perfis de clientes que não estejam bem representados no conjunto de treinamento.
