# 💡 Minha Primeira Página no Ar

<p align="center">
  Uma página simples e interativa feita para praticar HTML, CSS e JavaScript.
</p>

<p align="center">

![HTML5](https://img.shields.io/badge/HTML5-Estrutura-orange?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-Estilo-blue?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Interação-yellow?style=for-the-badge&logo=javascript&logoColor=black)

</p>

---

## ✨ Sobre o projeto

Este projeto apresenta uma lâmpada virtual controlada por um botão. Ao clicar em **Ligar**, o estado da página muda: a lâmpada é acesa, o fundo fica claro e o botão passa a oferecer a opção **Desligar**.

O objetivo é demonstrar, de forma simples e didática, a interação entre elementos da página e eventos do JavaScript.

## 🎯 Funcionalidades

- ✅ Alternar entre lâmpada ligada e desligada
- ✅ Alterar o emoji exibido na página
- ✅ Mostrar mensagens diferentes para cada estado
- ✅ Trocar o texto do botão
- ✅ Aplicar uma classe visual ao fundo da página
- ✅ Fazer a transição do fundo de forma suave

## 🖼️ Estados da lâmpada

| Estado | Ícone | Fundo | Texto do botão |
|---|---|---|---|
| Apagada | 🌑 | Cinza escuro | Ligar |
| Acesa | 💡 | Amarelo claro | Desligar |

## 📁 Estrutura dos arquivos

```text
professora/
├── index.html  # Estrutura da página
├── style.css   # Aparência visual da página
├── script.js   # Comportamento e interação
└── README.md   # Documentação do projeto
```

## 🧩 Explicação dos códigos

### `index.html`

O arquivo HTML define a estrutura principal da página:

- `<h1>` apresenta o título principal
- `<p>` exibe a tecnologia utilizada
- `<p id="lampada">` mostra a lâmpada usando um emoji
- `<button id="interruptor">` funciona como interruptor
- `<p id="aviso">` mostra o estado atual da luz
- `<script src="script.js">` conecta o JavaScript à página

### `style.css`

O CSS define a aparência do projeto:

- Centraliza o conteúdo com `margin: 24px auto`
- Define largura máxima e espaçamento lateral
- Usa uma fonte simples do sistema
- Coloca o conteúdo no centro da página
- Define o fundo escuro e o texto claro inicialmente
- Muda as cores quando o corpo recebe a classe `acesa`
- Personaliza o tamanho da lâmpada e o botão
- Cria uma transição suave no fundo com `transition`

### `script.js`

O JavaScript guarda o estado da lâmpada em uma variável:

```javascript
let ligada = false;
```

O valor `false` significa que a lâmpada começa apagada.

Depois, o código encontra os elementos importantes:

```javascript
const botao = document.querySelector("#interruptor");
const lampada = document.querySelector("#lampada");
const aviso = document.querySelector("#aviso");
```

Quando o botão recebe um clique:

1. `ligada = !ligada` troca o estado atual.
2. Se estiver ligada, o emoji muda para 💡.
3. A mensagem e o texto do botão são atualizados.
4. A classe `acesa` é adicionada ao elemento `<body>`.
5. Se estiver apagada, a classe `acesa` é removida.

O evento é registrado assim:

```javascript
botao.addEventListener("click", function () {
    // Código executado ao clicar
});
```

## 🔄 Como funciona a alternância

```text
Estado inicial
     ↓
ligada = false
     ↓
Clique no botão
     ↓
ligada = !ligada  → true
     ↓
Lâmpada acesa
     ↓
Novo clique
     ↓
ligada = !ligada  → false
     ↓
Lâmpada apagada
```

## 🚀 Como executar

1. Abra a pasta `professora`.
2. Abra o arquivo `index.html` no navegador.
3. Clique em **Ligar** para acender a lâmpada.
4. Clique em **Desligar** para retornar ao estado inicial.

Também é possível utilizar a extensão **Live Server** no Visual Studio Code.

## ⚠️ Observação sobre os estilos

O HTML atual referencia `estilo.css`, mas o arquivo existente está nomeado como `style.css`.

Para aplicar o CSS corretamente, há duas opções:

- Renomear `style.css` para `estilo.css`, ou
- Alterar a referência do HTML para:

```html
<link rel="stylesheet" href="style.css">
```

## 🛠️ Tecnologias utilizadas

- **HTML5** — estrutura da página
- **CSS3** — estilos e animações
- **JavaScript** — interação e mudança de estado

## 👨‍💻 Autor

### Murilo Santos

Projeto desenvolvido para aprendizado e prática de desenvolvimento web.

---

<p align="center">
  <strong>Minha primeira página no ar — feita com HTML, CSS e JavaScript 💛</strong>
</p>
