<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cleon Math Bot</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        header {
            background: #35424a;
            color: #ffffff;
            padding: 10px 0;
            text-align: center;
        }

        main {
            padding: 20px;
        }

        section {
            margin: 20px 0;
        }

        footer {
            text-align: center;
            padding: 10px 0;
            background: #35424a;
            color: #ffffff;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to Cleon Math Bot!</h1>
    </header>

    <main>
        <section id="calculator">
            <h2>Ask me a math question!</h2>
            <input type="text" id="userInput" placeholder="Type your math expression here...">
            <button onclick="getAnswer()">Calculate</button>
            <p id="botResponse"></p>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Cleon Math Bot. All rights reserved.</p>
    </footer>

    <script>
        async function getAnswer() {
            const userInput = document.getElementById('userInput').value;
            const response = document.getElementById('botResponse');

            // For a static version, we can simulate a response
            try {
                // Simulate evaluation using eval (not safe for production)
                const result = eval(userInput);
                response.textContent = `Result: $
