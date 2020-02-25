# Estruturas de Dados em R

Semelhante a diversas linguagens de programação, a linguagem R possui os seguintes tipos de dados mais comuns:
+ Vetor
+ Matriz
+ Lista 
+ Dataframe

### Vetor

Um vetor é coleção unidimensional homogênena de dados (números, caracteres, strings). Para criar um vetor, use a função **c()**, com um número arbitrário de argumentos.

``` R runnable
# Criando o vetor vetx de números inteiros com 5 elementos
vetx <- c(1,2,3,4,5)
print(vetx)

# Criando o vetor vletra de caracteres com 3 elementos
vletra <- c('a', 'b', 'c')
print(vletra)

# Criando o vetor vreal do real com 4 elementos
assign("vreal", c(5.7, 3.3, 6.5, 7.7))
print(vreal)
```
### Operações com vetores
