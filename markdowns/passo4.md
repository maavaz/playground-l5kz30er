### <b>Operações com Matrizes (Continuação) </b>

### Multiplicação matricial
Essa operação corresponde a multiplicação entre uma matriz (n x m) por uma matriz (m x p),onde o número de colunas da primeira tem que ser igual ao número de linhas da segunda resultando em uma matriz de dimensões (n x p), cujos elementos são a somatório do produto entre os elementos em linha da primeira pelos elementos em coluna da segunda.<br>

```math
 \begin{pmatrix}  a & b \\ c & d  \end{pmatrix}  +  \begin{pmatrix} x & y \\ w & z \end{pmatrix}  =    \begin{pmatrix} a+x & b+y \\ c+w & d+z \end{pmatrix}
```
```math
\begin{pmatrix} a & b\\ c & d \end{pmatrix} \cdot \begin{pmatrix} x & y\\ g & h \end{pmatrix} = \begin{pmatrix} a \cdot e + b \cdot g & a \cdot y + b \cdot h\\ c \cdot x + d \cdot g & c \cdot y + d \cdot h \end{pmatrix}
```
#### <b>Exemplo:</b><br>
``` R runnable
Mat = matrix(c(1, 2, 3, 4), nrow = 2)

Mat1 = matrix(c(2, 4, 6, 8), nrow = 2)

soma_mat =  Mat + Mat1

print(soma_mat)

```
