# Abordagens para Lidar com Conjuntos de Dados Desbalanceados
Neste projeto, foi desenvolvido um modelo de classificação com foco no tratamento de conjuntos de dados desbalanceados. Utilizando o conjunto de dados "diabetes" do pacote Pycaret, exploramos diversas técnicas para melhorar o desempenho dos modelos em cenários de desbalanceamento de classes.

## Modelagem Inicial com Pycaret
Inicialmente, realizamos a criação de modelos de classificação utilizando a biblioteca Pycaret no conjunto de dados original. Com 500 amostras da classe 0 e 268 da classe 1, analisamos diversas métricas de desempenho, com ênfase no Recall devido ao desbalanceamento das classes. O algoritmo Naive Bayes destacou-se com um Recall de 0.5702.

## Aumentando o Desbalanceamento de Classes
Em seguida, exploramos o impacto de aumentar ainda mais o desbalanceamento das classes, reduzindo o número de amostras da classe minoritária para 134. Isso nos permitiu avaliar como os modelos se comportam em condições ainda mais desafiadoras. Observamos uma queda no Recall em todos os modelos, indicando uma dificuldade crescente em identificar corretamente os casos da classe minoritária.

## Ajustando Parâmetros para o Desbalanceamento
Para lidar com o desbalanceamento das classes, realizamos ajustes nos parâmetros dos modelos, utilizando o parâmetro fix_imbalance=True no Pycaret. Essa abordagem resultou em melhorias significativas no desempenho do Recall em comparação com o cenário anterior, demonstrando a importância de considerar o desbalanceamento ao configurar os modelos.

## Utilização do Sklearn para Modelagem Customizada
Por fim, recriamos o modelo de Logistic Regression utilizando a biblioteca Sklearn e considerando o desbalanceamento das classes com o uso da função compute_class_weight. Essa abordagem nos permitiu avaliar a eficácia de uma modelagem customizada em lidar com conjuntos de dados desbalanceados. A Logistic Regression alcançou um Recall de 0.7037, demonstrando sua capacidade de identificar corretamente os casos da classe minoritária.

Em resumo, este projeto destacou a importância de considerar estratégias específicas para lidar com conjuntos de dados desbalanceados na construção de modelos de classificação. A escolha adequada de métricas e técnicas de modelagem pode ser crucial para alcançar um desempenho satisfatório em cenários desafiadores.
