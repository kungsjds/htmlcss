<strong>

<h1>Como aplicar um CSS aos elementos, menos para os elementos informados</h1>

<h2>Exemplo</h2>

<h3>Obs. colocar body antes, caso vá aplicar em tudo, pois o body também é um elemento e irá ser aplicado nele </h3>

<h4>Aplica o css para todos, menos os que forem informados no () do :not. No exemplo abaixo, não irá aplicar apenas para a tag "p", parágrafo </h4>

body :not(p) {
    background-color: red;
}

</strong>