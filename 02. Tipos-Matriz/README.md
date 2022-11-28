# Tipos de Matrizes 🐡

Primeiramente definiremos os tipos de matrizes dados de acordo com o número de linhas e colunas. Seja $A_{mxn} = (a_{ij}), esta matriz pode ser:$

### Matriz Linha

Quando $m=1$, chamamos a matriz $A_{1xn}$ de matriz linha:

#### $$A = (a_1, a_2, ..., a_n)$$

A matriz linha é denominada vetor linha (ou simplesmente, vetor).

### Matriz Coluna

Quando $n=1$, chamamos a matriz de matriz coluna.

$$
A = 
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
A = 
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
A = 
\begin{pmatrix}
2 & -1 &  3 & -2 \\
0 & 1  &  2 &  3 \\
0 & 0  &  9 &  1 \\
0 & 0  &  0 &  5 \\
\end{pmatrix}
$$

Dada uma matriz quadrada $A_n = (a_{ij})$, dizemos que A é uma matriz:

-  <strong>Triangular inferior</strong> quando $a_{ij} = 0$ se $i < j$, ou seja, possui todos elementos acima da diagonal principal nulos.

$$
A = 
\begin{pmatrix}
2  &  0  &  0 &  0 \\
2  &  1  &  0 &  0 \\
-3 &  3  &  9 &  0 \\
2  & -2  & -5 &  7 \\
\end{pmatrix}
$$

-  <strong>Diagonal</strong> quando $a_{ij} = 0$ se $i \neq j$, ou seja, possui todos elementos fora da diagonal principal nulos.

$$
A = 
\begin{pmatrix}
2  &  0  &  0 &  0 \\
0  &  1  &  0 &  0 \\
0  &  0  &  3 &  0 \\
0  &  0  & 0 &  4 \\
\end{pmatrix}
$$

-  <strong>Escalar</strong> quando $a_{ij} = k$, se $i = j$ e $0$, se $i \neq j$, onde $k$. Isto é, uma matriz escalar é diagonal e possui todos os elementos da diagonal principal iguais a um certo escalar $k$.

$$
\begin{pmatrix}
4  &  0  &  0 &  0 \\
0  &  4  &  0 &  0 \\
0  &  0  &  4 &  0 \\
0  &  0  & 0 &  4 \\
\end{pmatrix}
$$

Vale lembrar que que uma matriz escalar onde $k=1$ é chamada de matriz identidade. E é representada por $I_n$, ou simplesmente, $I$.