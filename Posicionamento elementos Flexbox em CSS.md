# ESTRUTURA BÁSICA
	É um modelo de layout unidimensional, distribui os espaco entre 
os itens e alinhamento.

## Flex Container 

-> tag que envolve os itens, nela aplica-se a propriedade display:flex
 pode ser feita em (div, span, h1, h2)

#Flex Container
Propriedades relacionadas: display(inicializador do container), flex-direction(direcionamento dos itens em linhas ou colunas), flex-wrap(quebra ou nao de linha), 
flex-flow(abreviacao do direction e wrap), justify-content (alinha os itens container), align-items(alinhamento dos eixos) , align-content (alinhamento das linhas)

#Flex Item
elementos filhos diretos do flex container (recursivo)
Propriedades relacionadas:flex-grow (fator do crescimento), flax-basis(tamanho inicial do item antes da distribuicao do espaco)
flex-shrink (capacidade de reducao), flex (abreviacao do grow, basis e shrink), order(ordem distribuicao e listagem dos itens),
 align-self(alinhamento especifico de um item do container).


#Fundamentos part1 -  flex container

###Display Flex - faz o dimensionamento para o menor possivel adequando a sua posicao de acordo 
com os seus itens.

Dicas: no VisualCode instalar as duas extensões HTML Snippets e HTML Preview
Ctrl + shift + v - abrirá a tela de visualização

Dicas comandos:
div*3  -> criará 3 div de uma só vez.

div.item*3 -> criará 3 div com o campo item.

li*5

###Flex-direction - estabelece o eixo principal do container, podendo assim definiar 
a direção dos itens colocados no flex container (linha e coluna).

####Eixos  row(padrao) 
####Eixos  row-reverse(ordenacao inversa)
####Eixos  column(padrao estilo colunas) 
####Eixos  column-reverse(ordenacao inversa)


 