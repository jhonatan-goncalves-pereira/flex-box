# flex-box
Flexbox é uma tecnologia do CSS que permite criar layouts flexíveis e responsivos de maneira eficiente. Ela funciona através de um sistema de containers e itens, que podem ser organizados de diversas maneiras na página.

## container
Um container Flexbox é um elemento que possui a propriedade display com o valor flex ou inline-flex. Ao aplicar essa propriedade a um elemento, ele se torna um container flexível, que pode conter um ou mais itens flexíveis em seu interior.

## itens
Os itens flexíveis, por sua vez, são os elementos contidos dentro de um container Flexbox. Eles são organizados dentro do container através das propriedades de alinhamento e espaçamento do Flexbox.


### propriedaedes CSS
Algumas das propriedades mais comuns do Flexbox incluem:
- justify-content: permite alinhar os itens horizontalmente dentro do container, distribuindo o espaço sobressalente entre eles ou os espaçando igualmente.
- align-items: permite alinhar os itens verticalmente dentro do container, posicionando-os no topo, no centro ou na base do container.
- align-self: permite alinhar um item individualmente em relação aos demais itens do container.
- flex-wrap: permite que os itens sejam organizados em uma ou múltiplas linhas, dependendo do espaço disponível.
flex-direction: permite definir a direção em que os itens serão organizados dentro do container, podendo ser em linha única, coluna única, linha reversa ou coluna reversa.

Além dessas propriedades, o Flexbox também oferece uma série de valores, que podem ser aplicados às propriedades para personalizar ainda mais o layout. Alguns dos valores mais comuns incluem:

- flex: define a proporção do item em relação aos demais itens do container.
auto: permite que o tamanho do item seja definido automaticamente, baseado no seu conteúdo.
- none: remove as propriedades de flexibilidade do item.
- space-between: distribui o espaço sobressalente entre os itens, deixando espaços iguais entre eles.
- space-around: distribui o espaço sobressalente entre os itens, deixando espaços iguais ao redor deles.

### exemplo de uso
partindo de uma págin a HTML 5 que possua uma div com a classe container:
```
<div class="container">
    <div class="item">
.......elementos/conteúdo
    </div>
</div>
```

 Criando um container Flexbox
Para criar um container Flexbox, basta adicionar a propriedade display com o valor flex ou inline-flex ao elemento que deseja transformar em container. Veja o exemplo:
```
.container {
  display: flex;
}

```

2 - Definindo a direção dos itens
Você pode definir a direção em que os itens serão organizados dentro do container utilizando a propriedade flex-direction. Por padrão, os itens são organizados em linha única. Veja o exemplo:
```
.container {
  display: flex;
  flex-direction: row-reverse;
}

```

3 - Alinhando os itens horizontalmente
Para alinhar os itens horizontalmente dentro do container, utilize a propriedade justify-content. Você pode escolher entre diversos valores, como center, flex-start e flex-end. Veja o exemplo:

```
.container {
  display: flex;
  justify-content: space-between;
}
```

4 - Alinhando os itens verticalmente
Para alinhar os itens verticalmente dentro do container, utilize a propriedade align-items. Assim como na propriedade justify-content, você pode escolher entre diversos valores, como center, flex-start e flex-end. Veja o exemplo:
```
.container {
  display: flex;
  align-items: center;
}

```

5 - Distribuindo o espaço entre os itens
Você pode distribuir o espaço sobressalente entre os itens utilizando a propriedade flex-grow. Ao aplicar um valor maior a um item, ele irá ocupar mais espaço do que os demais. Veja o exemplo:
```
.item {
  flex-grow: 1;
}

```

6 - Colocando espaços entre os itens
Para colocar espaços entre os itens dentro do container, utilize a propriedade margin. É importante lembrar que, ao utilizar a propriedade margin, o espaço será adicionado tanto entre os itens quanto nas bordas externas do container. Veja o exemplo:
```
.container {
  display: flex;
}

.item {
  margin-right: 10px;
}

```

Esses são apenas alguns exemplos de como utilizar o Flexbox no CSS. É possível combinar essas propriedades e valores de diversas maneiras para criar layouts flexíveis e responsivos de acordo com as necessidades do projeto. Faça o clone dos códigos na pasta src e veja melhor como funciona o flexbox na prática.