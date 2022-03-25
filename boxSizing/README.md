<strong>

<h1>Como funciona o box-sizing</h1>

<h2>Exemplo</h2>

div {
    width: 200px;
    height: 200px;
    background-color: #FF0000;
    padding: 10px;
    border: 10px solid #00FF00;

<h3>No border-box, o tamanho do conteúdo irá incluir o padding e border. Ele diminui o width e o height automaticamente com base no valor do padding e border, 
    até o valor do tamanho do conteúdo ficar o tamanho definido. 
    Como nesse exemplo, ele irá diminuir 20 no width e 20 no height. Ficando 180width e 180height. Mais o padding e border o conteúdo irá somar 200 no final.</h3>
    box-sizing: border-box;

<h3>O content-box é o tamanho padrão, quando não especifica um box-sizing. Com ele definido, o tamanho que definir no elemento, será o tamanho do conteúdo
    sem incluir margin, border, padding, etc. E após incluir um padding e border, o tamanho do conteúdo irá aumentar. No exemplo, o tamanho iria ficar em 220 width e 220 height.</h3>
    box-sizing: content-box;
}
</strong>