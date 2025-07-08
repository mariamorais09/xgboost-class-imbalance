*Projeto desenvolvido no âmbito da unidade curricular de Machine Learning I no segundo semestre do ano letivo 2024/2025*

**Modificação do XGBoost para Tratamento de Desbalanceamento de Classes**

*Descrição do Projeto*

Este projeto tem como objetivo a implementação, modificação e avaliação de um algoritmo de classificação para lidar com uma característica específica dos dados: desbalanceamento de classes em problemas de classificação binária.
Utilizamos como base o algoritmo de Gradient Boosting Trees (XGBoost), implementado do zero, e propusemos uma modificação para tornar o modelo mais robusto em datasets com classes desbalanceadas, sem utilizar técnicas externas de reamostragem.

*Objetivos*

- Implementar a versão padrão do algoritmo XGBoost a partir do zero, sem uso de bibliotecas prontas (como scikit-learn).
- Avaliar empiricamente a performance do modelo padrão em datasets desbalanceados.
- Propor e implementar uma modificação no algoritmo para melhorar sua robustez frente ao desbalanceamento.
- Comparar o desempenho entre a versão padrão e a versão modificada usando conjuntos de dados benchmark.

*Metodologia*

Algoritmo base: Gradient Boosting Trees inspirado no XGBoost.
Modificação proposta:
- Aplicação de pesos, dando maior peso à classe minoritária durante o treino
- Aplicação de Hellinger Gain Distance nos splits da primeira árvore
Dados: Conjuntos públicos de benchmark para classificação binária com diferentes níveis de desbalanceamento.
Avaliação: Métricas de desempenho focadas em classificação desbalanceada, como F1-score, PR-AUC, AUC-ROC.

*Como Executar*
Clone o repositório:

git clone https://github.com/mariamorais09/xgboost-class-imbalance.git
cd xgboost-class-imbalance
