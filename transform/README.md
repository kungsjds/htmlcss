<strong>

<h1>Como utilizar o incrível Transform</h1>

<h2>Exemplo 1</h2>

div {
    background-color: #FF0000;
    width: 200px;
    height: 200px;
    margin: auto;

    transform: scale(2,0.5);
<h3>Irá aumentar a div o dobro do width e o height irá diminuir pela metade. Valor 1 irá ficar inalterado.</h3>
<h3>O scale() aceita 2 valores, sendo o primeiro=width e o segundo=height. Podendo ser apenas um valor, ficando width e height, ele irá alterar ambos com o mesmo valor.</h3>

    transform: scaleX(5);
<h3>scaleX() é referente apenas ao width, e irá aumentar ele com base no valor informado.</h3>

    transform: scaleY(5);
<h3>scaleY() é referente apenas ao height, e irá aumentar ele com base no valor informado.</h3>
}

<h2>Exemplo 2</h2>

.div {
    background-color: #0000FF;
    width: 200px;
    height: 200px;
    margin: auto;
    
    transform: rotate(-50deg);
<h3>O rotate, rotaciona o elemento, inforando o valor com "deg", o valor negativo, exemplo -50deg, irá girar no sentido contrário.</h3>

    transform: rotateX(30deg);
<h3>O rotateX, rotaciona o elemento na horizontal.</h3>

    transform: rotateY(-20deg);
<h3>O rotateY, rotaciona o elemento na vertical.</h3>


    
    transform: skew(20deg, 50deg);
<h3>O skew distorce o elemento, o primeiro valor na horizontal e o segundo valor na vertical</h3>

    transform: skewX(50deg);
<h3>O skewX distorce o elemento horizontalmente</h3>

    transform: skewY(50deg);
<h3>O skewY distorce o elemento verticalmente</h3>
}

</strong>