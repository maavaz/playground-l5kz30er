# Entrada e Saída em R

A linguagem R provê diferentes forma para realizar a entrada e saída de dados.

### Entrada de dados

O formato mais adequado para realizar a entrada de dados que pode ser efetuado através da importação de dados, quando estão armazenados em arquivos, ou digitados diretamente no R.

A função **scan()** é utilizada para realizar a leitura dos dados diretamente do teclado, isto é, coloca o R em modo prompt onde o usuário deve digitar 1 ou mais dados (vetor), cada um seguido da tecla **Enter**. Para encerrar a entrada de dados basta digitar **Enter duas vezes consecutivas**. <br>
**Formato Geral**<br>
![excecao](/markdowns/imagens/scan.png)
``` R
veta <- scan()
1: 2
2: 4
3: 6
4: 8
5:  
Read 4 items

print(veta)
[1] 2 4 6 8

# Podemos entrar uma sequência em apenas 1 linha
veta <- scan()
1: 2 4 6 8
2:
Read 4 items
```
Por padrão, a função **scan()** espera que os dados digitados sejam numéricos, mas desejando digitar outros tipos de dados utilize a função com o parâmetro **what** que pode ter os seguintes tipos de dados: **logical, integer, numeric, complex, character, raw e list** <br>
![excecao](/markdowns/imagens/scanwhat.png)
<br>
``` R
> vetlet <-scan(what="character")
1: a
2: e
3: i
4: o
5: u
6: > 
 
Read 5 items
> vetlet
[1] "a" "e" "i" "o" "u"
```

### Exercício:<br>
```
Usando a função scan() crie variáveis para armazenar os seguintes valores:<br>
1, 3, 9, 13, 18, 20, 25, 32 <br>
1.0, 1.1, 1.2, 1.3, 1.4, 1.9 <br>
centro, tijuca, ilha do governador, leblon, ipanema<br>
TRUE, TRUE, FALSE, FALSE, TRUE<br>
```
