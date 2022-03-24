<strong>

<h1>Como aplicar um CSS aos elementos, menos para os elementos informados</h1>

<p>--HTML--</P>

<!-- <div>Div</div> -->

<!-- <p>Parágrafo</p> -->

<!-- <a href="">Link</a> -->


<p>--CSS--</P>

<p>Obs. colocar body antes, caso vá aplicar em tudo, pois o body também é um elemento e irá ser aplicado nele </p>

<p>Aplica o css para todos, menos os que forem informados no () do :not </p>

body :not(p) {
    background-color: red;
}

<p>Irá aplicar um background vermelho para a div e o link, menos para o parágrafo.</p>

</strong>