# Calculadora ➕➖✖️➗

Este projeto apresenta uma calculadora desenvolvida em HTML5, CSS e JavaScript. É um exemplo de aplicação prática das minhas habilidades em desenvolvimento web.

## Tecnologias Usadas 🖥️

- HTML5
- CSS
- JavaScript

## Estrutura do Projeto 📘

O projeto é composto por um arquivo HTML que integra a estrutura, o estilo e a lógica da calculadora.

### Código HTML 📖

A estrutura do arquivo HTML é a seguinte:

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>calculadora</title>
    <style>
        ...
    </style>
</head>
<body>
    ...
    <script>
        ...
    </script>
</body>
</html>
```

## Estrutura do CSS 🎨

O estilo da calculadora é definido na tag <style> do cabeçalho:

```
*{
    margin: 0;
    padding: 0;
}

.fundo {
    background-image: linear-gradient(45deg, black, aquamarine);
    height: 100vh;
    color: white;
    font-family: Arial, Helvetica, sans-serif;
    text-align: center;
}

.calculator {
    position: absolute;
    background-color: rgba(0, 0, 0, 0.9);
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    border-radius: 15px;
    padding: 15px;
}

.botao {
    width: 50px;
    height: 50px;
    font-size: 25px;
    margin: 3px;
    cursor: pointer;
    background-color: rgb(31, 31, 31);
    border: none;
    color: #fff;
}

.botao:hover {
    background-color: rgb(2, 2, 2);
}

#resultado {
    width: 207px;
    height: 30px;
    margin: 5px;
    font-size: 25px;
    background-color: rgb(12, 12, 12);
    color: white;
    text-align: right;
    padding: 5px;
}
```

## Funcionalidade JavaScript ☕
A lógica da calculadora é implementada através de funções JavaScript:

```
function insert(num) {
    var numero = document.getElementById('resultado').innerHTML;
    document.getElementById('resultado').innerHTML = numero + num;
}

function clean() {
    document.getElementById('resultado').innerHTML = "";
}

function back() {
    var resultado = document.getElementById('resultado').innerHTML;
    document.getElementById('resultado').innerHTML = resultado.substring(0, resultado.length - 1);
}

function calcular() {
    var resultado = document.getElementById('resultado').innerHTML;
    if (resultado) {
        document.getElementById('resultado').innerHTML = eval(resultado);
    } else {
        document.getElementById('resultado').innerHTML = "tem nada ai o";
    }
}
```

## Como Executar❔ :
1. Clone o repositório.
2. Abra o arquivo HTML em um navegador.

## Considerações Finais 🤔
Este projeto é uma demonstração de como integrar HTML, CSS e JavaScript para criar aplicações interativas, foi um dos meus primeiros contatos com estas tecnologias.<br><br>
Estou sempre buscando aprimorar minhas habilidades e desenvolver projetos ainda mais desafiadores.
