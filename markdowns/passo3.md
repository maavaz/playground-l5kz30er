### <b>Operações com Matrizes</b>

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



