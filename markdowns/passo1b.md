### Entrada de dados

A **função readLines()** é utilizada na entrada de dados quando os dados estão na forma de texto (strings). Cada linha (n > 1) é armazenada como um elemento de vetor e, por isso, podem ser acessadas por índice. O formato geral da função é dado abaixo: <br>
![excecao](/markdowns/imagens/readlines.png)
``` R
> texto <- readLines(n = 3)
Essa é a primeira linha
Essa é a segunda linha
Essa é terceira linha
> texto
[1] "Essa é a primeira linha" "Essa é a segunda linha" 
[3] "Essa é terceira linha"  
> texto[2]
[1] "Essa é a segunda linha"
> 
```

