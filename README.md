# Sobre

Este projeto usa o site : https://www.saucedemo.com/ com fins de demonstrar um teste    
E2E com login, carrinho de compras, cadastro de endereço, ilustrando todo o percurso  
de usuário dentro uma loja online.


# Como executar este projeto

Para executar o cypress:  

```sh
npx cypress open
```

para executar o teste

```sh
npm run test
```

## Test Case

**Supondo que a regra de negócio é a seguinte:**

Eu como usuário, quero logar na minha conta do Swag Labs, realizar compras ao meu critérios e recebê-los em minha casa.

**Requisitos:**  
* Logar com usuario valido  
* Os valores no carrinho de compras deve refletir o valor das peças adicionadas nele. 
* O usuário pode remover ou adicionar mais peças ao carrinho quantas   
vezes desejar.   
* No carrinho de compras ao clicar em checkout, o usuário deve ser encaminhado a uma tela para preencher suas informações postais.
* Ao clicar em continue o usuário deve ser encaminhado para uma tela de resumo das informações de compra e entrega.
* Ao clicar em finish deve aparecer uma mensagem confirmando a compra.
  
  
## Cenários de Login:

**1- Login** 
  1.1 Login com usuário válido e senha válida  
  1.2 Login com usuário inválido e senha válida
  1.3 Login com usuário válido e senha inválida

**2- Adicionar ao carrinho**  
   2.1 Clicar em vários produtos  
   2.2 Clicar no ícone de carrinho para
   ver se a quantidade e preço correspondem.    

**3- Remover do carrinho**  
   3.1 Dentro da página de carrinho clicar em remover vários produtos.  
   3.2 clicar Continue Shopping  
   3.3 Adicionar mais produtos  
   3.4 Clicar em carrinho  
   3.5 Dentro da página de carrinho verificar se a quantidade e preço correspondem.  

**4- Preencher formulário de checkout**  
    4.1 Na nova página preencher o formulário com código postal com letras  
    4.2 Na nova página preencher o formulário com código postal com números  
    4.3 Na nova página preencher o formulário com nome válido  
    4.4 Na nova página preencher o formulário com nome inválido  
    4.2 Clicar em finish    

**5- Exibe mensagem de confirmação**  
   5.1 Clicar em finish  
   5.2 Receber a mensagem de confirmação da compra.





