<strong>
    Como selecionar o Primeiro e Último elemento no CSS.
    
    Obs. É muito utilizado em Menus e tabelas. Para plicar uma borda somente na primeira e última div, por exemplo.

    Exemplo:

    HTML

    <div></div>
    <div></div>
    <div></div>
    <div></div>

    
    CSS
    
    Irá selecionar a primeira div e aplicar o css informado.

div:first-child {
    border-top-left-radius: 20px;
    border-top-right-radius: 20px;
}



    Irá selecionar a última div e aplicar o css informado.

div:last-child {
    border-bottom-left-radius: 20px;
    border-bottom-right-radius: 20px;
}
</strong>