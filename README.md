# Acesso Restrito

Este projeto inclui um código HTML que verifica o IP do usuário para restringir o acesso a um formulário. O código é útil para garantir que o formulário só possa ser acessado por usuários dentro da rede da escola.

## Código HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Acesso Restrito</title>
</head>
<body>
    <h1>Acesso Restrito</h1>
    <p>Este formulário só pode ser acessado dentro da escola.</p>
    <script>
        // Função para obter o IP do usuário via API pública
        async function getUserIP() {
            try {
                const response = await fetch('https://api64.ipify.org?format=json');
                const data = await response.json();
                return data.ip;
            } catch (error) {
                console.error('Erro ao obter o IP:', error);
                return null;
            }
        }

        // Verifica o IP do usuário
        async function checkAccess() {
            const userIP = await getUserIP();
            const allowedIP = '192.168.101.6'; // Coloque o IP ou faixa de IP permitida

            if (userIP === allowedIP) {
                window.location.href = 'https://forms.gle/2zRjS912gSFG5tVk9'; // Substitua pelo link do seu formulário
            } else {
                document.body.innerHTML += '<p>Você não está na rede da escola. O acesso ao formulário foi bloqueado.</p>';
            }
        }

        // Executa a verificação
        checkAccess();
    </script>
</body>
</html>
