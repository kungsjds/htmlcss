<strong>
<h1>Como selecionar o Primeiro e Último elemento no CSS.</h1>
    
<p>Obs. É muito utilizado em Menus e tabelas. Para plicar uma borda somente na primeira e última div, por exemplo.</p>

<p>Exemplo:</p>

<p>HTML</p>

<!-- <div></div>
     <div></div>
     <div></div>
     <div></div> -->

    
<p>CSS</p>
    
<p>Irá selecionar a primeira div e aplicar o css informado.</p>

div:first-child {
    border-top-left-radius: 20px;
    border-top-right-radius: 20px;
}



<p>Irá selecionar a última div e aplicar o css informado.</p>

div:last-child {
    border-bottom-left-radius: 20px;
    border-bottom-right-radius: 20px;
}
</strong>