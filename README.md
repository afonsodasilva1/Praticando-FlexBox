# Praticando-FlexBox
 Praticando o meu CSS3 com o FlexBox

Minhas anotações sobre o FlexBox:

Para utilizar o flexbox é importante entender o conceito de pai e filho. Sempre que precisarmos 
de alinha um elemento devemos aplicar a propriedade "Display: flex", no container pai para que
os containers filhos se adaptem. Devemos também colocar a direcção do alinhamento ou seja o
flex-direction, que poder receber valores como: row, column, row-reverse, column-reverse... tal
como mostra o exemplo a seguir:

html, body, #app{
    height: 100%;
    margin: 0;
}
#app{ => Container pai
    display: flex;
    flex-direction: row;
}
.box{ => Container filho
    width: 60px;
    height: 60px;
    background: #f00;
    margin: 5px;
}

propriedades align-itens e justify-content

ambas são utilzadas para alinhar elementos. align alinha os elementos no eixo contrário definido no flex-direction, já o justify-content alinha os elementos no  mesmo eixo definido pelo flex-direction

Ex.:
#app{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
}

Flex-grow E Flex-shrink

Ambas são utilizadas para o reajuste dos elementos e são usadas no container filho, básicamente podemos chamar de comportamento.

Flex-grow é usada para indicar que o elemento pode crescer de acordo com o tamnho da tela, já o flex-shrink é o oposto, não cresce encolhe de acordo a tela.