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
O índice Ibovespa é o principal indicador de desempenho do mercado de capitais brasileiro, nele é agrupado as empresas brasileiras mais importantes negociadas na B3.
Ele foi criado em 1968 e se tornou referência mundial para o mercado brasileiro.
Este estudo foi atualizado em 31 de agosto de 2021 sendo considerado a quantidade teórica reportada nesta data.
Os setores que compõem o indice são; Bens Indls, Consumo Não-Cíclico, Consumo Cíclico, Diverso, Financeiro e Outros, Mats Básicos, Petróleo, Saúde, Tec.Informação, Telecomunicação e Utilidade Públ.
Podemos observar que atualmente o setor de Financeiro possue maior relevância no índice seguido pelo setor de Materiais Básicos que juntos correspondem a aproximadamente 45%.

Abaixo temos as representações gráficas de sua composição.
![Gráfico de Rosca - Setores e Subsetores](https://user-images.githubusercontent.com/843826/131518825-67af5875-4c3d-43a9-9aa7-448e9600e21e.png)
![Gráfico de Árvore Setores e Sub Setores](https://user-images.githubusercontent.com/843826/131519236-883d181a-573b-4338-bf99-9cd165f66963.png)



