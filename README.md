# Adivinhe-o-valor
Programa básico de números aleatórios.
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <input type="">
    <button>
        Advinhe o valor!
    </button>

    <script>
        var segredo = Math.round(Math.random() *10);
        var input = document.querySelector("input");
        input.focus();

        function verifica(){
            if(input.value == segredo){
                alert("Você ACERTOU!");
            } else{
                alert("Você ERROU!!!!");
            }
            input.value = "";
            input.focus();
        }
        var button = document.querySelector("button");
        button.onclick = verifica;
    </script>
</body>
</html>
