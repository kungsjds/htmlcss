<strong>
<h1>Como selecionar elementos pelos seus atributos.</h1>


<h3>Definir o atributo que irá aplicar o css pelo "[nome-atributo]"</h3>

<h3>Exemplos:</h3>

[type=text] {
    display: block;
}

input[type=password]  {
    border: 2px solid blue;
}

[href] {
    display: block;
}

[href="#teste"] {
    background-color: red;
}

<h3>Nomes de atributos criados, devem ser incluídos entre "". Como names, value, etc. Tudo que precisa definir um nome e já não é do próprio HTML.</h3>
[name="usuario"] {
    border-radius: 50%;
}

<h3>Utilizando o ^= verifica o valor informado entre "" no início do href(ou o atributo que for informado), e quem tiver irá aplicar o css.</h3>
[href^="https:"] {
    background-color: #b7b7b7;
}

<h3>Utilizando o *= verifica o valor informado entre "" em qualquer parte do href(ou o atributo que for informado), e quem tiver irá aplicar o css.</h3>
[href*="tecnologia"] {
    background-color: #171717;
}

<h3>Utilizando o $= verifica o valor informado entre "" no final do href(ou o atributo que for informado), e quem tiver irá aplicar o css.</h3>
[href$="anos/"] {
    background-color: #9c9c9c;
}

</strong>