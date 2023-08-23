# Data Lovers

## Índice

* [1. Preâmbulo](#1-preâmbulo)
* [2. Resumo do projeto](#2-resumo-do-projeto)
* [3. Definição de produto](#3-definição-de-produto)
* [4. Protótipos](#4-protótipos)
* [5. Testes de usabiliade](#5-testes-de-usabilidade)
* [6. Testes unitários](#6-testes-unitários)
* [7. Checklist](#7-checklist)
* [8. Ferramentas utilizadas](#8-ferramentas-utilizadas)
* [9. Desenvolvedoras](#9-desenvolvedoras)

***

## 1. Preâmbulo

Segundo a
[Forbes](https://www.forbes.com/sites/bernardmarr/2018/05/21/how-much-data-do-we-create-every-day-the-mind-blowing-stats-everyone-should-read),
90% dos dados que existem hoje foram gerados durante os últimos dois anos. A
cada dia geramos 2.5 milhões de terabytes de dados, uma cifra sem precedentes.

Apesar disso, os dados por si só são de pouca utilidade. Para que essas grandes
quantidades de dados se convertam em **informação** compreensível para os
usuários, precisamos entender e processar estes dados. Uma forma simples de
fazer isso é criando _interfaces_ e _visualizações_.

## 2. Resumo do projeto

Neste projeto construímos uma página web para visualizar um conjunto (set) de dados que se adéquem às necessidades do nosso usuário. Como itens essenciais, era necessária uma interface que permita visualizar dados, filtrá-los, ordená-los e fazer algum cálculo agregado.

Definimos nossa área de interesse diante dos temas propostos e procuramos entender quem seria nosso usuário e o que exatamente ele necessitaria saber ou ver, para assim conseguir construir uma interface que o ajude a interagir e entender melhor os dados.

Este foi nosso "dado" escolhido:

* [Pokémon](src/data/pokemon.json): Neste conjunto você encontrará uma
  lista com os 251 Pokémons da região de Kanto e Johto, com suas respectivas estatísticas utilizadas no jogo [Pokémon GO](http://pokemongolive.com).
  - [Pesquisa com jogadores de Pokémon Go](src/data/README.pt-BR.md)

O objetivo principal deste projeto foi aprender a desenhar e construir uma
interface web onde se possa visualizar e manipular dados, entendendo a necessidade do usuário.

## 3. Definição de produto

O projeto foi construído para jogadores de Pokémon GO. Onde os usuários pudessem ter uma série de informações dos pokémons para assim ajudá-los nas estratégias de jogo.

Com tais informações sua escolha será mais precisa na hora de jogar. Para auxiliar na busca, o projeto conta com a barra de pesquisa, o filtro por tipo, e a opção de ordenar.

### Para acessar o projeto **[clique aqui](https://adrianakatarina.github.io/Data-Lovers/)**

### Histórias de usuários

Para a execução do projeto, planejamos um protótipo capaz de suprir as necessidades de nosso público-alvo. Partindo das seguintes histórias de usuários:

1. Eu, como jogador novato de Pokémon Go, quero ter acesso a uma lista de pokémons para conhecê-los;

2. Eu como jogador de Pokémon Go, quero ter opção de filtrar por tipo para saber quais e quantos pokémons pertencem ao tipo especificado;

3. Eu, como jogador, quero organizar os pokémons em ordem alfabética e numérica para encontrá-los com mais facilidade;

4. Eu como mestre pokémon, quero saber quantos candies serão necessários para um pokémon evoluir;

5. Eu como jogador de Pokémon Go, quero uma barra de pesquisa para buscar rapidamente um pokémon específico.

Ao acessar o site, o usuário clica na pokebola e será direcionado para uma página com todos os cards de pokémons. Cada card possui na parte frontal informações como: peso, altura, raridade, e geração. Ao passar o mouse pelo card, o mesmo vira e irá trazer informações de: fraqueza, resistência, evoluções e quantos candies são necessários para sua evolução.


## 4. Protótipos

Uma vez tendo essas referências do tópico acima, seguimos para o desenvolvimento de dois protótipos. Um voltado para desktop e outro para mobile.

### Protótipo de Baixa Fidelidade

<div align="center">
  <h3>Protótipo web</h3>
  <img alt="Tela Home do Prototipo de Baixa Fidelidade" src="https://github.com/AdrianaKatarina/Data-Lovers/assets/122534293/b2ed2fe0-917c-4af6-a59e-79dc98496863" width="500" height="250"/>
  <img alt="Tela dos Pokemons do Prototipo de Baixa Fidelidade" src="https://github.com/AdrianaKatarina/Data-Lovers/assets/122534293/000eba84-1a6a-4051-9603-8bfeb178242f" width="500" height="250"/>

  <h3>Protótipo mobile</h3>
  <img alt="Tela mobile do Prototipo de Baixa Fidelidade" src="https://github.com/AdrianaKatarina/Data-Lovers/assets/122534293/3cd8b2d5-0197-4da9-9f02-92b48bdaa8e0" width="300" height="400"/>
</div>

### Protótipo de Alta Fidelidade

<div align="center">
  <h3>Protótipo web</h3>
  <img alt="Tela Home do Prototipo de Alta Fidelidade" src="https://github.com/AdrianaKatarina/Data-Lovers/assets/122534293/ce900532-56c6-4462-ae7d-d026c1b87844" width="500" height="300"/>
  <img alt="Tela inicial card-front do Prototipo de Alta Fidelidade" src="https://github.com/AdrianaKatarina/Data-Lovers/assets/122534293/45c2d92d-de6a-4862-9185-d22f201ef94b" width="500" height="300"/>
  <img alt="Tela inicial card-back do Prototipo de Alta Fidelidade" src="https://github.com/AdrianaKatarina/Data-Lovers/assets/122534293/c8b3225b-8cc3-4e43-be31-ef4c8ebe9974" width="500" height="300"/>

  <h3>Protótipo mobile</h3>
  <img alt="Tela Home Mobile do Prototipo de Alta Fidelidade" src="https://github.com/AdrianaKatarina/Data-Lovers/assets/122534293/67c70edd-49fb-41f2-9312-3260e390d95c" width="200" height="400"/>
  <img alt="Tela inicial card-front Mobile do Prototipo de Alta Fidelidade" src="https://github.com/AdrianaKatarina/Data-Lovers/assets/122534293/bc8fbfb9-a763-4654-b977-011d710fa910" width="200" height="400"/>
  <img alt="Tela inicial card-back Mobile do Prototipo de Alta Fidelidade" src="https://github.com/AdrianaKatarina/Data-Lovers/assets/122534293/3f9cee15-c73f-49e7-945e-1de4ef07b433" width="200" height="400"/>
</div>



## 5. Testes de usabilidade

Fizemos testes de usabilidades e constatamos que:

1º - A barra de pesquisa deveria aceitar somente letras e corrigimos esta questão na estrutura do HTML do projeto;

2º - Ao analisar todos os cards dos pokémons, haviam 2 cards (Golbat e Chansey) não continham os dados de candy-cost, pesquisamos e adicionamos as informações no arquivo de dados;

3º - Em telas de 1366 x 768, os cards ficavam com a altura cortando as informações, fizemos os ajustes necessários;

4º - Na utilização do filtro de tipos, o usuário ao selecionar a opção "todos os tipos" o campo aparecia vazio, sem nenhuma informação, colocamos uma condicional no código para quando o usuário escolher um tipo específico;

5º - Em alguns cards como, Eevee e Tyrogue, foi observado constarem algumas vírgulas(",,,") embaixo da tabela de evolução, corrigimos no código colocando o método join("") depois da tabela.

6º - Nos cards, o tamanho da letra do nome do pokémon estava pouco destacado. Resolvemos aumentar o tamanho da fonte.

7º - O nosso usuário sentiu falta de alguma descrição do que pode ser encontrado no site. Resolvemos isso colocando um alert assim que o usuário acessa a página dos cards.


## 6. Testes unitários

Durante o projeto escrevemos nossos testes unitários para as funções encarregadas de processar, filtrar e ordenar os dados, assim como calcular estatísticas.

Nossos testes unitários tiveram uma cobertura mínima de 100% de statements (sentenças), 100% de functions (funções), 100% de lines (linhas), e 91.66% de branches (ramos) do arquivo src/data.js

Ao rodar os testes, observamos que apesar da cobertura de 100% das linhas, uma em específico não foi coberta pelos testes. Tivemos a orientação que isso não iria impactar no resultado final do projeto, uma das possibilidades seria algum bug no Jest.


## 7. Checklist

* [✓] Usar VanillaJS.
* [✓] Passar pelo linter (`npm run pretest`)
* [✓] Passar pelos testes (`npm test`)
* [✓] Testes unitários cobrem um mínimo de 70% de statements, functions, lines e
  branches.
* [✓] Inclui uma _definição de produto_ clara e informativa no `README.md`.
* [✓] Inclui histórias de usuário no `README.md`.
* [✓] Inclui rascunho da solução (protótipo de baixa fidelidade) no `README.md`.
* [✓] Inclui uma lista de problemas detectados nos testes de usabilidade no
  `README.md`.
* [✓] UI: Mostra lista/tabela/etc com dados e/ou indicadores.
* [✓] UI: Permite ordenar dados por um ou mais campos (asc e desc).
* [✓] UI: Permite filtrar dados com base em uma condição.
* [✓] UI: É _responsivo_.

## 8. Ferramentas utilizadas

* Git
* GitHub
* HTML
* CSS
* JavaScript
* Node.js
* Jest
* Figma
* Trello

## 9. Desenvolvedoras

[![Github Badge](https://img.shields.io/badge/-AdrianaOliveira-000?style=flat-square&logo=Github&logoColor=white&link=https://github.com/AdrianaKatarina)](https://github.com/AdrianaKatarina)
[![Linkedin Badge](https://img.shields.io/badge/-Adriana-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/adroliveira/)](https://www.linkedin.com/in/adroliveira/)
[![Gmail Badge](https://img.shields.io/badge/-Email-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:dricakatarina@gmail.com)](mailto:dricakatarina@gmail.com)


[![Github Badge](https://img.shields.io/badge/-KeilaOliveira-000?style=flat-square&logo=Github&logoColor=white&link=https://github.com/Keilaoliveira0112)](https://github.com/Keilaoliveira0112)
[![Linkedin Badge](https://img.shields.io/badge/-Keila-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/keilaoliveiracopy/)](https://www.linkedin.com/in/keilaoliveiracopy/)
[![Gmail Badge](https://img.shields.io/badge/-Email-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:keilaoliveira.copy@gmail.com)](mailto:keilaoliveira.copy@gmail.com)