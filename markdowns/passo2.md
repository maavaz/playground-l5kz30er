# Estruturas de Dados em R

Semelhante a diversas linguagens de programação, a <b>linguagem R</b> possui os seguintes tipos de dados mais comuns:
+ <b>Vetor</b>
+ <b>Matriz</b>
+ <b>Lista </b>
+ <b>Dataframe</b>

### <b>Vetor</b>

Um vetor é coleção unidimensional homogênena de dados (números, caracteres, strings). Para criar um vetor, use a **função c()**, com um número arbitrário de argumentos.

``` R runnable
# Criando o vetor vetx de números inteiros com 5 elementos
vetx <- c(1,2,3,4,5)
print(vetx)

#Pulando de Linha 
cat("\n")

# Criando o vetor vletra de caracteres com 3 elementos
vletra =  c('a', 'b', 'c')
print(vletra)

#Pulando de Linha 
cat("\n")

# Criando o vetor vreal do real com 4 elementos
assign("vreal", c(5.7, 3.3, 6.5, 7.7))
print(vreal)

#Pulando de Linha 
cat("\n")

# Criando um vetor com função rep() - repetição de valores e parâmetro each= informando que cada número deve ser repetido 3 x
numeros <- rep(1:3,each=3)
print(numeros)

```
### <b>Operações com vetores</b>
Podemos fazer operações aritméticas com vetores, como somar, subtrair, multiplicar e dividir.Essas operações são efetuadas elemento a elemento.
``` R runnable
# Criando o vetor de números inteiros ímpares
veti <- c(1,3,5)
print(veti)

#Pulando de Linha 
cat("\n")

# Criando o vetor de números pares a partir da operação soma
vetp =  veti + c(1, 1, 1)
print(vetp)

#Pulando de Linha 
cat("\n")

# Criando o vetor vreal do real com 4 elementos
vreal = c(5.7, 3.3, 6.5, 7.7) * 2
print(vreal)

#Pulando de Linha 
cat("\n")

# Criando um vetor de inteiros onde os elementos são potencias de base 2
vpot = c(2, 2, 2, 2) ** c(2, 3, 4, 5)
print(vpot)

#Pulando de Linha 
cat("\n")

# produto de 2 matrizes unidimensionais
vprod = c(1, 2, 3) %*% c(2, 3, 4)
print(vprod)

```

### Fatiamento (Slice) em vetores

Um vetor pode ser subdividido/fatiado (Slice) utilizando os índices numéricos que representam as posições dos elementos do vetor.  Os exemplos a seguir mostram essa técnica:

```R runnable

# Extrair do vetor s os elementos da 2º e 3º posições

s = c("aa", "bb", "cc", "dd", "ee") 
print( s[c(2, 3)]) 

cat("\n")

# Extração duplicando os elementos duplicados (extrai os elementos 1 ou + vezes. Extrai o elemento da 3ª posição 2 x

print(s[c(2, 3, 3)]) 

cat("\n")

Out-of-Order Indexes
The index vector can even be out-of-order. Here is a vector slice with the order of first and second members reversed.

> s[c(2, 1, 3)] 
[1] "bb" "aa" "cc"
Range Index
To produce a vector slice between two indexes, we can use the colon operator ":". This can be convenient for situations involving large vectors.

> s[2:4] 
[1] "bb" "cc" "dd"
More information for the colon operator is available in the R documentation.

> help(":")




