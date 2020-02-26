# Estruturas de Dados em R

Semelhante a diversas linguagens de programação, a linguagem R possui os seguintes tipos de dados mais comuns:
+ Vetor
+ Matriz
+ Lista 
+ Dataframe

### <b>Vetor</b>

Um vetor é coleção unidimensional homogênena de dados (números, caracteres, strings). Para criar um vetor, use a função **c()**, com um número arbitrário de argumentos.

``` R runnable
# Criando o vetor vetx de números inteiros com 5 elementos
vetx <- c(1,2,3,4,5)
print(vetx)

# Criando o vetor vletra de caracteres com 3 elementos
vletra =  c('a', 'b', 'c')
print(vletra)

# Criando o vetor vreal do real com 4 elementos
assign("vreal", c(5.7, 3.3, 6.5, 7.7))
print(vreal)
```
### <b>Operações com vetores</b>
Podemos fazer operações aritméticas com vetores, como somar, subtrair, multiplicar e dividir.Essas operações são efetuadas elemento a elemento.
``` R runnable
# Criando o vetor de números inteiros ímpares
veti <- c(1,3,5)
print(veti)

# Criando o vetor de números pares a partir da operação soma
vetp =  veti + c(1, 1, 1)
print(vetp)

# Criando o vetor vreal do real com 4 elementos
vreal = c(5.7, 3.3, 6.5, 7.7) * 2
print(vreal)

# Criando um vetor de inteiros onde os elementos são potencias de base 2
vpot = c(2, 2, 2, 2) ** c(2, 3, 4, 5)
print(vpot)

# produto de 2 matrizes unidimensionais
vprod = c(1, 2, 3) %*% c(2, 3, 4)
print(vprod)

```
### <b>Matrizes</b>

Matrizes são generalizações multidimensionais de vetores, isto é, possuem mais de uma dimensão. São vetores que podem ser indexados por dois ou mais índices e serão impressos em especial maneiras. Em R, as matrizes são criadas pela função **matrix()**. O formato geral é:<br>
                      ![excecao](/markdowns/imagens/matrix.png)


``` R runnable
# Criando a matriz 2x2 matx 
matx <- matrix(c(1,2,3,4),ncol = 2)
print(matx)

#Pulando de Linha 
cat("\n")

# Criando a matriz 3x3 maty
maty <- matrix(c(10,100,1000, 20, 200, 2000, 30, 300, 3000),ncol = 3)
print(maty)

#Pulando de Linha 
cat("\n")

# Criando uma matriz 3 X 3 com números inteiros gerados de 1 até 9 

matx <- matrix(data = 1:9, nrow=3 ,ncol = 3)
print(matx) 

#Pulando de Linha 
cat("\n")

# Criando a matriz 3 X 3 com números inteiros gerados de 1 até 9, mas  organizados por linha  (byrow)

matz <- matrix(data = 1:9, nrow=3 ,ncol = 3, byrow=TRUE)
print(matz) 

```

Para realizarmos o produto de 2 vetores utilizamos o operador **%*%**. Por exemplo:


