# Acesso Restrito - Temática Escolar

## Descrição

Este projeto consiste em uma página de acesso restrito para uma plataforma escolar. O objetivo é permitir que usuários acessem formulários específicos com base em sua rede IP ou através de um código de acesso. O acesso é controlado por uma verificação de rede e um código de acesso. Além disso, o número de acessos diários é registrado em uma planilha do Google Sheets.

## Funcionalidades

- **Verificação de Rede**: Verifica se o usuário está conectado à rede escolar permitida.
- **Código de Acesso**: Permite o uso de um código para desbloquear o acesso caso o usuário não esteja na rede permitida.
- **Redirecionamento**: Redireciona o usuário para o formulário selecionado.
- **Registro de Acesso**: Envia o IP do usuário e o número de acessos diários para uma planilha do Google Sheets.

## Instruções de Uso

1. **Configuração do Código**:
    - Substitua `'SEUCODIGO'` pelo código de acesso correto no arquivo `index.html`.

2. **Configuração do Web App**:
    - Atualize a URL do Web App no arquivo `index.html` para `https://script.google.com/macros/s/AKfycbwAVWsiag9nWHv1IO0M5ai6nzga5pEOeI02x3zYyOa_ltBJyOWYOApboaMbZui3VkbH/exec` se necessário.

3. **Configuração da Sub-rede**:
    - Ajuste o IP e a sub-rede permitida no arquivo `index.html` conforme necessário.

4. **Implementação**:
    - Faça o upload do arquivo `index.html` para seu servidor web ou ambiente de hospedagem.

## Estrutura do Projeto

- `index.html`: Arquivo HTML principal contendo a lógica para verificação de rede, código de acesso e redirecionamento.
- **Web App**: URL para o script do Google Apps que registra o número de acessos diários na planilha.

## Dependências

- **Google Apps Script**: Utilizado para registrar o número de acessos diários.
- **Fetch API**: Usada para obter o IP do usuário e enviar dados para o Web App.

## Licença

Este projeto está licenciado sob a [Licença MIT](https://opensource.org/licenses/MIT).

