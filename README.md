**Dragon Ball API**: Explore o universo de Dragon Ball enquanto estuda programação com a linguagem  [**Javascript**](https://thiagorossi.com.br/category/javascript) em meu site. Neste caso em especial, o código faz uma requisição AJAX e manipulação de respostas no formato json.

Escolha uma das raças através do botões e veja a mágica acontecendo.

## Dragon Ball API explicado:

O código é dividido em três partes:  **CSS**,  **HTML**  e  **JavaScript**.

**CSS**: O CSS está definindo o estilo dos elementos na página. Por exemplo,  `.tr-db-race-btn`  e  `#tr-container`  são estilizados como uma grade com três colunas e um espaço de 10px entre os itens da grade.

**HTML**: O HTML cria a estrutura da página. Há uma  `div`  com a classe  `tr-db-race-btn`  que contém vários botões. Cada botão tem um evento  `onclick`  que chama a função  `buscaPorRaca`  com um argumento de raça específico. Há também uma  `div`  com o id  `tr-container`  onde os cartões de personagens serão inseridos.

**JavaScript**: O JavaScript define duas funções,  `buscaPorRaca`  e  `limpaCard`.

-   `buscaPorRaca(raca)`: Esta função faz uma chamada à API de Dragon Ball para buscar personagens de uma raça específica. Para cada personagem retornado, cria uma  `div`  para o personagem e adiciona o nome, imagem e informações de Ki do personagem à  `div`. Em seguida, adiciona a  `div`  do personagem ao  `tr-container`.
-   `limpaCard()`: Esta função remove todos os cartões de personagens existentes. É chamada no início de  `buscaPorRaca`  para garantir que os cartões de personagens de buscas anteriores sejam removidos antes de adicionar novos cartões.
