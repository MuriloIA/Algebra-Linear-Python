# Tipos de Matrizes 🐡

Primeiramente definiremos os tipos de matrizes dados de acordo com o número de linhas e colunas. Seja $A_{mxn} = (a_{ij})$, esta matriz pode ser:

## Matriz Linha

Quando $m=1$, chamamos a matriz $A_{1xn}$ de matriz linha:

### $$A = (a_1, a_2, ..., a_n)$$

A matriz linha é denominada vetor linha (ou simplesmente, vetor).

## Matriz Coluna

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

## Matriz Quadrada

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

### - Destacamos numa matriz quadrada $A_n = (a_{ij})$ os seguintes elementos:

- Diagonal Principal: Formada pelos termos $a_{ii}$, ou seja, pelos termos onde os índices de linha e coluna são iguais.

- Diagonal Secundária: Formada pelos termos $a_{ij}$, onde $i+j=n+1$.

<center><img src="https://estudos.rededecisao.com.br/wp-content/uploads/sites/5/2020/09/O-que-e-matriz_Imagem_9.png" width=40%></center>

<strong style="color: darkred;">Observação</strong>
Toda matriz quadrada $A_n$, tem obrigatoriamente uma <i>diagonal principal</i> e uma <i>diagonal secundária</i>.

## Matrizes Quadradas Especiais

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
A = 
\begin{pmatrix}
4  &  0  &  0 &  0 \\
0  &  4  &  0 &  0 \\
0  &  0  &  4 &  0 \\
0  &  0  & 0  &  4 \\
\end{pmatrix}
$$

Vale lembrar que que uma matriz escalar onde $k=1$ é chamada de matriz identidade. E é representada por $I_n$, ou simplesmente, $I$.

$$
I = 
\begin{pmatrix}
1  &  0  &  0 &  0 \\
0  &  1  &  0 &  0 \\
0  &  0  &  1 &  0 \\
0  &  0  &  0 &  1 \\
\end{pmatrix}
$$

## Matriz Oposta

Data a matriz $A = (a_{ij}) \in M_{mxn}(R)$, dizemos que a matriz $B = (b_{ij}) \in M_{mxn}(R)$ é oposta de A se $b_{ij} = -a_{ij}$ para todo $i \in {1, 2, ..., m}$ e todo $j \in {1, 2, ..., n}$. Ou seja, os elementos da matriz oposta de $A$ são os elementos opostos aos elementos de $A$. Representamos a oposta de $A$ por $-A$.

**Exemplo:**<br>

A matriz oposta de

$$
A = 
\begin{pmatrix}
2  & 27 &  9\\
-1 & 1  &  0\\
3  & -7 &  4\\
\end{pmatrix}
$$

é 

$$-A =
\begin{pmatrix}
-2  & -27 &  -9\\
1   & -1  &  0\\
-3  & 7   &  -4\\
\end{pmatrix}
$$

## Matriz Transposta

Dada a matriz $A = (a_{ij}) \in M_{mxn}(R)$, dizemos que a matriz $B = (b_{ij}) \in M_{nxm}(R)$ é transposta de $A$ se $b_{ji} = a_{ij}$ para todo $i \in {1, 2, ..., m}$ e todo $j \in {1, 2, ..., n}$. Representamos a transposta de $A$ por $A^t$.

**Exemplo:**

A transposta de

$$
A = 
\begin{pmatrix}
2  & 5 &  \frac{2}{3}\\
0 & \sqrt{7}  &  6\\
\end{pmatrix}
$$ 

é 

$$A^t =
\begin{pmatrix}
2    &  0\\
5    &  \sqrt{7}\\
\frac{2}{3}   &  6\\
\end{pmatrix}
$$

##### Propriedades

- $T_1$: $(A^t)^t = A$

- $T_2$: $(A + B)^t = A^t + B^t$

- $T_3$: $(\alpha A)^t = \alpha A^t$

- $T_4$: $(AB)^t = A^tB^t$

## Matriz Simétrica

Dizemos que uma matriz 

$$A = (a_{ij}) \in M_n(R)$$

é simétrica se 
 
$$A = A^t$$

isto é, 
 
$$a_{ij} = a{ji}, \forall i, j \in 1, 2, ..., n$$

**Exemplo:**

A matriz 

$$
A = 
\begin{pmatrix}
2  & -1 & 3\\
-1 & 1  & -7\\
3  & -7 & 4\\  
\end{pmatrix}
$$ 

é simétrica, já que

$$A^t =
\begin{pmatrix}
2  & -1 & 3\\
-1 & 1  & -7\\
3  & -7 & 4\\  
\end{pmatrix} = A
$$

## Matriz Antissimétrica

Dizemos que uma matriz $A = (a_{ij}) \in M_n(R)$ é antissimétrica se $A = -A^t$, isto é,

$$
a_{ij} =
  \begin{cases}
    0       & i=j\\
    -a_{ij} & i\neq j
  \end{cases}
$$