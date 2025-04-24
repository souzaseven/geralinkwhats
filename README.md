# 📱 Gerador de Link para WhatsApp

Uma ferramenta web para criar links diretos de conversa no WhatsApp com números de telefone e mensagens pré-definidas, incluindo geração de QR Code e personalização de temas.
<!--
![Pré-visualização](https://github.com/souzaseven/horatrabalhada/blob/Desafios/Hora%20trabalhada/horatrabalhada.png?raw=true)
-->
## ✨ Funcionalidades

- **Links Diretos de Conversa**
  - Gera links para WhatsApp e WhatsApp Web
  - Pré-prepara mensagens automaticamente
  - Inclui automaticamente código do Brasil (+55)

- **Geração de QR Code**
  - Cria QR Codes escaneáveis para compartilhamento fácil
  - Utiliza a biblioteca QRCode.js

- **Experiência do Usuário**
  - Alternância entre temas claro/escuro
  - Validação de entrada
  - Sistema de feedback visual
  - Design responsivo

- **Funções Úteis**
  - Copiar link para área de transferência
  - Iniciar conversa diretamente
  - Opção para WhatsApp Web

## 🛠️ Tecnologias Utilizadas

- **Frontend**
  - HTML5 semântico
  - CSS3 com variáveis
  - JavaScript puro (ES6+)

- **Bibliotecas**
  - Font Awesome (ícones)
  - QRCode.js (geração de QR Codes)
  - Google Analytics (métricas)

- **Recursos do Navegador**
  - localStorage (preferências de tema)
  - Clipboard API (cópia de links)

## 📂 Estrutura de Arquivos
whatsapp-link-generator/ <br>
├── link-whatsapp.html # Estrutura principal <br>
├── style.css # Estilos e temas <br>
└── script.js # Lógica da aplicação <br>



## 🎨 Personalização

- **Temas Disponíveis:**
  - 🌞 Tema Claro (padrão)
  - 🌚 Tema Escuro

- **Estilos:**
  - Cores semânticas
  - Efeitos de hover
  - Sombras e bordas arredondadas
  - Layout responsivo

## ⚙️ Como Usar

1. Insira o número de telefone (sem espaços ou caracteres especiais)
2. Digite sua mensagem (opcional)
3. Escolha uma ação:
   - `Gerar`: Cria os links
   - `Iniciar`: Abre a conversa diretamente
   - `Copiar`: Copia o link
   - `QR Code`: Gera um código escaneável

```javascript
// Exemplo de geração de link
function criarLink(numero, mensagem) {
    const mensagemFormatada = encodeURIComponent(mensagem);
    const numeroFormatado = numero.replace(/\D/g, '');
    return `https://wa.me/${codigoPais}${numeroFormatado}?text=${mensagemFormatada}`;
}
```

📱 Responsividade
O design se adapta a:

Desktop
Tablets
Smartphones

``` CSS
/* Exemplo de media query */
@media (max-width: 600px) {
    .btn-container {
        flex-direction: column;
    }
    .btn {
        margin-bottom: 10px;
        width: 100%;
    }
}
```

📌 Dicas <br>
Para números internacionais, remova o +55 do código <br>
Mensagens longas são automaticamente codificadas <br>
O QR Code pode ser salvo como imagem (clique com o botão direito)
