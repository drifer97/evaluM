🧩 Análise de Modelo de Classificação – Métricas de Avaliação
Olá, pessoal! 👋

Recentemente, finalizei um estudo prático sobre métricas de avaliação em problemas de classificação. Trabalhei com uma matriz de confusão simples, aplicada em um modelo que classifica imagens de gatos e cachorros.

📊 Resultados das Métricas
A partir da matriz de confusão:

Verdadeiro Positivo (VP): 50
Verdadeiro Negativo (VN): 35
Falso Positivo (FP): 5
Falso Negativo (FN): 10
Calculei as principais métricas para avaliar o desempenho do modelo:

1️⃣ Acurácia
Fórmula:

Acur
a
ˊ
cia
=
𝑉
𝑃
+
𝑉
𝑁
𝑉
𝑃
+
𝑉
𝑁
+
𝐹
𝑃
+
𝐹
𝑁
Acur 
a
ˊ
 cia= 
VP+VN+FP+FN
VP+VN
​
 
Cálculo:

Acur
a
ˊ
cia
=
50
+
35
50
+
35
+
5
+
10
=
85
100
=
0.85
 
(
85
%
)
Acur 
a
ˊ
 cia= 
50+35+5+10
50+35
​
 = 
100
85
​
 =0.85(85%)
2️⃣ Precisão
Fórmula:

Precis
a
˜
o
=
𝑉
𝑃
𝑉
𝑃
+
𝐹
𝑃
Precis 
a
˜
 o= 
VP+FP
VP
​
 
Cálculo:

Precis
a
˜
o
=
50
50
+
5
=
50
55
≈
0.9091
 
(
90.91
%
)
Precis 
a
˜
 o= 
50+5
50
​
 = 
55
50
​
 ≈0.9091(90.91%)
3️⃣ Revocação (Sensibilidade)
Fórmula:

Revoca
c
¸
a
˜
o
=
𝑉
𝑃
𝑉
𝑃
+
𝐹
𝑁
Revoca 
c
¸
​
  
a
˜
 o= 
VP+FN
VP
​
 
Cálculo:

Revoca
c
¸
a
˜
o
=
50
50
+
10
=
50
60
≈
0.8333
 
(
83.33
%
)
Revoca 
c
¸
​
  
a
˜
 o= 
50+10
50
​
 = 
60
50
​
 ≈0.8333(83.33%)
4️⃣ F1-Score
Fórmula:

𝐹
1
=
2
×
Precis
a
˜
o
×
Revoca
c
¸
a
˜
o
Precis
a
˜
o
+
Revoca
c
¸
a
˜
o
F1=2× 
Precis 
a
˜
 o+Revoca 
c
¸
​
  
a
˜
 o
Precis 
a
˜
 o×Revoca 
c
¸
​
  
a
˜
 o
​
 
Cálculo:

𝐹
1
=
2
×
0.9091
×
0.8333
0.9091
+
0.8333
=
2
×
0.7575
1.7424
≈
0.8696
 
(
86.96
%
)
F1=2× 
0.9091+0.8333
0.9091×0.8333
​
 =2× 
1.7424
0.7575
​
 ≈0.8696(86.96%)




![Captura de tela_15-11-2024_212353_chatgpt com](https://github.com/user-attachments/assets/36e58e63-6043-468e-9651-ea21bba1ad99)

Aqui está a Curva ROC do modelo, com os seguintes destaques:

A Taxa de Verdadeiros Positivos (TPR) está no eixo Y.
A Taxa de Falsos Positivos (FPR) está no eixo X.
A linha cinza representa uma classificação aleatória (AUC = 0.5).
O modelo alcançou uma AUC = 0.98, indicando excelente desempenho.

 
