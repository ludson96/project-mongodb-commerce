# Repositório do projeto Mongodb Commerce

## Módulo: BACK-END

 Repositório possuí projeto desenvolvido no período que estive na **Trybe**, abordando os conceitos **CRUD** completo em **MongoDB**.

## Informações de aprendizados

- Este é um projeto desenvolvido para me ajudar a aprender `Mongodb`;
- Meu primeiro projeto usando `Mongodb`;
- Utilizei a extensão do VSCode `MongoDB for VS Code` para realizar as operações.

## Linguagem usadas

[![Mongo][Mongo-logo]][Mongo-url]
[![Docker][Docker-logo]][Docker-url]
[![ESLint][ESLint-logo]][ESLint-url]

## O que foi desenvolvido

Neste projeto utilizamos o banco NoSQL MongoDb, manipulamos o banco de dados commerce, que contém dados do cardápio do McDonald's, como ingredientes, valores nutricionais e dados fictícios de vendas .

## Instruções para instalar e rodar

1. Clone o repo:

    ```bash
    git clone git@github.com:Ludson96/project-mongodb-commerce.git
    ```

1. Entre na pasta do repositório que você acabou de clonar:

    ```bash
    cd project-mongodb-commerce
    ```

1. Instale as dependências e inicialize o projeto:

    ```bash
    npm install
    ```

1. Caso queira utilizar o mongodb pelo docker execute o seguinte comando:

    ```bash
    docker run -d --name=nomeDoContainer -v "$PWD:/app" -p 27017:27017 mongo:5.0;
    ```

1. Utilize o arquivo do banco de dados no `assets` o `produtos.bson`

## Uso

Dentro da pasta `challenges` estão numerados comandos do mongodb, e logo abaixo seu respectivo desafio proposto pela **Trybe**.

## Desafios

<details>

### 1 - Retorne a quantidade de documentos inseridos na coleção `produtos`

- `desafio1.js`

### 2 - Ordene a coleção `produtos` pela quantidade de lanches vendidos em ordem crescente, mostrando apenas o `nome` e a quantidade de lanches `vendidos`

- `desafio2.js`

### 3 - Retorne o lanche mais vendido, mostrando apenas o `nome` e a quantidade do lanche mais vendido

- `desafio3.js`

### 4 - Retorne os lanches que tiveram vendas maiores que `50` e menores que `100`, mostrando apenas o nome e a quantidade de lanches `vendidos` em ordem crescente

- `desafio4.js`

### 5 - Retorne o `nome`, as `curtidas` e `vendidos` dos lanches que tiveram quantidade de `curtidas` igual a `36` ou tenham a quantidade de vendas igual a `85`

- `desafio5.js`

### 6 - Retorne o `nome` e as `curtidas` dos lanches que tiveram curtidas maiores que `10` e menores que `100`

- `desafio6.js`

### 7 - Retorne o `nome` e `vendidos` dos lanches que tenham sido `vendidos` com uma quantidade diferente de `50` e em que o campo `tags` não exista

- `desafio7.js`

### 8 - Delete os lanches com menos de `50` `curtidas` e retorne o `nome` dos lanches que restaram no banco

- `desafio8.js`

### 9 - Retorne o `nome` de todos os lanches que possuam `calorias` abaixo de `500`

- `desafio9.js`.

### 10 - Retorne o `nome` de todos os lanches que tenham o percentual de `proteínas` maior ou igual a `30` e menor ou igual a `40`

- `desafio10.js`

### 11 - Retorne o `nome` do produto, a quantidade de `curtidas` e quantos itens foram `vendidos` dos produtos que não sejam iguais a `Big Mac` e `McChicken`

- `desafio11.js`

### 12 - Adicione `ketchup` aos `ingredientes` para todos os sanduíches menos o `McChicken`, garantindo que não haja duplicidade nos `ingredientes`

- `desafio12.js` duas queries, **nesta ordem**:

1. Crie uma query que adicione `ketchup` aos `ingredientes` para todos os sanduíches menos o `McChicken`, garantindo que não haja duplicidade nos `ingredientes`.

2. Crie uma query que retorne o `nome` e `ingredientes` de todos os documentos.

