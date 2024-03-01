# web-front-2

index.html

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Filmes Favoritos</title>
<style>
    body {
        font-family: Arial, sans-serif;
        background-color: #f0f0f0;
    }
    .container {
        max-width: 600px;
        margin: 20px auto;
        padding: 20px;
        background-color: #fff;
        border-radius: 8px;
        box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    h1 {
        text-align: center;
    }
    input[type="text"] {
        width: calc(100% - 80px);
        padding: 10px;
        margin-right: 10px;
        border: 1px solid #ccc;
        border-radius: 4px;
        outline: none;
    }
    button {
        padding: 10px 20px;
        background-color: #007bff;
        color: #fff;
        border: none;
        border-radius: 4px;
        cursor: pointer;
    }
    button:hover {
        background-color: #0056b3;
    }
    ul {
        list-style-type: none;
        padding: 0;
    }
    li {
        background-color: #007bff;
        color: #fff;
        padding: 10px;
        margin-top: 5px;
        border-radius: 4px;
    }
</style>
</head>
<body>
<div class="container">
    <h1>Filmes Favoritos</h1>
    <div>
        <input type="text" id="filmeInput" placeholder="Digite o nome do filme">
        <button>Adicionar</button>
    </div>
    <ul id="listaFilmes">
        
    </ul>
    <script src="app.js"></script>
</div>


testes.js 

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Filmes Favoritos</title>
<style>
    body {
        font-family: Arial, sans-serif;
        background-color: #f0f0f0;
    }
    .container {
        max-width: 600px;
        margin: 20px auto;
        padding: 20px;
        background-color: #fff;
        border-radius: 8px;
        box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    h1 {
        text-align: center;
    }
    input[type="text"] {
        width: calc(100% - 80px);
        padding: 10px;
        margin-right: 10px;
        border: 1px solid #ccc;
        border-radius: 4px;
        outline: none;
    }
    button {
        padding: 10px 20px;
        background-color: #007bff;
        color: #fff;
        border: none;
        border-radius: 4px;
        cursor: pointer;
    }
    button:hover {
        background-color: #0056b3;
    }
    ul {
        list-style-type: none;
        padding: 0;
    }
    li {
        background-color: #007bff;
        color: #fff;
        padding: 10px;
        margin-top: 5px;
        border-radius: 4px;
    }
</style>
</head>
<body>
<div class="container">
    <h1>Filmes Favoritos</h1>
    <div>
        <input type="text" id="filmeInput" placeholder="Digite o nome do filme">
        <button>Adicionar</button>
    </div>
    <ul id="listaFilmes">
        
    </ul>
    <script src="app.js"></script>
</div>


app.js

const listaFilmes = document.querySelector("#listaFilmes")
let filmes = [{
    nome: 'Harry Potter',
    lancamento: 2001,
    rating: 10,


}]

    


window.onload = () =>{
    for(let i=0; i < filmes.length;i++){
        let listaItem = document.createElement('li')
        listaFilmes.append(listaItem)
        listaItem.innerHTML = filmes[i].nome

        let ratingItem = document.createElement('li')
        listaFilmes.append(ratingItem)
        ratingItem.innerHTML - filmes[i].rating
    }
}
