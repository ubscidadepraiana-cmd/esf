<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Check-in Confraternização de Fim de Ano</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #1f4068, #162447);
            color: #fff;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }
        .container {
            max-width: 500px;
            width: 90%;
            background: rgba(255, 255, 255, 0.95);
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.5);
            color: #333;
            text-align: center;
        }
        h1 {
            color: #ff5722;
            margin-bottom: 5px;
            font-size: 2.2em;
        }
        h2 {
            color: #007bff;
            font-size: 1.1em;
            margin-top: 0;
            border-bottom: 2px solid #ccc;
            padding-bottom: 10px;
        }
        label {
            display: block;
            margin-top: 15px;
            font-weight: bold;
        }
        input, textarea {
            width: 100%;
            padding: 10px;
            margin-top: 5px;
            border: 1px solid #ccc;
            border-radius: 5px;
            box-sizing: border-box;
        }
        button {
            background-color: #ff5722;
            color: white;
            padding: 12px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            width: 100%;
            margin-top: 20px;
            font-size: 1.1em;
        }
        button:hover {
            background-color: #e64a19;
        }
        .note {
            margin-top: 20px;
            padding: 10px;
            background-color: #fff3e0;
            border-left: 5px solid #ff9800;
            color: #555;
            text-align: left;
        }
    </style>
</head>
<body>

<div class="container">
    <h1>🎉 Check-in da Confraternização! 🥂</h1>
    <h2>Por favor, confirme sua presença e contribuição.</h2>

    <div class="note">
        ⚠️ <b>IMPORTANTE:</b> Este formulário não coleta dinheiro. Ele apenas registra seu nome e o valor que você irá contribuir.
    </div>

    <!-- FORM SUBMIT -->
    <form action="https://formsubmit.co/ubscidadepraiana@gmail.com" method="POST">

        <!-- Remove captcha -->
        <input type="hidden" name="_captcha" value="false">

        <!-- Mensagem após enviar -->
        <input type="hidden" name="_next" value="https://google.com">

        <label>Seu Nome Completo:</label>
        <input type="text" name="Nome" required>

        <label>Valor da Contribuição (R$):</label>
        <input type="number" name="Contribuição" min="0" step="0.01" required>

        <label>Acompanhantes:</label>
        <textarea name="Acompanhantes" rows="3" placeholder="Ex: Maria, João, Criança (4 anos)"></textarea>

        <button type="submit">Confirmar Check-in e Contribuição</button>
    </form>

    <hr>
    <footer>
        <small>Aguardamos você na festa! | Desenvolvido por Lucas Marini.</small>
    </footer>
</div>

</body>
</html>
