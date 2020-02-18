# Console do R

O **programa R** permite a sua utilização através de uma interface interativa. O **R** emite um prompt que espera comandos de entrada. O padrão
O prompt é '>', que no UNIX pode ser igual ao prompt do shell e, portanto, pode parecer que nada está acontecendo. No entanto, como veremos, é fácil mudar para um prompt R diferente se
Como desejar.

Pacotes no R

A linguagem R possui vários pacotes que, para instalá-los, basta digitar no console: 
install.packages("nome-do-pacote")
É necessário colocar as aspas para o pacote instalar. Uma vez instalado, o pacote não é carregado automaticamente.
Para carregar o pacote, basta digitar no console:
library(nome-do-pacote)
Agora as aspas não são necessárias.
Instalar pacote por pacote pode ser uma tarefa chata. Além do mais, isto exige que você saiba quais são
os pacotes que fazem cada coisa. Felizmente, o CRAN mantém coleções de pacotes de determinados temas,
chamados de Task Views. Existe um de econometria, e para instalar ele é necessário instalar o pacote ctv ,
e depois o task view de econometria:
