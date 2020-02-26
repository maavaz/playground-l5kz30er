### Saída de dados

A função **print()** é uma das principais funções para exibir valores na console do R.<br>
O formato geral da função é:<br>
                        ![excecao](/markdowns/imagens/printR.png)


Usando a função write.table()
Para exportar objetos do R, usamos a função write.table(), que possui argumentos parecidos com aqueles da função read.table().

A função write.table() é capaz de criar um arquivo de texto no formato txt ou csv, com as especificações definidas pelos argumentos.

Para ilustrar o uso desta função, considerer o conjunto de dados iris

data(iris)
str(iris)
'data.frame':   150 obs. of  5 variables:
 $ Sepal.Length: num  5.1 4.9 4.7 4.6 5 5.4 4.6 5 4.4 4.9 ...
 $ Sepal.Width : num  3.5 3 3.2 3.1 3.6 3.9 3.4 3.4 2.9 3.1 ...
 $ Petal.Length: num  1.4 1.4 1.3 1.5 1.4 1.7 1.4 1.5 1.4 1.5 ...
 $ Petal.Width : num  0.2 0.2 0.2 0.2 0.2 0.4 0.3 0.2 0.2 0.1 ...
 $ Species     : Factor w/ 3 levels "setosa","versicolor",..: 1 1 1 1 1 1 1 1 1 1 ...
Podemos exportar esse data frame com

write.table(iris, file = "dados/iris.csv")
Por padrão, o arquivo resultante tem colunas separadas por espaço, o separador de decimal é ponto, e os nomes das linhas são também incluídos (o que geralmente é desnecessário). Para alterar essa configuração podemos fazer

write.table(iris, file = "dados/iris.csv", row.names = FALSE,
            sep = ";", dec = ",")
Os argumentos são

iris: o nome do objeto a ser exportado (matriz ou data frame)
"iris.csv": nome do arquivo a ser gerado. (Considerando que o arquivo iris.csv será criado dentro do diretório dados).
row.names = FALSE: para eliminar o nome das linhas do objeto (geralmente desnecessário), como retornado por row.names()
sep = ";": o separador de colunas (também pode ser ",", "\t" para tabulação e "" para espaços)
dec = ",": o separador de decimais (também pode ser ".")
Note que o objeto a ser exportado (nesse caso iris) deve ser em formato tabular, ou seja, uma matriz ou data frame. Outras classes de objetos podem ser exportadas, mas haverá uma coerção para data frame, o que pode fazer com que o resultado final não seja o esperado.

Assim como read.table() possui as funções read.csv() e read.csv2(), a função write.table() possui as funções write.table() e write.table2() como wrappers. O comando acima também poderia ser executado como
