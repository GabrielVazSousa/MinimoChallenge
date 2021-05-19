## MinimoChallenge
Desafio de Programação - Minimo 2021


Olá!! Tudo bem com vocês? 

Se você está aqui, provavelmente está participando do processo seletivo da Minimo! Seja muito bem-vindo, e esperamos que gostem do desafio que vamos propôr. Pensamos esta etapa como meio de tornar esta experiência mais construtiva para vocês e também para nos ajudar a avaliar o fit de vocês com a empresa!

Como dissemos na descrição da vaga no site da Preparo, nós não esperamos nenhum conhecimento técnico prévio de nenhum dos candidatos. Mas uma coisa que valorizamos muito por aqui, é a **capacidade de aprender** e a **autonomia** de cada um. No dia a dia da empresa vocês irão se deparar com inúmeras situações em que vocês terão que:

* entender uma necessidade do cliente
* converter esta necessidade em requisitos técnicos
* pesquisar a melhor maneira cumprir com os requisitos
* Implementar uma solução aplicando o que pesquisou
* Apresentar ao cliente o resultado obtido e coletar feedbacks
* Realizar os ajustes necessários e colocar em produção
* Monitoramento e manutenção da solução 
* Prospecção de novas oportunidades 

Pensando nisso, desenvolvemos este desafio, que consta de uma pequena simulação do processo descrito acima. Na maioria dos casos, não nos prendemos a uma tecnologia ou metodologia específica para solucionar nossos problemas. Porém, dado o contexto atual, uma das maneiras mais eficientes e coerentes de solucionar problemas é por meio da utilização de software! Por isso, no desafio de hoje, vocês utilizarão esta ferramenta principal. Chega de papo, e vamos logo para a descrição do case! 

# O Desafio
## Descrição do case
Imagine-se trabalhando para um determinado cliente da Minimo, cuja área de atuação é o **e-commerce**, chamado **Vendas Mil**. Este cliente ele possui diversos parceiros de logística para entregar os seus prdutos na casa de seus clientes, e cada parceiro possui uma maneira diferente de calcular o preço cobrado pelo envio dos pedidos. Um deles é o **Logistica Inteligente** e ele cobra do **Vendas Mil** por meio de duas frentes diferentes: Logística e Frete. A soma das duas frentes compõe o preço final que será cobrado por pedido. O preço é composto da seguinte regra: 

### Custo de Logística:
O custo de logística é o preço cobrado para receber, empacotar, armazenar e enviar os pedidos. Basicamente, ele depende do peso e das dimensões do produto e da quantidade de itens comprados. As instruções de cobrança foram enviadas pelo forncedor e foram baseadas em uma simulação de 150 pedidos contendo de 1 a 2 unidades de produto por pedido. Segue o e-mail: 

![image](https://user-images.githubusercontent.com/53821307/118822844-e0b8b400-b88e-11eb-803d-46b130d6bf49.png)
 
observações:
 * Considere que o 

### Custo de Frete:
O custo de frete é o preço cobrado para levar o pedido até a casa do comprador. Ele é calculado com base no CEP do comprador e do peso total do pacote a ser enviado. Para calcular o preço do frete, é necessário consultar as tabelas em csv disponibilizadas neste repositório dentro da pasta "CSVs". 

Basicamente basta consultar a coluna "Geografia Comercial" para determinado intervalo de "CEP Inicial" e "CEP Final" que contém o CEP do comprador no arquivo "codigo-por-cep.csv". E então consultar qual o preço para o código encontrado no processo anterior e peso do total do pedido no arquivo "preco-por-codigo-e-peso.csv". 

## Regras
Faça um fork deste repositório e desenvolva um software para automatizar o cálculo do preço que será cobrado por pedido utilizando sua tecnologia de preferência (python, javascript, c#, Excel, etc.).

O programa que você desenvolver deve ter como **entrada** os seguintes **parâmetros**: 

* largura, profundidade e altura para cada unidade de produto em **metros**
* peso de cada unidade do produto em **gramas**
* Quantidade comprada (un. de produtos) 
* CEP de entrega

E deve ter como **saída** o preço que será cobrado por pedido. 

### Casos de teste
O seu software que você desenvolver dar a mesma resposta para os casos descritos abaixo:

#### Caso 1:
**Parâmetros**: 
* Peso do produto: 250g
* Dimensões do produto: 0,2 x 0,2 x 0,3m
* Quantidade do pedido: 2un.
* CEP: 05612-050 

**Saída esperada**:
* R$XX,XX
 
