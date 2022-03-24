<strong>

    Como aplicar um CSS aos elementos, menos para os elementos informados

    --HTML--

<div>Div</div>

<p>Parágrafo</p>

<a href="">Link</a>


    --CSS--

    Obs. colocar body antes, caso vá aplicar em tudo, pois o body também é um elemento e irá ser aplicado nele 

    Aplica o css para todos, menos os que forem informados no () do :not 

body :not(p) {
    background-color: red;
}

    Irá aplicar um background vermelho para a div e o link, menos para o parágrafo.

</strong>