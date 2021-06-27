# Fast and Furries

 <img src="/src/image/logo.png">

Projeto da disciplina Introdução ao Desenvolvimento Web - SCC0219.

O tema escolhido por nós foi desenvolver um website de um petshop virtual.

### Autores

| NUSP     | Nome                       |
|----------|----------------------------|
| 10851687 |	Débora Buzon da Silva      |
| 11275147	| Dikson Ferreira dos Santos |
| 10716960	| Fernando de Souza Lincoln  |

### Tabela de conteúdos 

- [1. Requisitos](#1-requisitos)
- [2. Descrição do Projeto](#2-descrição-do-projeto)
- [3. Comentários sobre o código](#3-comentários-sobre-o-código)
- [4. Plano de teste](#4-plano-de-teste)
- [5. Resultados dos testes](#5-resultados-dos-testes)
- [6. Building](#6-building)
- [7. Problemas](#7-problemas)
- [8. Comentários](#8-comentários)

## 1. Requisitos

O sistema deve ter 2 tipos de usuários: clientes e administradores (o segundo ainda precisa ser implementado).

Os administradores são responsáveis por registrar/gerenciar administradores, clientes e produtos fornecidos. O aplicativo já vem com uma conta `admin` com senha `admin`.

Clientes são usuários que acessam o sistema para comprar produtos.

O registro do administrador contém nome, CPF, telefone e e-mail.

O registro de cada cliente contém nome, CPF, endereço, telefone e e-mail.

Os registros de produto incluem nome, id, foto, descrição, preço, quantidade em estoque e quantidade vendida.

Venda de produtos: Os produtos são selecionados, são incluídos em um carrinho e sua quantidade escolhida. Os produtos são comprados usando um número de cartão de crédito (qualquer número é aceito pelo sistema). A quantidade de produto vendida é subtraída da quantidade em estoque e adicionada à quantidade vendida. Os carrinhos são esvaziados somente quando o pagamento é efetuado ou quando os clientes removem todos os produtos.

Gerenciamento de produto: os administradores podem [criar/atualizar/ler/excluir](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete) novos produtos. Por exemplo, eles podem alterar a quantidade em estoque.

Nosso sistema, como funcionalidade extra, também terá um teste de personalidade em forma de quiz, que de acordo com as respostas dos usuários, escolherá um animal que mais se encaixa com o seu perfil.

O sistema é responsivo e visa uma boa acessibilidade e usabilidade para seus usuários.

## 2. Descrição do Projeto

Fast & Furries é um petshop virtual, implementado com HTML, CSS e JavaScript (até agora), que vende produtos destinados ao cuidado e ao lazer de bichinhos de estimação, como brinquedos, acessórios, caminhas e muito mais.

### Diagrama de navegação:

<img src="https://github.com/dbuzon/ProjetoWeb/blob/master/mockups/navigationDiagram.png" width=600px>

As imagens do mockup estão na pasta `/mockups`. 
Também pode ser acessado nos links abaixo:
- [Homepage](/mockups/Homepage.png)
  - [Produto](/mockups/Produto.png)
- [Login](/mockups/Login.png)
- [Perfil do Cliente](/mockups/PerfildoCliente.png)
- [Carrinho](/mockups/carrinho.png)
  - [Finalizar Compra](/mockups/FinalizarCompra.png)

### Funcionalidades

As funcionalidades visadas pelo nosso site são:

- Login com email e senha na plataforma, com opção de criar uma nova conta.
- Visualização das informações do cliente, com opção de alterar cadastro.
- Visualização da página de administrador, com opção de administrar os produtos e usuários da loja.
- Acesso à homepage, com visualização de alguns produtos selecionados pela loja.
- Visualização de um produto, com seu nome, descrição, preço e botão para adicionar ao carrinho.
- Acesso ao carrinho de compras, com opção de mudar a quantidade de itens, conferir o preço total e finalizar compra.
- Opção de inserir informações do cartão de crédito para efetuar o pagamento.
- Opção de alterar o endereço de entrega.
- Um teste de personalidade animal com perguntas de múltiplas respostas  

### Servidor

As informações salvas no servidor são as que estão descritas na parte **1. Requisitos**.

## 3. Comentários sobre o código

Usamos bootstrap para facilitar a implementação de um layout responsivo.

## 4. Plano de teste

Nosso projeto foi desenvolvido e testado no Firefox e no Google Chrome, dois navegadores muito populares no mercado.
Não utilizamos cookies no projeto, então cada vez que a página é recarregada, as informações são perdidas (por isso que o carrinho fica sempre com 3 produtos quando a página é recarregada, mesmo que removam ou adicionem itens nele). 

## 5. Resultados dos testes

O comportamento do site apresenta ser satisfatório nos dois navegadores testados, tendo em vista as limitações indicadas. 

## 6. Building

Para visualização do site, somente é necessário que esse repositório seja baixado. O acesso a cada página individual pode ser realizado abrindo o arquivo HTML correspondente no seu navegador preferido - As condições de teste estão indicadas na parte **4. Plano de teste**

## 7. Problemas

- Certa dificuldade de traduzir as imagens do mockup para código HTML e CSS, por causa da falta de padronização do tamanho das fontes entre as telas feitas no mockup.
- Tempo gasto no aprendizado de novas tecnologias, como bootstrap 
- Algumas coisas específicas de implementação de cada navegador tornam alguns bugs difíceis de serem identificados. Por exemplo, [Array.sort se comporta diferentemente em diferentes navegadores.](https://stackoverflow.com/questions/55039157/array-sort-behaves-differently-in-firefox-and-chrome-edge)

## 8. Comentários

Os mockups foram feitos usando a ferramenta Figma.
