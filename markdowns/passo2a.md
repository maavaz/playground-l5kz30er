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
vet = c("aa", "bb", "cc", "dd", "ee")

vetlog= c(FALSE, TRUE, FALSE, TRUE, FALSE) 

# Seleciona o segundo e quarto elementos de vet a partir de vetlog

print(vet[vetlog])

# Pula linha
cat("\n")

# a seleção pode ser feita sem a criação de vetlog 

print(vet[c(FALSE, TRUE, FALSE, TRUE, FALSE)]) 
```
