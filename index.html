<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Acesso Restrito - Temática Escolar</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f0f8ff;
            color: #333;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
            position: relative;
        }
        .container {
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            padding: 20px;
            width: 90%;
            max-width: 400px;
            text-align: center;
            position: relative;
        }
        h1 {
            color: #2c3e50;
            margin-bottom: 20px;
        }
        p {
            color: #555;
            margin-bottom: 20px;
        }
        .error-message {
            color: #c0392b;
            font-weight: bold;
            margin-top: 20px;
        }
        .success-message {
            color: #27ae60; /* Verde */
            font-weight: bold;
            margin-top: 20px;
        }
        select {
            width: 100%;
            padding: 10px;
            margin-bottom: 20px;
            font-size: 16px;
            border: 2px solid #2c3e50;
            border-radius: 5px;
            background-color: #eaf2f8;
            color: #333;
        }
        button {
            background-color: #2c3e50;
            color: #fff;
            padding: 10px 15px;
            border: none;
            border-radius: 5px;
            font-size: 16px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        button:hover {
            background-color: #34495e;
        }
        .logo {
            width: 80px;
            position: absolute;
            bottom: 10px;
            right: 10px;
        }
        #quick-access-icon {
            width: 30px;
            height: 30px;
            background-color: red;
            position: fixed;
            top: 10px;
            right: 10px;
            border-radius: 50%;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        #quick-access-icon.active {
            background-color: green; /* Cor verde quando o código está correto */
        }
        #code-input-box {
            position: fixed;
            top: 50px;
            right: 10px;
            background-color: white;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Acesso Restrito</h1>
        <p id="network-status">Verificando rede...</p>

        <label for="formSelector">Escolha sua sala:</label>
        <select id="formSelector">
            <!-- Salas da turma 2 -->
            <option value="https://docs.google.com/forms/d/e/1FAIpQLSfsokvJ5Jl5WuFtBcBCWnoXRhsFZ60wpTZhBohbQOBU5j28AA/viewform">Sala 2A</option>
            <option value="https://forms.gle/2zRjS912gSFG5tVk9B">Sala 2B</option>
            <option value="https://forms.gle/2zRjS912gSFG5tVk9C">Sala 2C</option>
            <option value="https://forms.gle/2zRjS912gSFG5tVk9D">Sala 2D</option>
            <option value="https://forms.gle/2zRjS912gSFG5tVk9E">Sala 2E</option>
            <option value="https://forms.gle/2zRjS912gSFG5tVk9F">Sala 2F</option>
            
            <!-- Salas da turma 3 -->
            <option value="https://forms.gle/2zRjS912gSFG5tVk9G">Sala 3A</option>
            <option value="https://forms.gle/2zRjS912gSFG5tVk9H">Sala 3B</option>
            <option value="https://forms.gle/2zRjS912gSFG5tVk9I">Sala 3C</option>
            <option value="https://forms.gle/2zRjS912gSFG5tVk9J">Sala 3D</option>
            <option value="https://forms.gle/2zRjS912gSFG5tVk9K">Sala 3E</option>
            <option value="https://forms.gle/2zRjS912gSFG5tVk9L">Sala 3F</option>
        </select>
        <button id="submitBtn">Acessar Sala</button>

        <!-- Adiciona o logo na parte inferior direita -->
        <img src="https://i.postimg.cc/BbqnT0ZX/Pri-Arte-20240902-141956-0000.png" alt="Logo Escolar" class="logo">
    </div>

    <!-- Ícone de entrada rápida -->
    <div id="quick-access-icon" onclick="toggleCodeInput()"></div>
    
    <!-- Caixa de entrada de código -->
    <div id="code-input-box" style="display: none;">
        <input type="text" id="access-code" placeholder="Insira o código">
        <button onclick="validateCode()">Entrar</button>
    </div>

    <script>
        let codeValidated = false;

        async function getUserIP() {
            try {
                const response = await fetch('https://api64.ipify.org?format=json');
                if (!response.ok) {
                    throw new Error('Erro ao acessar a API');
                }
                const data = await response.json();
                return data.ip;
            } catch (error) {
                console.error('Erro ao obter o IP:', error);
                return null;
            }
        }

        function sendAccessData(ip) {
            const url = "https://script.google.com/macros/s/AKfycbwAVWsiag9nWHv1IO0M5ai6nzga5pEOeI02x3zYyOa_ltBJyOWYOApboaMbZui3VkbH/exec";

            fetch(url, {
                method: 'POST',
                mode: 'no-cors', // Modo no-cors para evitar problemas de CORS
                headers: {
                    'Content-Type': 'application/json'
                },
                body: JSON.stringify({ ip: ip })
            }).then(response => console.log('Dados enviados com sucesso'))
              .catch(error => console.error('Erro ao enviar os dados:', error));
        }

        function showErrorMessage(message) {
            const errorMessageElement = document.getElementById('network-status');
            errorMessageElement.textContent = message;
            errorMessageElement.classList.remove('success-message'); // Remove a classe de sucesso, se existir
            errorMessageElement.classList.add('error-message'); // Adiciona a classe de erro
        }

        function showSuccessMessage(message) {
            const successMessageElement = document.getElementById('network-status');
            successMessageElement.textContent = message;
            successMessageElement.classList.remove('error-message'); // Remove a classe de erro, se existir
            successMessageElement.classList.add('success-message'); // Adiciona a classe de sucesso
        }

        function toggleCodeInput() {
            const codeInputBox = document.getElementById('code-input-box');
            codeInputBox.style.display = codeInputBox.style.display === 'none' ? 'block' : 'none';
        }

        function validateCode() {
            const accessCode = document.getElementById('access-code').value;
            const validCode = 'SEUCODIGO'; // Insira o código de acesso correto aqui

            if (accessCode === validCode) {
                showSuccessMessage('Código correto! Clique em "Acessar Sala" para entrar.');
                document.getElementById('quick-access-icon').classList.add('active'); // Muda o ícone para verde
                codeValidated = true;
            } else {
                showErrorMessage('Código incorreto! Tente novamente.');
                document.getElementById('quick-access-icon').classList.remove('active'); // Mantém o ícone vermelho
                codeValidated = false;
            }
        }

        async function checkAccess() {
            const userIP = await getUserIP();
            const allowedSubnet = '138.94.66.230/2400'; // Sub-rede permitida

            const formSelector = document.getElementById('formSelector');
            const submitBtn = document.getElementById('submitBtn');
            
            submitBtn.addEventListener('click', () => {
                if (codeValidated || (userIP && isIPInSubnet(userIP, allowedSubnet))) {
                    const selectedFormURL = formSelector.value;
                    sendAccessData(userIP); // Envia os dados de acesso antes de redirecionar
                    window.location.href = selectedFormURL;
                } else {
                    showErrorMessage('Acesso negado! Você deve se conectar à rede escolar ou inserir o código correto.');
                }
            });

            if (userIP && isIPInSubnet(userIP, allowedSubnet)) {
                showSuccessMessage('Você está na rede escolar.');
                document.getElementById('quick-access-icon').classList.add('active');
            } else {
                showErrorMessage('Você não está na rede escolar. Insira o código de acesso.');
            }
        }

        function isIPInSubnet(ip, subnet) {
            // Função para verificar se o IP está na sub-rede permitida
            // Implementação simplificada para este exemplo
            return ip.startsWith(subnet.split('/')[0]);
        }

        checkAccess();
    </script>
</body>
</html>
