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
A operação de subtração de matrizes é semelhante a soma, isto é, dada duas matrizes de mesma dimensão, a subtração de ambas resulta numa matriz cujos elementos são a subtração dos elementos das matrizes originais, conforme exibido abaixo. <br>

```math
  e .\begin \begin{pmatrix} x & y \\ w & z \end{pmatrix}  =    \begin{pmatrix} e.x & e.y \\ e.w & e.z \end{pmatrix}
```
#### <b>Exemplo:</b><br>
``` R runnable
Mat = matrix(c(1, 2, 3, 4), nrow = 2)

Mat1 = matrix(c(2, 4, 6, 8), nrow = 2)

sub_mat =  Mat1 - Mat

print(sub_mat)

```
