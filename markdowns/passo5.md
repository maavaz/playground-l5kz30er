# DataFrame em R
---
Até agora as estruturas de dados apresentadas (vetor e matriz) armazenam dados de um mesmo tipo. DataFrame são estruturas de dados tabulares, parecidos com as matrizes bi-dimensionais, mas podem ter diferentes tipos de dados em suas colunas, isto é, cada coluna contém valores variáveis de mesmo tipo e cada linha contém um conjunto de valores das diferentes colunas (um por coluna).
Os DataFrames possuem as seguintes características:
+ As colunas deve ter uma nome, não devem estar vazios.
+ Os nomes das linhas devem ser exclusivos (índices).
+ Os dados armazenados em um dataframe podem ser do tipo numérico, real ou caractere.
+ Cada coluna deve conter o mesmo número de itens de dados.
Exemplo:
table class="table table-condensed">
<thead>
<tr class="header">
<th align="left">nome</th>
<th align="left">altura</th>
<th>idade</th>
<th align="left">sexo</th>
<th align="left">peso</th>
<th align="left">fumante</th>
<th align="center">uf</th>
<th align="left">renda</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left">João</td>
<td align="left">1.80</td>
<td>22</td>
<td align="left">masculino</td>
<td align="left">78.3</td>
<td align="left">sim</td>
<td align="center">PB</td>
<td align="left">2</td>
</tr>
<tr class="even">
<td align="left">Pedro</td>
<td align="left">1.77</td>
<td>21</td>
<td align="left">masculino</td>
<td align="left">82.1</td>
<td align="left">não</td>
<td align="center">AL</td>
<td align="left">5</td>
</tr>
<tr class="odd">
<td align="left">Amanda</td>
<td align="left">1.71</td>
<td>18</td>
<td align="left">feminino</td>
<td align="left">66.5</td>
<td align="left">sim</td>
<td align="center">PE</td>
<td align="left">10</td>
</tr>
<tr class="even">
<td align="left">Fábio</td>
<td align="left">1.65</td>
<td>20</td>
<td align="left">masculino</td>
<td align="left">88.1</td>
<td align="left">não</td>
<td align="center">PE</td>
<td align="left">20</td>
</tr>
<tr class="odd">
<td align="left">Fernanda</td>
<td align="left">1.66</td>
<td>23</td>
<td align="left">feminino</td>
<td align="left">58.0</td>
<td align="left">sim</td>
<td align="center">SP</td>
<td align="left">10</td>
</tr>
<tr class="even">
<td align="left">Gustavo</td>
<td align="left">1.63</td>
<td>19</td>
<td align="left">masculino</td>
<td align="left">75.4</td>
<td align="left">não</td>
<td align="center">CE</td>
<td align="left">NA</td>
</tr>
</tbody>
</table>

``` R runnable
# Create the data frame.
emp.data <- data.frame(
   emp_id = c (1:5), 
   emp_name = c("Rick","Dan","Michelle","Ryan","Gary"),
   salary = c(623.3,515.2,611.0,729.0,843.25), 
   
   start_date = as.Date(c("2012-01-01", "2013-09-23", "2014-11-15", "2014-05-11",
      "2015-03-27")),
   stringsAsFactors = FALSE
)
# Print the data frame.			
print(emp.data) 
```
