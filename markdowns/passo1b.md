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

A linguagem R permite a leitura diretamente de arquivos (importação de dados) e o método mais comum de importação de dados é utilizando a **função read.table()**, cujo formato geral do comando é apresentado abaixo:<br>

![excecao](/markdowns/imagens/readtable.png)


Como exemplo,utilizaremos os dados do arquivo **"texte.txt"** no diretório de trabalho, com o seguinte formato:
campo1;campo2;campo3
01;"teste_campo1";"teste_campo3"
02;"teste1_campo1";"teste1_campo3"
No exemplo abaixo, utilizamos a **função readtable()** para efetuar a leitura desses dados e importá-los para a **variável tabela**:
``` R
> tabela <- read.table("teste.txt", header=TRUE,sep=";")
> tabela
  campo1        campo2        campo3
1      1  teste_campo1  teste_campo3
2      2 teste1_campo1 teste1_campo3

# A função str() exibe a estrutura do objeto tabela.
> str(tabela)
'data.frame':	2 obs. of  3 variables:
 $ campo1: int  1 2
 $ campo2: Factor w/ 2 levels "teste_campo1",..: 1 2
 $ campo3: Factor w/ 2 levels "teste_campo3",..: 1 2
```

