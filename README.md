
# 1. Sobre o Dataset
### Food and Goods Deliveries in Brazil
### O que é o Delivery Center

Com seus diversos hubs operacionais espalhados pelo Brasil, o Delivery Center é uma plataforma integra lojistas e marketplaces, criando um ecossistema saudável para vendas de good (produtos) e food (comidas) no varejo brasileiro.

Atualmente temos um cadastro (catálogo + cardápio) com mais de 900 mil itens, milhares de pedidos e entregas são operacionalizados diariamente com uma rede de milhares lojistas e entregadores parceiros espalhados por todas as regiões do país.

Tudo isso gera dados e mais dados a todo momento!

Diante disso, nosso negócio está cada vez data driven, ou seja, utilizando dados para tomar decisões e numa visão de futuro sabemos que utilizar os dados de forma inteligente pode ser o nosso grande diferencial no mercado.

# 2. Objetivo do Projeto
Neste projeto eu irei realizar a análise descritiva do Dataset  Delivery Center com o intuito de entender a eficiência dos centros de distribuição perante as lojas ou marketplaces as quais atende.

# 3. Pipeline de Solução
1.Compreensão do negócio  
2.Compreensão dos dados  
3.Preparação dos dados  
4.Análise  

# 4. Técnologias e ferramentas utilizadas
- Python (polars, pandas, matplotlib, seaborn, folium).  
- Estatísticas.  
- Limpeza, manipulação, visualização e exploração de dados.  

# 5. Insights
### - Cidades com maior quantidade de pedidos
![image](https://github.com/user-attachments/assets/0fedf7d9-6019-4415-b21a-e9bf7aec5ec4)

### -Quantidade de Centros de Distribuição X Quantidade de Lojas por Cidade
Centros de Distribuição
![image](https://github.com/user-attachments/assets/e549aa25-2c22-4a3c-945a-587bc58a5bd8) 
Lojas 
![image](https://github.com/user-attachments/assets/50dfa691-1b08-4398-bcf9-3ecd8b7a9994) 

### -Tempo total do pedido por cidade

![image](https://github.com/user-attachments/assets/18d52f16-3bf1-4149-a6a7-f559cb4ee6fd)

De modo geral, o tempo total é menor em Curitiba. Isso pode ter acontecido tanto pela cidade ser menor, como pelo centro de distribuição estar mais proximos dos pontos de entrega. De toda forma, não é uma diferença tão significante quando comparado com as outras cidades

### -Há preferência por tipo de transporte utilizado em cada cidade
![image](https://github.com/user-attachments/assets/15877ee5-db4d-4f64-bcc0-2c4a2aaaa71d)



O tipo de transporte de preferência é a Moto em sua totalidade. No entanto, no Rio de Janeiro é visto uma diferença menor entre o uso de bike e moto quando comparado com outras cidades.

### -Há relação entre o hub e os cancelamentos?
![image](https://github.com/user-attachments/assets/410187c6-03fc-48b5-af26-7b2c2d6e9293)

Há hubs nas cidades de Rio de Janeiro, São Paulo e Curitiba que possuem 100% dos pedidos cancelados, mas também são hubs com o menor número de pedidos. De modo geral, os cancelamentos não passam de 5%, o que demonstra uma certa eficiência dos hubs.

### -Há relação entre distância média dos pedidos com o cancelamento levando em consideração o tipo de transporte utilizado?
![image](https://github.com/user-attachments/assets/38845890-c35f-4910-baf2-545fd1363f1a)

Cancelamentos parecem não ter relação com o tipo de transporte utilizado, visto que a média de distância para bicicleta é menor para os dois tipos de Status.

### -E com o Tempo Total do Pedido?
![image](https://github.com/user-attachments/assets/ca9115f2-9904-450f-8e1f-3abacd6b48a7)

Aparentemente o tempo total do pedido tem relação com os cancelamentos, independente do tipo de transporte utilizado em cada cidade.

### -Quais fatores mais influenciam o tempo de entrega total?
![image](https://github.com/user-attachments/assets/69a3c33a-9a0e-432b-9b62-3790f53d6db5) ![image](https://github.com/user-attachments/assets/5b621769-3e30-45b3-9b70-dccfcaf10ab5)
![image](https://github.com/user-attachments/assets/c76c976e-06e9-4d92-9c8f-fef40132097c)


# 3. Conclusão

- Hubs por cidade  
A quantidade de hubs não esta diretamente relacionada com a quantidade de lojas presentes em cada cidade. A cidade de Curitiba é a cidade que possui uma maior desproporção de hubs por loja, possuindo quase que um hub por loja, e isso, não tem relação direta com a quantidade de pedidos gerados em cada cidade, logo que Curitiba é a cidade que possui menos pedidos,também sendo a menor em extensão.

- Cancelamentos  
De modo geral, não há preferência por tipo de transporte, com exceção da cidade do Rio de Janeiro que parece quase que igualar o uso dos dois tipos de transporte.

Sobre a distância a ser percorrida por cada tipo de transporte, parece não haver uma relação direta com cancelamentos. A unica relação que vemos com a distância é a de que o condutor que utiliza bicicletas parece sempre percorrer uma distância menor do que quem utiliza moto. Os pedidos mais curtos podem estar sendo direcionados para quem utiliza mais bicicletas do que motos.

Já o tempo total do pedido, desde a sua criação até a entrega tem uma relação com os cancelamentos, independente do tipo de transporte utilizado havendo também uma tolerância maior que 8 dias até o cancelamento.

- Tempo gasto em cada etapa  
Apesar da preparação do pedido levar um tempo consideravel, o tempo gasto no transporte acaba sendo consideravelmente maior que o de preparo e todas as outras etapas. Inclusive, nos pedidos com Status Cancelado é o que vemos a maior disparidade com relação aos finalizados, até mesmo para cidade de Curitiba que possui a maior quantidade de hubs por lojas. 

# 4. Considerações Finais

Será necessário análisar mais profundamente a quantidade de hubs por cidade, visto que a quantidade de hubs em Curitiba e em Porto Alegre são bem maiores, quando comparado com o número de lojas e pedidos, mas possuindo praticamente o mesmo nivel de eficiência dos outros hubs.

