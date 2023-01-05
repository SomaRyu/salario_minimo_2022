# salario_minimo_2022
O objetivo deste trabalho foi realizar a previsão do salário mínimo no Brasil para o ano de 2022 a partir dos valores desde a implantação do Plano Real.
Os dados empregados foram retirados da internet (IpeaData) e apenas o último aumento anual foi considerado nas análises estatísticas.
Para a previsão do salário mínimo foi utilizado a Regressão Linear com e sem o treinamento dos dados.
A análise estatística a partir da Regressão Linear, com e sem treinamento dos dados, demonstrou uma forte correlação entre o salário mínimo e o tempo (R² > 0,95). Ambas as previsões apresentaram valores similares de salário mínimo, entretanto, os salários obtidos diferiram significativamente do valor real ( > 12%).

Estendendo o estudo, considerou-se uma nova variável para a previsão do salário mínimo para 2022, a inflação, sendo ela estimada a partir do índice IPCA (Índice Nacional de Preços ao Consumidor Amplo).
Este índice, calculado pelo IBGE (Instituto Brasileiro de Geografia e Estatística), mensura a variação do preço de produtos e serviços consumidos pela população mensalmente. Neste estudo foram considerados os valores acumulados por ano.
Analisando o salário mínimo a partir da variável tempo e inflação, foi realizada a Regressão Linear Múltipla (RLM) com e sem o treinamento dos dados.
O valor utilizado da inflação para as previsões de 2022 foi a média da inflação do dataframe analisado, no caso da RLM sem o treinamento dos dados, a inflação média foi obtida a partir dos dados de 1995-2021, enquanto para a inflação média da RLM com treinamento dos dados, o seu valor foi obtido do grupo de treino (X_train).
O modelo que apresentou o valor mais próximo ao salário mínimo de 2022 foi o sem treinamento dos dados, apresentando uma diferença de 10,64% em relação ao valor de 2022. No entanto, o modelo com treinamento dos dados demonstrou uma maior correlação entre as variáveis e o salário mínimo, com R² = 0,9714, superior ao valor obtido da correlação sem treinamento de dados (R² = 0,9659).

O projeto foi desenvolvido utilizando a plataforma GoogleColab.
Fontes:
http://www.ipeadata.gov.br/exibeserie.aspx?stub=1&serid1739471028=1739471028
https://www.ibge.gov.br/estatisticas/economicas/precos-e-custos/9256-indice-nacional-de-precos-ao-consumidor-amplo.html?t=series-historicas
