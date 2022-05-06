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

É propriedade que estabelece o eixo principal do container, definindo a direção que os flex itens são colocados dentro do flex container.

### flex-wrap

É propriedade que define se os itens devem ou não quebrar a linha. Por padrão não quebram a linha, fazendo com que os flex itens sejam compactados além do limite do conteúdo.

### flex-flow

É uma atalho para as propriedades flex-derection e flex-wrap, portanto em termos de resultados de exibição, não há diferença entre usa o flex-flow somente ou usar o flew-wrap combinado ao flex-derection.

### justify-content

Propriedade que se encarrega de alinhar os itens dentro do container de acordo com a direção pretendida e trata da distribuição de espaçamento entre eles, todavia essa propriedade não se aplica caso o elemento ocupa 100% do container

### align-itens

Trata do alinhamento dos flex itens de acordo com o eixo do container, funcionando de modo diferente quando os itens estão em linhas ou em colunas.

### align-content

Propriedade responsável por tratar o alinhamento das linhas do container em relação ao eixo vertical do container. Para esse propriedade seja aplicada é necessário que o container utileze quebra de linha e a altura do container deve ser maior que a soma das linhas dos itens.

## Flex item

### flex-grow

Propriedade que define a proporcionalidade de crescimento dos itens, respeitando o tamnaho de seus conteúdos internos. Caso tenhamos adicionado justify-content ao nosso flex containe, ele funcionará somente se o flex-grow for igual a zero.

### flex-basis

Propriedade que define o tamanho inicial de um flex item.

### flex-shrink

Propriedade que estabelece a capacidade de redução ou compressão do tamanho de um item

### flex

É um propriedade atalho para flex-grow, flex-shrink e flex-basis

### order

propriedade que pode ser utilizada para alterar a ordem de exibição dos itens (sem necessariamente ter que apresentar na ordem que está presente no HTML ou na ordem exatamente inversa)

### align-self

propriedade de que serve para determinar alinhamento individual de uma dado flex item
