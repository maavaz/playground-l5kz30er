### <b>Vetor (Continuação) </b>

### Nomeando os elementos do vetor
O R permite a associação de nomes aos elementos de um vetor.
 
> v = c("Mary", "Sue") 
> v 
[1] "Mary" "Sue"
We now name the first member as First, and the second as Last.

> names(v) = c("First", "Last") 
> v 
 First   Last 
"Mary"  "Sue"
Then we can retrieve the first member by its name.

> v["First"] 
[1] "Mary"
Furthermore, we can reverse the order with a character string index vector.

> v[c("Last", "First")] 
  Last  First 
 "Sue" "Mary"
