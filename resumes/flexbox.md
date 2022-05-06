# Posicionamento de elementos com Flexbox em CSS

## Introdução ao flexbox

### Para que serve flexbox?

Ele foi projetado como um modelo de layout unidimensional e como um método ofecere distribuição de espaço entre itens e recursos de alinhamento.

### O que é uma tag flex container e uma tag flex item?

É uma tag que envolve itens (elementos filhos) que serão transformados em "flex itens". Vale ressaltar que um flex item pode envolver outros itens, e assim ser simultaneamente um flex container. É na tag flex container que aplicamos a propriedade "display: flex".

### Propriedades relacionadas ao flex container

- display
- flex-derection
- flex-wrap
- flex-flow
- justify-content
- align-items
- align-content

### Propriedades relacionadas ao flex item

- flex-grow
- flex-basis
- flex-shrink
- flex
- order
- align-self

## Flex Container

### display

Ao definirmos atribuímos "display:flex" à um dado elemento, tornamos todos os seus elementos filhos em flex itens, portanto é assim que criamos um flex container

### flex-derection

É propriedade que estabelece o eixo principal do container, definindo a direção que os flex itens são colocados dentro do flex container. Seus valores podem ser:

- row (padrão): alinha os itens na horizontal da esquerda para a direita
- row-reverse: alinha os itens na horizontal da direita para a esquerda
- column: alinha os itens na vertical de cima para baixo
- column-reverse: alinha os itens na vertical de baixa para cima

### flex-wrap

É propriedade que define se os itens devem ou não quebrar a linha. Por padrão não quebram a linha, fazendo com que os flex itens sejam compactados além do limite do conteúdo. Seus valores podem ser:

- nowrap (padrão): não permite a quebra da linha
- wrap: permite a quebra de linha assim que um dos flex itens não puder ser mais compactado
- wrap-reverse: semelhante ao wrap, porém o item que não puder ser mais compactado é "jogado" na direção contrária, isto é, para cima

### flex-flow

É uma atalho para as propriedades flex-derection e flex-wrap, portanto em termos de resultados de exibição, não há diferença entre usa o flex-flow somente ou usar o flew-wrap combinado ao flex-derection.

### justify-content

Propriedade que se encarrega de alinhar os itens dentro do container de acordo com a direção pretendida e trata da distribuição de espaçamento entre eles, todavia essa propriedade não se aplica caso o elemento ocupa 100% do container

### align-itens

Trata do alinhamento dos flex itens de acordo com o eixo do container, funcionando de modo diferente quando os itens estão em linhas ou em colunas.
