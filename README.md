# Classificador de Imagens de Gatos e Cachorros

Este é um projeto de classificação de imagens, onde o modelo foi treinado para classificar imagens de gatos e cachorros. O objetivo principal do projeto é avaliar o desempenho do modelo de aprendizado de máquina utilizando métricas de avaliação como Acurácia, Precisão, Revocação, F1-Score, além da Curva ROC.

## Descrição

O modelo foi treinado com um conjunto de dados contendo imagens de gatos e cachorros. Utilizando uma abordagem simples com uma matriz de confusão, foram calculadas as principais métricas para avaliar o desempenho do modelo, além da curva ROC para análise da taxa de falsos positivos e verdadeiros positivos.

## Resultados das Métricas

A partir da matriz de confusão:

|                          | Predição: Gato | Predição: Cachorro |
|--------------------------|-----------------|---------------------|
| **Real: Gato**            | 50 (VP)         | 10 (FN)             |
| **Real: Cachorro**        | 5 (FP)          | 35 (VN)             |

- **Verdadeiro Positivo (VP)**: 50
- **Verdadeiro Negativo (VN)**: 35
- **Falso Positivo (FP)**: 5
- **Falso Negativo (FN)**: 10

Com base na matriz de confusão, foram calculadas as seguintes métricas:

### 1. Acurácia
A **Acurácia** é a porcentagem de previsões corretas feitas pelo modelo.

- Fórmula: \(\frac{VP + VN}{VP + VN + FP + FN}\)
- Resultado: **85%**

### 2. Precisão
A **Precisão** mede a confiabilidade do modelo ao prever um gato.

- Fórmula: \(\frac{VP}{VP + FP}\)
- Resultado: **90.91%**

### 3. Revocação (Sensibilidade)
A **Revocação** mede a capacidade do modelo em identificar corretamente os gatos (classe positiva).

- Fórmula: \(\frac{VP}{VP + FN}\)
- Resultado: **83.33%**

### 4. F1-Score
O **F1-Score** é a média harmônica entre precisão e revocação, proporcionando um equilíbrio entre ambas.

- Fórmula: \(2 \times \frac{\text{Precisão} \times \text{Revocação}}{\text{Precisão} + \text{Revocação}}\)
- Resultado: **86.96%**

### 5. Curva ROC e AUC

A **Curva ROC** (Receiver Operating Characteristic) é usada para avaliar a performance de classificadores binários. Ela plota a taxa de verdadeiros positivos (TPR) contra a taxa de falsos positivos (FPR) para diferentes limiares de decisão. O **AUC** (Área Sob a Curva) fornece uma medida agregada do desempenho do modelo.

- **AUC**: A área sob a curva ROC, que varia de 0 a 1. Quanto mais próxima de 1, melhor o desempenho do modelo.

Abaixo está o gráfico da curva ROC para este modelo:


![Captura de tela_15-11-2024_212353_chatgpt com](https://github.com/user-attachments/assets/a85292ce-121d-45b0-8e0d-019977cf812e)



O gráfico da curva ROC mostra como o modelo ajusta suas decisões entre "Gato" e "Cachorro".

O eixo Y mede a taxa de acertos (quantos gatos o modelo identificou corretamente).
O eixo X mede a taxa de erros (quantos cachorros foram classificados como gatos).
A linha azul mostra o desempenho do modelo, que é muito bom, pois fica longe da linha cinza (classificação aleatória).
Com um valor AUC = 0.98, o modelo acerta na maioria das vezes, o que indica uma separação quase perfeita entre gatos e cachorros.

 
