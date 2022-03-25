<strong>

<h1>Como utilizar o seletor Before e After.</h1>

<h2>OBS: Too Before e After tem que ter um (content). Para utilizar o content vazio, basta informar display: inline-block.</h2>

<h3>Exemplos:</h3>

<h3>Before, aplica um style antes do elemento informado</h3>
span::before {
    content: "";
    display: inline-block;
    background-color: #FF0000;
    width: 30px;
    height: 30px;
}

<h3>After, aplica um style depois do elemento informado</h3>
span::after {
    content: "";
    display: inline-block;
    background-color: #FF0000;
    width: 30px;
    height: 30px;
}

<h2>Exemplos práticos para balões</h2>


<h3>Aplicando o triângulo do balão ao lado da div, porém, com a ponta do triângulo apontando para baixo</h3>
.ballonOne::after {
    content: "";
    display: inline-block;    
    position: absolute;
    top: 35px;
    border: 20px solid;
    border-color: #0000FF transparent transparent transparent;

}

<h3> OBS: border-color funciona em sentido horário, sendo: cima, direita, baixo, esquerda.</h3>

<h3>Aplicando o triângulo do balão ao lado da div, com a ponta do triângulo apontando para a direita</h3>
.ballonTwo::after {
    content: "";
    display: inline-block;
    position: absolute;
    top: 35px;
    margin-left: 18px;
    border: 20px solid;
    border-color: transparent transparent transparent #0000FF;
}

<h3>Aplicando o triângulo do balão abaixo da div, com a ponta do triângulo apontando para baixo</h3>
.ballonThree::after {
    content: "";
    display: block;
    position: absolute;
    margin-top: 20px;
    border: 20px solid;
    border-color: #0000FF transparent transparent transparent;
}
</strong>