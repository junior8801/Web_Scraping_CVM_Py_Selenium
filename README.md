## Web Scraping Composição do Índice Bovespa

### Objetivo
Realizar uma raspagem de dados do site da b3 para extração dos dados de composição do índice Bovespa para apresentação da representatividade dos setores e subsetores na compozição do índice Ibovespa.

### Libs
Utilizando as bibliotecas Kora, Selenium and Plotly Express. 

### DataSet
Fonte de Dados https://sistemaswebb3-listados.b3.com.br/indexPage/day/IBOV?language=pt-br

#### Variáveis
| Coluna | Descrição |
| --- | --- |
| Setor | Variável categórica com o Setor/Subsetor. |
| Código | Código de negociação do papel da empresa que é negociada no mercado de capitais. |
| Ação | Nome da empresa. |
| Tipo | Categoria de negociação da empresa, ON/PN. |
| Qtde. Teórica | Quantidade fisica teórica de papéis na composição do índice. |
| Part. (%) | Participação em percentual da empresa na composição do índice. |
| Part. (%)Acum. | Participação em percentual acumulado da empresa na composição do índice. |

### Preparação dos dados

Necessário incluir uma nova variável para separação do Setor e Sub setor, posteriormente o ajuste dos nomes dos Setores; "Cons N  Básico" e "Cons N Cíclico" para "Consumo Não-Cíclico", "Financ e Outros" para "Financeiro e Outros"

### Apresentação
![alt text](https://raw.githubusercontent.com/junior8801/Web_Scraping_CVM_Py_Selenium/blob/main/Gr%C3%A1fico%20de%20Rosca%20-%20Setores%20e%20Subsetores.png)

