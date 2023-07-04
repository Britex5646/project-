<html lang="PT-BR"
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        a {
            text-decoration: none;
        }

        .box {
            font-size: 20px;
            color: white;
            height: 250px;
            width: 350px;
            border-radius: 10px;
            background: #333232;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }

        .buttons-container {
            display: flex;
            justify-content: space-around;
            align-items: center;
            height: 50px;
            width: 150px;
        }

        button {
            height: 30px;
            width: 50px;
            background: white;
            color: black;
            font-weight: 600;
            border-radius: 5px;
            border: 2px solid black;
        }
    </style>
    <title>Pedido Irrecusavel</title>
</head>
<body>
    <div class="box">
        <p>BEIJINHO HOJE?</p>
        <div class="buttons-container">
            <button><a href="https://www.youtube.com/watch?v=lg5WKsVnEA4">Sim</a></button>
            <button id="no">Nao</button>
        </div>
    </div>
</body>
<script>
    let button = document.getElementById('no');
    let height = window.innerHeight - 50;
    let width = window.innerWidth - 50;

    button.addEventListener('mouseover', function () {
        button.style.position = "absolute"
        button.style.top = Math.random() * height + "px";
        button.style.left = Math.random() * width + "px";
    })
</script>
</html>