### 13 - Inclua o campo `criadoPor` em todos os documentos, colocando `Ronald McDonald` no valor desse campo

- `desafio13.js` duas queries, **nesta ordem**:

1. Crie uma query que adicione o campo `criadoPor` em todos os documentos, colocando `"Ronald McDonald"` no valor desse campo.

2. Crie uma query que retorne o `nome` e `criadoPor` de todos os produtos.

### 14 - Crie uma query que retorne todos os lanches que possuem *picles* em seus ingredientes e mostre apenas os `3` primeiros itens contidos no array `valoresNutricionais`

- `desafio14.js`
- Sua query deve retornar apenas os campos `nome`, `ingredientes` e `valoresNutricionais`.

### 15 - Adicione o campo `avaliacao` em todos os documentos da coleção e efetue alterações nesse campo

- `desafio15.js` quatro queries, **nesta ordem**:

1. Crie uma query que inclua o campo `avaliacao` do tipo `NumberInt`, com o valor `0` em todos os documentos da coleção.

2. Crie uma query que incremente o valor do campo `avaliacao` em `5` em todos os sanduíches de carne do tipo `bovino`.

3. Crie uma query que incremente o valor do campo `avaliacao` em `3` em todos os sanduíches de `ave`.

4. Crie uma query que retorne o `nome` e `avaliacao` de todos os sanduíches.

### 16 - Adicione o campo `ultimaModificacao` com a data corrente somente no sanduíche `Big Mac`

- `desafio16.js` duas queries, **nesta ordem**:

1. Crie uma query que inclua somente ao sanduíche `Big Mac` o campo `ultimaModificacao` com a data corrente. Para a data corrente faça uso do tipo `date` ou `timestamp`.

2. Crie uma query que retorne o `nome` de todos os documentos em que o campo `ultimaModificacao` existe.

### 17 - Retorne a quantidade total de produtos em uma nova coleção chamada `resumoProdutos`

- `desafio17.js` duas queries, **nesta ordem**:

1. Crie uma query que insira na coleção `resumoProdutos` um documento com os campos: `franquia` com o valor `McDonalds` e `totalProdutos` com o valor sendo a quantidade total de produtos registrados na coleção `produtos`.

2. Crie uma query que retorne os campos `franquia` e o `totalProdutos` da coleção `resumoProdutos`, resultantes da primeira query.

### 18 - Inclua `bacon` no final da lista de `ingredientes` dos sanduíches `Big Mac` e `Quarteirão com Queijo`

- `desafio18.js` duas queries, **nesta ordem**:

1. Crie uma query que faça a inclusão de `bacon` no final da lista de `ingredientes` dos sanduíches `Big Mac` e `Quarteirão com Queijo`.

2. Crie uma query que retorne o `nome` e `ingredientes` de todos os documentos.

### 19 - Remova o item `cebola` de todos os sanduíches

- `desafio19.js` duas queries, **nesta ordem**:

1. Crie uma query que faça a remoção do item `cebola` em todos os sanduíches.

2. Crie uma query que retorne o `nome` e `ingredientes` de todos os documentos.

### 20 - Remova o primeiro `ingrediente` do sanduíche `Quarteirão com Queijo`

- `desafio20.js` duas queries, **nesta ordem**:

1. Crie uma query que faça a remoção do **primeiro** `ingrediente` no sanduíche `Quarteirão com Queijo`.

2. Crie uma query que retorne o `nome` e `ingredientes` de todos os documentos.

### 21 - Remova o último `ingrediente` do sanduíche `Cheddar McMelt`

- `desafio21.js` duas queries, **nesta ordem**:

1. Crie uma query que faça a remoção do **último** `ingrediente` no sanduíche `Cheddar McMelt`.

2. Crie uma query que retorne o `nome` e `ingredientes` de todos os documentos.

### 22 - Adicione a quantidade de vendas dos sanduíches por dia da semana

- `desafio22.js` quatro queries, **nesta ordem**:

