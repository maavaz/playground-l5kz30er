### <b>Operações com Matrizes</b>

### Soma de Matrizes
A operação de soma de matrizes segue a mesma sintaxe que na operação entre escalares, isto é, dada duas matrizes de mesma dimensão, a soma de ambas resulta numa matriz cujos elementos são a soma dos elementos das matrizes originais, conforme exibido abaixo. <br>

```math
 \begin{pmatrix}  a & b \\ c & d  \end{pmatrix}  +  \begin{pmatrix} x & y \\ w & z \end{pmatrix}  =    \begin{pmatrix} a+x & b+y \\ c+w & d+z \end{pmatrix}
```

#### <b>Exemplo:</b><br>
``` R runnable
Mat = matrix(c(1, 2, 3, 4), nrow = 2)

Mat1 = matrix(c(2, 4, 6, 8), nrow = 2)

soma_mat =  Mat + Mat1

print(soma_mat)

```
### Subtração de Matrizes
A operação de subtração de matrizes é semelhante a soma, isto é, dada duas matrizes de mesma dimensão, a subtração de ambas resulta numa matriz cujos elementos são a subtração dos elementos das matrizes originais, conforme exibido abaixo. <br>

```math
 \begin{pmatrix}  a & b \\ c & d  \end{pmatrix}  -  \begin{pmatrix} x & y \\ w & z \end{pmatrix}  =    \begin{pmatrix} a-x & b-y \\ c-w & d-z \end{pmatrix}
```
#### <b>Exemplo:</b><br>
``` R runnable
Mat = matrix(c(1, 2, 3, 4), nrow = 2)

Mat1 = matrix(c(2, 4, 6, 8), nrow = 2)

sub_mat =  Mat1 - Mat

print(sub_mat)

```
### Multiplicação por um escalar
Dada uma matriz de qualquer dimensão, a multiplicação por um escalar e, tal que e ∈ R, resulta em uma matriz onde seus elementos correspondem ao produto do escalar por cada um dos elementos da matriz. <br>

```math
 e . \begin{pmatrix} x & y \\ w & z \end{pmatrix}  =    \begin{pmatrix} e.x & e.y \\ e.w & e.z \end{pmatrix}
```
#### <b>Exemplo:</b><br>
``` R runnable
e <- 5
Mat = matrix(c(1, 2, 3, 4), nrow = 2)

Mat1 = matrix(c(2, 4, 6, 8), nrow = 2)

prod_mat =  e * Mat
prod_mat1 = e * Mat1

print(prod_mat)

print(prod_mat1)
```

### Multiplicação entre Matrizes
A operação de multiplicação entre matrizes resulta em uma matriz onde os elementos correspondem ao produto dos elementos equivalentes das duas matrizes de mesmas dimensões. <br>

```math
 \begin{pmatrix}  a & b \\ c & d  \end{pmatrix}  °  \begin{pmatrix} x & y \\ w & z \end{pmatrix}  =    \begin{pmatrix} a.x & b.y \\ c.w & d.z \end{pmatrix}
```

#### <b>Exemplo:</b><br>
``` R runnable
Mat = matrix(c(1, 2, 3, 4), nrow = 2)

Mat1 = matrix(c(2, 4, 6, 8), nrow = 2)

mult_mat =  Mat * Mat1

print(mult_mat)

```

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

