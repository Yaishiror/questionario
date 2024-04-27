<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Questionário</title>
    <style>
        body {
            display: flex;
            justify-content: center; 
            align-items: center;
            height: 100vh;
            margin: 0;
            font-family: Arial, sans-serif;
        }
        .question {
            text-align: center;
            margin-bottom: 20px;
            font-size: 20px;
        }
        .options {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }
        .option {
            margin: 10px;
            padding: 10px 20px;
            font-size: 16px;
            border: 1px solid #ccc;
            background-color: #f9f9f9;
            cursor: pointer;
        }
        .option:hover {
            background-color: #e9e9e9;
        }
    </style>
</head>
<body>

<div class="question">
    <b>
    <h2>pergunta?</h2>
    </b>
</div>

<div class="options">
    <button class="option" onclick="redirecionar()">Sim</button>
    <button class="option" onclick="moverNao()">Não</button>
</div>

<script>
    function redirecionar() {
        // Redirecionar para o vídeo no YouTube
        window.location.href = "https://www.youtube.com/watch?v=iRWSjN--LHY";
    }

    function moverNao() {
        // Mover o botão "Não" para uma nova posição na tela
        var naoButton = document.querySelector('.option:last-child');
        var optionsDiv = document.querySelector('.options');
        optionsDiv.insertBefore(naoButton, optionsDiv.firstChild);
    }
</script>

</body>
</html>
