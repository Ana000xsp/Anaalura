<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Transição de Cores</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: Arial, sans-serif;
            transition: background-color 1s;
        }
    </style>
</head>
<body>
    <h1>Clique para mudar a cor de fundo</h1>
    <script>
        const cores = ["red", "blue", "green", "yellow", "purple", "pink", "orange"];
        let indice = 0;

        document.body.addEventListener("click", () => {
            indice = (indice + 1) % cores.length;
            document.body.style.backgroundColor = cores[indice];
        });
    </script>
</body>
</html>
