# Algebra Linear Básico Com Python

Autor: Murilo Rocha<br>
Cientista de dados formado em Matemática Aplicada 

## Introdução 🐣

Nos cardos desta pasta, você encontrará uma série de informações e explicações sobre a disciplina de Álgebra Linear e como colocar em prática os conceitos aprendidos utilizando a linguagem de programação Python. A Álgebra Linear é um ramo da matemática muito útil na computação, usado em cálculo numérico, estatística e aprendizado de máquina. Se você pretende se aprofundar em um desses tópicos, precisará ter um conhecimento intermediário de Álgebra Linear. E este é o local perfeito para você iniciar o seu aprendizado!

Cada Jupyter Notebook aborda um tópico específico de Álgebra Linear. A sequência de como você deve ler os Notebooks/Cadernos é a mesma ordem seguida neste documento. Para facilitar, cada caderno possui um índice numérico, que vai de 01 a n, siga esta mesma ordem para que seu aprendizado seja completo.

## Definição de Matriz Real 🐆

Uma matriz real $A$ de ordem $mXn$ ($m$ por $n$) é uma tabela de $m.n$ números reais, dispostos em $m$ linhas e $n$ colunas, onde $m$ e $n \in \mathbb{Z}^+$. Uma matriz real de $m$ linhas e $n$ colunas pode ser representado por $A_{mXn}(R)$, que se lê "Matriz $A$ $m$ por $n$". Também podemos escrever $A = (a_{ij})$; onde $i$ é o índice de linha e $j$ é o índice de coluna. Ou ainda,

$$
\begin{pmatrix}
a_{1,1} & a_{1,2} & a_{1,3} & ... & a_{1,n} \\
a_{2,1} & a_{2,2} & a_{2,3} & ... & a_{2,n} \\
.        & .        & .        &  .  & .    \\
.        & .        & .        &  .  & .    \\
.        & .        & .        &  .  & .    \\
a_{m,1} & a_{m,2} & a_{m,3} & ... & a_{m,n}
\end{pmatrix}
$$

Os elementos de uma matriz podem ser limitados por parênteses, colchetes ou barras duplas. Podemos também representar os elementos de uma matriz por fórmulas.

## Tipos de Matrizes 🐡

Primeiramente definiremos os tipos de matrizes dados de acordo com o número de linhas e colunas. Seja $A_{mxn} = (a_{ij}), esta matriz pode ser:$

### Matriz Linha

Quando $m=1$, chamamos a matriz $A_{1xn}$ de matriz linha:

#### $$A = (a_1, a_2, ..., a_n)$$

A matriz linha é denominada vetor linha (ou simplesmente, vetor).

### Matriz Coluna

Quando $n=1$, chamamos a matriz de matriz coluna.

$$
\begin{pmatrix}
a_1\\
a_2\\
.      \\
.      \\
.      \\
a_m
\end{pmatrix}
$$

A matriz coluna pode ser denominada vetor coluna.

### Matriz Quadrada  🦔

Chamamos de matriz quadrada a matriz que tem o número de linhas igual ao número de colunas, isto é, $m=n$:

$$
\begin{pmatrix}
a_{1,1} & a_{1,2} &  ... & a_{1,n} \\
a_{2,1} & a_{2,2} &  ... & a_{2,n} \\
.        & .      &   .  &  .      \\
.        & .      &   .  &  .      \\
.        & .      &   .  &  .      \\
a_{m,1} & a_{m,2} &  ... &  a_{n,n}
\end{pmatrix}
$$

Dizemos que a matriz acima é uma matriz quadrada de ordem $n$, e escrevemos apenas $A_n$.

#### - Destacamos numa matriz quadrada $A_n = (a_{ij})$ os seguintes elementos:

- Diagonal Principal: Formada pelos termos $a_{ii}$, ou seja, pelos termos onde os índices de linha e coluna são iguais.

- Diagonal Secundária: Formada pelos termos $a_{ij}$, onde $i+j=n+1$.

<center><img src="https://estudos.rededecisao.com.br/wp-content/uploads/sites/5/2020/09/O-que-e-matriz_Imagem_9.png" width=40%></center>

<strong style="color: darkred;">Observação</strong>
Toda matriz quadrada $A_n$, tem obrigatoriamente uma <i>diagonal principal</i> e uma <i>diagonal secundária</i>.

### Matrizes Quadradas Especiais

Dada uma matriz quadrada $A_n = (a_{ij})$, dizemos que A é uma matriz:

-  <strong>Triangular superior</strong> quando $a_{ij} = 0$ se $i > j$, ou seja, possui todos elementos abaixo da diagonal principal nulos.

$$
\begin{pmatrix}
2 & -1 &  3 & -2 \\
0 & 1  &  2 &  3 \\
0 & 0  &  9 &  1 \\
0 & 0  & -0 &  5 \\
\end{pmatrix}
$$

Dada uma matriz quadrada $A_n = (a_{ij})$, dizemos que A é uma matriz:

-  <strong>Triangular inferior</strong> quando $a_{ij} = 0$ se $i < j$, ou seja, possui todos elementos abaixo da diagonal principal nulos.

$$
\begin{pmatrix}
2  &  0  &  0 &  0 \\
2  &  1  &  0 &  0 \\
-3 &  3  &  9 &  0 \\
2  & -2  & -5 &  7 \\
\end{pmatrix}
$$