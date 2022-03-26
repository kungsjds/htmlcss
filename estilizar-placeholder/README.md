<strong>

<h1>Como estilizar o placholder do input. E suas versões.</h1>

<h2>Exemplos:</h2>


<h3>Placeholder para todos os navegadores modernos</h3>
.estilo::placeholder {
    color: #FF0000;
}

<h3>Placeholder para: Webkit, Blink, Edge</h3>
.estilo::-webkit-input-placeholder {
    color: #FF0000;
}

<h3>Firefox 4 ao 18</h3>
.estilo:-moz-placeholder {
    color: #FF0000;
}

<h3>Firefox 19+</h3>
.estilo::-moz-placeholder {
    color: #FF0000;
}

<h3>IE 10 e 11</h3>
.estilo:-ms-input-placeholder {
    color: #FF0000;
}

<h3>Microsoft Edge</h3>
.estilo::-ms-input-placeholder {
    color: #FF0000;
}

</strong>