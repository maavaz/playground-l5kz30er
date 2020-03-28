### <b>Vetores</b>

### Nomeando os elementos do vetor
O R permite a associação de nomes aos elementos de um vetor.
 
#### Exemplos: 
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
