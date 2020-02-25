# Entrada e Saída em R

A linguagem R provê diferentes forma para realizar a entrada e saída de dados.

### Entrada de dados

O formato mais adequado para realizar a entrada de dados que pode ser efetuado através da importação de dados, quando estão armazenados em arquivos, ou digitados diretamente no R.

A função **scan()** é utilizada para realizar a leitura dos dados diretamente do teclado, isto é, coloca o R em modo prompt onde o usuário deve digitar 1 ou mais dados (vetor), cada um seguido da tecla **Enter**. Para encerrar a entrada de dados basta digitar **Enter duas vezes consecutivas**. 


Por padrão, a função **scan()** espera que os dados digitados sejam numéricos, mas desejando digitar outros tipos de dados utilize a função com o parâmetro **what** que pode ter os seguintes tipos de dados: **logical, integer, numeric, complex, character, raw e list**


Exercício:
Usando a função **scan()** crie variáveis para armazenar os seguintes valores:
1, 3, 9, 13, 18, 20, 25, 32 
1.0, 1.1, 1.2, 1.3, 1.4, 1.9
centro, tijuca, ilha do governador, leblon, ipanema
a, e, i, o, u
TRUE, TRUE, FALSE, FALSE, TRUE
