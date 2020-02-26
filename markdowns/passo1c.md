### <b>Saída de dados</b>
As funções de saída de dados em R mostram uma série de argumentos. Aqui, apenas mostraremos as funções na sua forma mais básica. Sugerimos acessar o help() na console para ver as diversas formas de utilização dessas funções.<br>
A função **print()** é uma das principais funções para exibir valores na console do R.<br>
O formato geral da função é:<br>
                        ![excecao](/markdowns/imagens/printR.png) <br>

A função **cat()** mostra a saída no console dos argumentos depois de transformá-los em caracteres.<br>
O formato geral é:<br>
                         ![excecao](/markdowns/imagens/cat.png) <br>
                         
A função **format()** mostra na console uma saída formatada dos dados.<br>
O formato geral é:
![excecao](/markdowns/imagens/formatR.png) <br>
 
Para exportar objetos do R, pode-se usar a função **write.table()**, que possui argumentos parecidos com aqueles da função read.table().
A função write.table() é capaz de criar um arquivo de texto no formato txt ou csv, com as especificações definidas pelos argumentos.<br>
O formato geral é:<br>
![excecao](/markdowns/imagens/writetable.png) <br>

Note que o objeto a ser exportado deve estar em formato tabular, ou seja, uma matriz ou data frame. Outras classes de objetos podem ser exportadas, mas haverá uma transformação para data frame, o que pode fazer com que o resultado final não seja o esperado.<br>

Assim como read.table() possui as funções read.csv() e read.csv2(), a função write.table() possui as funções write.table() e write.table2() como wrappers. O comando acima também poderia ser executado como
