# Primeiros passos
**R** é uma linguagem de expressão com uma sintaxe muito simples. Como na linguagem Python, **R** faz distinção entre maiúsculas e minúsculas, portanto **A** e **a** são símbolos diferentes e se referem a variáveis diferentes. <br>


### <b>Variáveis</b>

Para um programa, escrito em uma linguagem qualquer, manipular os dados, estes precisam estar armazenados em locais da memória do computador. Esses locais usados para armazenar dados são denominados de **variáveis**. Por definição,

*As **Variáveis** representam locais de memória usados para armazenar, temporariamente, os dados(valores) que deverão ser utilizados durante a execução do programa ou na seção do terminal.*

Toda variável tem que ter:

+ <b>Um nome</b> - é como a variável será chamada ao guardar e recuperar os dados da memória. O nome deve seguir a regra descrita abaixo e;
+ <b>Um tipo</b> - esse tipo (inteiro, real etc.) é definido quando variável é criada, baseando-se nos dados a ela atribuído; 

#### <b>Regra de definição de nomes de variáveis:</b><br>
Os nomes de variáveis permitem todos caracteres alfanuméricos (e em alguns países isso inclui letras acentuadas) mais **.(ponto)** e **_ (sublinhado)**, com a restrição de que um nome comece (primeiro caracter) com **.(ponto)** ou **letra** e, se começar com **.(ponto)**, o segundo caracter **não** pode ser um **dígito**. Os nomes possuem tamanho ilimitado.

**OBS:** O comando **ls()** lista todas as variáveis/objetos criados pelo usuário em uma sessão. O comando **ls.str()** além de exibir as variáveis, exibe também a sua estrutura e seu conteúdo.

### <b>Comando de Atribuição</b>

O comando de atribuição tem a função de mover (atribuir) um valor para dentro de uma variável. Uma variável é criada no momento da execução do comando. O **R** pode usar quatro tipos/formas de representação do comando de atribuição, a saber:<br>
![atribuicao](/markdowns/imagens/atribuicao.png)

``` R
z <- 7                # Criando a variável z do tipo inteiro

10 -> x               # Criando a variável x do tipo inteiro

nome = "Marco"        # Criando a variável nome do tipo string

assign("preco", 1.99) # Criando a variável preco do tipo float(Real)
```
### <b>Operadores aritméticos</b>
Os operadores utilizados nas expressões aritméticas, são:<br>
<b>Operador&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Significado<br>
&nbsp;+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;adição<br>
&nbsp;-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;subtração<br>
&nbsp;*&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;multiplicação<br>
&nbsp;/&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;divisão<br>
&nbsp;^&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;potência<br>
&nbsp;exp()&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;exponencial<br>
&nbsp;sqrt()&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;raíz quadrada<br>
&nbsp;factorial()&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;fatorial<br>
&nbsp;log(); log2(); log10()&nbsp;&nbsp;logaritmos<br>
</b>

**OBS: A ordem de execução dos operadores tem o parênteses como a maior prioridade, seguido de Multiplicação (atenção !!), divisão, adição e a subtração como sendo a de menor Prioridade**<br>

<b>Exercícios</b><br>
*Utilize a console do R para executar as seguintes equações:*<br>
<b>a) 30 + 61 − 20 / 2 ?<br>
b) raiz quadrada da expressão de a) ?<br>
c) −24 + 5! ?<br>
d) logaritmo de c) ?<br>
</b>
### <b>Executando Comandos em R</b>

Os comandos em R podem ser executados diretamente na console do editor ou através de um arquivo de script (**extensão .R**) que pode ser executado comando a comando ou, caso deseje executar todos os comandos do script na sequência, utilizar a função **source()**. O formato geral simplificado do comando é apresentado abaixo:</br>
![excecao](/markdowns/imagens/source.png)

