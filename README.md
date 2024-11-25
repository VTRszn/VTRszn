<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pedido de Namoro</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 100px;
        }

        h1 {
            color: #333;
        }

        #buttons {
            position: relative;
            margin-top: 50px;
        }

        .btn {
            font-size: 18px;
            padding: 10px 20px;
            margin: 5px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
        }

        #btnSim {
            background-color: #4CAF50;
            color: white;
        }

        #btnNao {
            background-color: #f44336;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>
    <h1>Hj tem cuzin?</h1>
    <div id="buttons">
        <button id="btnSim" class="btn">Sim</button>
        <button id="btnNao" class="btn">Não</button>
    </div>

    <script>
        const btnNao = document.getElementById('btnNao');

        btnNao.addEventListener('mouseover', () => {
            const maxWidth = window.innerWidth - btnNao.offsetWidth;
            const maxHeight = window.innerHeight - btnNao.offsetHeight;

            const randomX = Math.floor(Math.random() * maxWidth);
            const randomY = Math.floor(Math.random() * maxHeight);

            btnNao.style.left = randomX + 'px';
            btnNao.style.top = randomY + 'px';
        });

        document.getElementById('btnSim').addEventListener('click', () => {
            alert('Eu sabia que você diria sim! ❤️');
        });
    </script>
</body>
</html>