1. Crie uma query que inclua um campo `vendasPorDia` em todos os sanduíches. O valor deste campo deverá ser um **array** com sete posições. Cada uma delas representará um dia da semana, e cada posição iniciará em `0`. O **array** deve seguir a estrutura do exemplo abaixo:

    ```json
    "vendasPorDia": [0, 0, 0, 0, 0, 0, 0]
    ```

    > O primeiro item desse **array** representa as vendas no **domingo**, o segundo item representa as vendas na **segunda-feira**, e assim sucessivamente até chegar ao último item, que representa as vendas no **sábado**.

1. Crie uma query que incremente as vendas de `Big Mac` às **quartas-feiras** em `60`.

1. Crie uma query que incremente as vendas de todos os sanduíches de carne do tipo `bovino` aos **sábados** em `120`.

1. Crie uma query que retorne o `nome` e `vendasPorDia` de todos os documentos.

### 23 - Insira os valores `combo` e `tasty` no **array** `tags` de todos os sanduíches e aproveite para deixar os valores em ordem alfabética ascendente (A a Z)

- `desafio23.js` duas queries, **nesta ordem**:

1. Crie uma query que faça tanto a inserção dos valores `combo` e `tasty` no **array** `tags` de todos os sanduíches. Ordene os valores de `tags` em ordem alfabética ascendente.

2. Crie uma query que retorne o `nome` e `tags` de todos os documentos.

### 24 - Ordene em todos os documentos os valores do **array** `valoresNutricionais` pelo campo `percentual` de forma decrescente

- `desafio24.js` duas queries, **nesta ordem**:

1. Crie uma query que faça em todos os documentos a ordenação dos valores do **array** `valoresNutricionais` pelo campo `percentual` de forma decrescente.

2. Crie uma query que retorne o `nome` e `valoresNutricionais` de todos os documentos.

### 25 - Adicione o valor `muito sódio` ao final do **array** `tags` nos produtos em que o `percentual` de `sódio` seja maior ou igual a `40`

- `desafio25.js` duas queries, **nesta ordem**:

1. Crie uma query que faça a adição do valor `muito sódio` ao final do **array** `tags` nos produtos em que o `percentual` de `sódio` seja maior ou igual a `40`.

2. Crie uma query que retorne o `nome` e `tags` de todos os documentos.

### 26 - Adicione o valor `contém sódio` ao final do **array** `tags` nos produtos em que o `percentual` de `sódio` seja maior do que `20` e menor do que `40`

- `desafio26.js` duas queries, **nesta ordem**:

1. Crie uma query que faça a adição do valor `contém sódio` ao final do **array** `tags` nos produtos em que o `percentual` de `sódio` seja maior do que `20` e menor do que `40`.

2. Crie uma query que retorne o `nome` e `tags` de todos os documentos.

### 27 - Conte quantos produtos contém `Mc` no nome, sem considerar letras maiúsculas ou minúsculas

- `desafio27.js`

### 28 - Conte quantos produtos têm `4` ingredientes

- `desafio28.js`

### 29 - Renomeie o campo `descricao` para `descricaoSite` em todos os documentos

- `desafio29.js` duas queries, **nesta ordem**:

1. Crie uma query que faça a renomeação do campo `descricao` para `descricaoSite` em todos os documentos.

2. Crie uma query que retorne o `nome` e `descricaoSite` de todos os documentos.

### 30 - Remova o campo `curtidas` do item `Big Mac`

- `desafio30.js` duas queries, **nesta ordem**:

1. Crie uma query que faça a remoção do campo `curtidas` do item `Big Mac`.

2. Crie uma query que retorne o `nome` para todos os documentos e `curtidas` (exceto para `Big Mac`).

### 31 - Retorne o `nome` dos sanduíches em que o número de `curtidas` é maior que o número de sanduíches `vendidos`

- `desafio31.js`

### 32 - Retorne o `nome` e a quantidade de vendas (`vendidos`) dos sanduíches em que o número de vendas é múltiplo de `5`

- `desafio32.js`

</details>

^[1] `produtos.bson` fornecidos pela Trybe.

[Mongo-url]:https://www.mongodb.com/
[Mongo-logo]: https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white
[Docker-logo]: https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white
[Docker-url]: https://www.docker.com
[ESLint-logo]: https://img.shields.io/badge/ESLint-4B3263?style=for-the-badge&logo=eslint&logoColor=white
[ESLint-url]: https://eslint.org/
