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


Logical Index Vector
A new vector can be sliced from a given vector with a logical index vector, which has the same length as the original vector. Its members are TRUE if the corresponding members in the original vector are to be included in the slice, and FALSE if otherwise.

For example, consider the following vector s of length 5.

> s = c("aa", "bb", "cc", "dd", "ee")
To retrieve the the second and fourth members of s, we define a logical vector L of the same length, and have its second and fourth members set as TRUE.

> L = c(FALSE, TRUE, FALSE, TRUE, FALSE) 
> s[L] 
[1] "bb" "dd"
The code can be abbreviated into a single line.

> s[c(FALSE, TRUE, FALSE, TRUE, FALSE)] 
[1] "bb" "dd"
