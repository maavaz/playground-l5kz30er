### <b>Vetores</b>

### Nomeando os elementos do vetor
O R permite a associação de nomes aos elementos de um vetor.
 
#### Exemplos:
``` R runnable

vsaldo = c(100, 2000, -300, 3000, -200, 1200, 250, -100, 3200, 200, 1400, -150) 

# nomeia cada elemento de vsaldo
names(vsaldo) = c("jan", "fev", "mar", "abr", "mai", "jun", "jul", "ago", "set", "out", "nov", "dez") 
 
print (vsaldo)

#Pula Linha
cat("\n")

# seleciona o saldo do mês de março ("mar")
saldo <- vsaldo["mar"] 

print(saldo)

#Pula Linha
cat("\n")

# Seleção na ordem inversa
ultimo <- vsaldo[c("dez", "nov", "out")] 
   
print(ultimo)
```


### Fatiamento (Seleção) através de Índices Lógicos
Os elementos de um determinado vetor podem ser selecionados/fatiados a partir de um vetor lógico (índices) de mesma dimensão que o vetor original.  Os elementos são selecionados se o correspondente no vetor lógico for Verdade (True), do contrário não é selecionado.

#### Exemplos:
``` R runnable
vet <- c("aa", "bb", "cc", "dd", "ee")

vetlog <- c(FALSE, TRUE, FALSE, TRUE, FALSE) 

# Seleciona o segundo e quarto elementos de vet a partir de vetlog

print(vet[vetlog])

# Pula linha
cat("\n")

# a seleção pode ser feita sem a criação de vetlog 

print(vet[c(FALSE, TRUE, FALSE, TRUE, FALSE)]) 
```

### Algumas funções de manipulação de vetores
Abaixo apresentamos alguns exemplos de outras funções de manipulação de vetores. <br>

``` R runnable
vet1 <- c(4,1,2,3)
vet2 <- c(8,7,6,5)

# A função order() ordena o vetor em ordem crescente ou decrescente, mas exibe a ordenação pelos índices do vetor

vet3<- order(vet1, decreasing = FALSE)

cat("   ",vet1, "<-- vet1\n")
cat("   ",vet3, "<--ìndices ordenados vet1\n")

#Pula linha
cat("\n")

#Para exibir o vetor ordenado utiliza-se o operador [ ] que seleciona um elemento através da posição dele no vetor

vet3<- vet1[order(vet1, decreasing = FALSE)]

print(vet3)

# A função sort() ordena o vetor em ordem crescente ou decrescente, exibindo o vetor ordenado

vet3 <- sort(vet2, , decreasing = TRUE)

print(vet3)

#Pula linha
cat("\n")

# sum() retorna a soma dos elementos e cumsum() retorna a soma cumulativa dos elementos

cat ("   ",sum(vet1), "<-- Soma dos elemento de vet1\n")

#Pula linha
cat("\n")

cat ("   ",cumsum(vet1), "<-- Soma cumulativa dos elemento de vet1\n")

```

