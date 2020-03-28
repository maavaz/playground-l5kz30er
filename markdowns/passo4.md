### <b>Operações com Matrizes (Continuação) </b>

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

Mat = matrix(c(2, 4, 6, 8), nrow = 2)

det_mat =  det(Mat)

print(det_mat)

```
### Inversa de uma Matriz

A inversa de uma matriz quadrada qualquer cujo determinante seja não nulo, A<sub>n,n</sub>, é uma matriz de mesmas dimensões que atenda a seguinte condição:
```math
A^{-1} \cdot A = I
```

Onde, I é a matriz identidade de mesma dimensão que a matriz A.<br>

A inversa de uma matriz é estimada pela função **solve()**, mesma função utilizada para resolução de sistemas de equações em R.

#### <b>Exemplo:</b><br>
``` R runnable

Mat = matrix(c(2, 4, 6, 8), nrow = 2)

inv_mat =  solve(Mat)

print(inv_mat)

```
### Traço de uma matriz

A soma dos elementos da diagonal de uma matriz quadrada define o traço de uma matriz. Assim, para uma matriz quadrada de ordem 2, o traço é determinado por:
```math
tr\begin{pmatrix} a & b\\ c & d \end{pmatrix} = a + d
```
Em R, a obtenção do traço passa pela extração dos elementos da diagonal da matrix, por meio da função diag(), e a soma destes elementos pela função sum(). <br>

#### <b>Exemplo:</b><br>
``` R runnable

Mat = matrix(c(2, 4, 6, 8), nrow = 2)

traco_mat =  sum(diag(Mat))

print(traco_mat)

```

### União matrizes
A união de matrizes é bastante importante para formarmos um conjunto de dados maior a partir de dados menores. Essa união pode ocorrer de duas formas: por linhas e por colunas. Para unirmos duas matrizes através das colunas, utilizamos a **função cbind()**. Já para fazer a união através das linhas, usamos a **função rbind()**.

#### <b>Exemplo:</b><br>
``` R runnable
Mat = matrix(c(1, 2, 3, 4), nrow = 2)
Mat1 = matrix(c(2, 4, 6, 8), nrow = 2)

cmat =  cbind(Mat,Mat1)

print(cmat)

rmat = rbind(Mat,Mat1)

print(rmat)

```

### Nomes das linhas e colunas em uma matriz
Dar nomes as linhas e colunas de uma matriz facilita a utilização e leitura dos dados de seus dados e, por conta disso, a linguagem R possui duas funções **rownames()** e **colnames()* para efetuar as operações de nomear as linhas e colunas, respectivamente. Uma vez com nomes das linhas e colunas, podemos utilizar os mesmos para realizar filtros na matriz. 

#### <b>Exemplo:</b><br>
``` R runnable

Mat = matrix(c(1000, -200, 120,-100, 250, -20, 300, 1000, 2000), ncol=3, nrow = 3)

# Renomeando as colunas e linhas da matriz
colnames(Mat) <- c("Jan", "Fev", "Mar")
rownames(Mat) <- c("Ana", "André", "Carlos")

print(Mat)

cat("\n")

# Para Exibir apenas as transaçoes realizadas pelo cliente André

trans = Mat["André",]
print(trans)

cat("\n")

# realiza a soma das transações por correntista (soma das linhas)
corr = rowSums(Mat)
print(corr)

cat("\n")

# realiza a soma das transações a cada mês (soma das colunas)
mes = colSums(Mat)
print(mes)

```
