# Teste de Softwre (Neurotech) 

## Desafio  

- 1- Acessar o site www.americanas.com
- 2- Buscar por "PS4"
- 3- Selecionar o Primeiro console
- 4- Digitar o CEP e imprimir os valores dos fretes disponíveis
- 5- Clicar em comprar
- 6- Selecionar garantia +12meses
- 7- Clicar em continuar
- 8- Verificar se o produto se encontra na cesta

## Ferramenta Utilizada 

Para a realização do teste da aplicação web, foi utilizado a ferramenta SELENIUM  (IDE) que é um ambiente integrado de desenvolvimento para scripts de testes automatizados.

## Descrição  da Realização do teste 

Primeiro passo foi abrir o site www.americanas.com.br
```
Comando: Open
```
Em seguida, digitar o produto que deseja ser pesquisado na barra de pesquisa, nesse caso "PS4"
``` 
Comando: type  
alvo:id=h_search-input 
Valor: PS4
``` 
Selecionar o produto desejado "PS4"
``` 
Comando: click at 
alvo: css=.row > .product-grid-item:nth-child(1) .TitleUI-bwhjk3-15 
```
Clicar na caixa de calcular o frete, inserindo o cep. 
```
Comando: click
Alvo: css=.address__TextUI-sc-1a6a0ss-0
```
Digitar o valor do cep
```
Comando: type
Alvo: id=freight-field
Valor: 56328-310
```
Clicar no botão "OK" para imprimir o valor do frete
``` 
Comando: click
Alvo: css=#freight-field-button .TextUI-sc-1i9za0i-4
```
Clicar no botão continuar para ir para a próxima página da compra 
``` 
Comando: click
Alvo: css=.bdJeMR
```
Escolher a opção de garantia de (+12 meses)
```
Comando: Click
Alvo: css=.ColUI-gjy0oc-0:nth-child(3) .LabelUI-sc-1x9td29-0
```
Clicar no botão continuar para ir para o carrinho de compras 
```
Comando: Click
Alvo: css=.Wrapper-sc-1i9za0i-3
```
Verificar se o produto que foi escolhido se encontra na cesta de compras
``` 
Comando: verify element present
Alvo: linkText=Console Playstation 4 Hits 1TB Bundle 10 - Gran Turismo + Death Stranding + The Last of Us - PS4
``` 
