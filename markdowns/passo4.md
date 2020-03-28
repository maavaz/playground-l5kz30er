### <b>Operações com Matrizes (Continuação) </b>

### Multiplicação matricial
Essa operação corresponde a multiplicação entre uma matriz (n x m) por uma matriz (m x p),onde o número de colunas da primeira tem que ser igual ao número de linhas da segunda resultando em uma matriz de dimensões (n x p), cujos elementos são a somatório do produto entre os elementos em linha da primeira pelos elementos em coluna da segunda.<br>
Em R, a multiplicação matricial é representada pelo operador **%*%**, respeitando a equidade entre o número de colunas da primeira matriz e o número de linhas da matriz da segunda. <br>


```math
\begin{pmatrix} a & b\\ c & d \end{pmatrix} \cdot \begin{pmatrix} x & y\\ w & z \end{pmatrix} = \begin{pmatrix} a \cdot x + b \cdot w & a \cdot y + b \cdot z\\ c \cdot x + d \cdot w & c \cdot y + d \cdot z \end{pmatrix}


```
#### <b>Exemplo:</b><br>
``` R runnable
Mat = matrix(c(1, 2, 3, 4), nrow = 2)

Mat1 = matrix(c(2, 4, 6, 8), nrow = 2)

mult_mat =  Mat %*% Mat1

print(mult_mat)

```

### Matriz Transposta
A operação de transposição de uma matriz A (m,n) consiste em trocar as linhas pelas colunas de A, esta nova matriz é chamada de matriz transposta de A , representada por A<sup>T</sup>, e é uma matriz (n,m) cujo termo da linha j e coluna i é a<sup>T</sup><sub>ji</sub> = a<sub>ij</sub> para j = 1, ... , n e i= 1, ... , m. <br>


```math
\begin{pmatrix} a & c & e\\ b & d  & f\end{pmatrix} ^ {T} = \begin{pmatrix} a & b\\ c & d\\ e & f \end{pmatrix}

```
#### <b>Exemplo:</b><br>
``` R runnable

Mat = matrix(c(2, 4, 6, 8, 10, 12), nrow = 2)

trans_mat =  t(Mat)

print(Mat)
print(trans_mat)

```

### Determinante de uma Matriz
O determinante de uma matriz é uma função matricial que converte uma matriz quadrada em um escalar. Para uma matriz quadrada de ordem 2, o determinante é definido como:


```math
det\begin{pmatrix}
a & b\\ 
c & d
\end{pmatrix} = a\cdot d - c\cdot b

```
#### <b>Exemplo:</b><br>
``` R runnable

Mat = matrix(c(2, 4, 6, 8, 10, 12), nrow = 2)

trans_mat =  t(Mat)

print(Mat)
print(trans_mat)

```
### Inversa de uma Matriz

A inversa de uma matriz quadrada qualquer cujo determinante seja não nulo, A<sub>n,n</sub>, é uma matriz de mesmas dimensões que atenda a seguinte condição:
```math
A^{-1} \cdot A = I
```


Onde, I é a matriz identidade de mesma dimensão que a matriz A.



A inversa de uma matriz é estimada pela função **solve()**, mesma função utilizada para resolução de sistemas de equações em R.

#### <b>Exemplo:</b><br>
``` R runnable

Mat = matrix(c(2, 4, 6, 8, 10, 12), nrow = 2)

inv_mat =  solve(Mat)

print(inv_mat)

```
