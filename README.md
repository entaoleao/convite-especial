# convite-especial[Uploading jantacomapitica.htm<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Convite para um Jantar Especial</title>

    <style>
        body{
            background-image: url('https://img.freepik.com/vetores-premium/padrao-sem-emenda-de-mao-desenhada-sushi_70536-111.jpg?size=626&ext=jpg');
            background-size: cover;
            background-repeat: no-repeat;
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .container{
            background-color: rgba(255, 255, 255, 0.8); /* Fundo branco com transparência */
            border-radius: 20px;
            padding: 30px;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        h1{
            color: #ff1493; /* Rosa brilhante */
        }

        img{
            width: 200px;
            border-radius: 50%;
            margin-top: 20px;
        }

        p{
            margin-top: 20px;
            line-height: 1.5;
        }

        button{
            background-color: #ff1493; /* Rosa brilhante */
            border: none;
            color: white;
            padding: 20px 40px; /* Aumentando o tamanho do botão */
            font-size: 16px;
            border-radius: 10px; /* Aumentando o raio da borda */
            cursor: pointer;
            margin-top: 20px;
            transition: background-color 0.3s;
        }

        button:hover{
            background-color: #d111a1; /* Rosa mais escuro */
        }

        #nao{
            position: relative;
        }

        @keyframes correr {
            0% { left: 0; top: 0; }
            25% { left: 0; top: 20px; }
            50% { left: 20px; top: 20px; }
            75% { left: 20px; top: 0; }
            100% { left: 0; top: 0; }
        }

    </style>

</head>
<body>

    <div class="container">
        <h1>Convite para um Jantar Especial</h1>

        <img src="https://i.pinimg.com/736x/e9/8e/19/e98e194cacd32c677caa46a1a0b5e1a5.jpg" alt="Macaquinho fofo">
        
        <p>Olá minha pitica,</p>
        <p>Gostaria de te convidar para um jantar especial no restaurante Yurai Sushi Prime nesta sexta-feira, dia 26, às 20:00.</p>
        <p>O que acha?</p>

        <a href="https://www.youtube.com/watch?v=wji_5z7Aw-o"><button id="sim">Sim, vamos lá!</button></a>
        <button id="nao" onmouseover="correr()">Não, prefiro ver mais opções...</button>
    </div>

    <script>
        function correr() {
            var botaoNao = document.getElementById("nao");
            var larguraJanela = window.innerWidth;
            var alturaJanela = window.innerHeight;
            var maxX = larguraJanela - botaoNao.offsetWidth - 200; // Aumentando a margem de espaço
            var maxY = alturaJanela - botaoNao.offsetHeight - 200; // Aumentando a margem de espaço
            var aleatorioX = Math.floor(Math.random() * maxX);
            var aleatorioY = Math.floor(Math.random() * maxY);
            botaoNao.style.left = aleatorioX + "px";
            botaoNao.style.top = aleatorioY + "px";
            botaoNao.addEventListener("mouseenter", function() {
                aleatorioX = Math.floor(Math.random() * maxX);
                aleatorioY = Math.floor(Math.random() * maxY);
                botaoNao.style.left = aleatorioX + "px";
                botaoNao.style.top = aleatorioY + "px";
            });
        }
    </script>

</body>
</html>
l…]()
