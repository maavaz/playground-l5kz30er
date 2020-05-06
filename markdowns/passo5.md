# DataFrame em R
---
Até agora as estruturas de dados apresentadas (vetor e matriz) armazenam dados de um mesmo tipo. DataFrame são estruturas de dados tabulares, parecidos com as matrizes bi-dimensionais, mas podem ter diferentes tipos de dados em suas colunas, isto é, cada coluna contém valores variáveis de mesmo tipo e cada linha contém um conjunto de valores das diferentes colunas (um por coluna).
Os DataFrames possuem as seguintes características:
+ As colunas deve ter um nome, não devem ser vazios.
+ Os nomes das linhas devem ser exclusivos (índices).
+ Os dados armazenados em um dataframe podem ser do tipo numérico, real ou caractere.
+ Cada coluna deve conter o mesmo número de itens de dados. <br>
Observe o DataFrame a seguir onde cada coluna representa um tipo de dados referente as informações dos alunos e cada linha representa um aluno:<br>
<table class="table table-condensed">
<thead>
<tr class="header">
<th align="center">nome</th>
<th align="center">altura</th>
<th>idade</th>
<th align="center">sexo</th>
<th align="center">peso</th>
<th align="center">uf</th>
<th align="center">renda (S.M.)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left">João</td>
<td align="center">1.70</td>
<td>22</td>
<td align="center">M</td>
<td align="center">78.3</td>
<td align="center">PB</td>
<td align="center">2</td>
</tr>
<tr class="even">
<td align="left">Pedro</td>
<td align="center">1.87</td>
<td>21</td>
<td align="center">M</td>
<td align="center">92.1</td>
<td align="center">AL</td>
<td align="center">5</td>
</tr>
<tr class="odd">
<td align="left">Ana</td>
<td align="center">1.69</td>
<td>18</td>
<td align="center">F</td>
<td align="center">66.5</td>
<td align="center">PE</td>
<td align="center">10</td>
</tr>
<tr class="even">
<td align="left">Teo</td>
<td align="center">1.75</td>
<td>20</td>
<td align="center">M</td>
<td align="center">88.1</td>
<td align="center">RJ</td>
<td align="center">20</td>
</tr>
<tr class="odd">
<td align="left">Fernanda</td>
<td align="center">1.66</td>
<td>23</td>
<td align="center">F</td>
<td align="center">58.0</td>
<td align="center">SP</td>
<td align="center">10</td>
</tr>
<tr class="even">
<td align="left">Gustavo</td>
<td align="center">1.73</td>
<td>19</td>
<td align="center">M</td>
<td align="center">75.4</td>
<td align="center">CE</td>
<td align="center">NA</td>
</tr>
</tbody>
</table>
O exemplo a seguir representa a criação do DataFrame (tabela) acima:<br>

```` R runnable
# Create the data frame.
alun.data <- data.frame( 
   alun_name = c("João","Pedro","Ana","Teo","Fernanda", "Gustavo"),
   alun_altu = c(1.7,1.87,1.69,1.75,1.66, 1.73), 
   alun_sexo = c('M', 'M', 'F', 'M', 'F', 'M'),
   alun_peso = c(78.3, 92.1, 66.5, 88.1, 58, 75.4),
   alun_sigla =c("PB", "AL", "PE", "RJ", "SP", "CE"),
   alun_renda = c(2, 5, 10, 20, 10, "NA"),
   stringsAsFactors = FALSE
)
# Print the data frame.			
print(emp.data) 

```
