### Guia de CSS: Estilizando suas Páginas Web

#### **O que é CSS?**
CSS (Cascading Style Sheets) é uma linguagem de estilo utilizada para descrever a apresentação de um documento HTML. Com CSS, é possível controlar cores, fontes, espaçamento, layouts e muito mais, tornando as páginas web visualmente atrativas e organizadas.

#### **Como o CSS funciona?**
CSS funciona aplicando estilos a elementos HTML. Ele pode ser adicionado de três maneiras principais:

1. **Inline:** Estilos diretamente no elemento HTML.
   ```html
   <p style="color: blue; font-size: 16px;">Texto estilizado</p>
   ```

2. **Interno:** Dentro de uma tag `<style>` no cabeçalho do documento.
   ```html
   <style>
       p {
           color: blue;
           font-size: 16px;
       }
   </style>
   ```

3. **Externo:** Em um arquivo separado com extensão `.css`.
   ```html
   <link rel="stylesheet" href="estilos.css">
   ```
   ```css
   p {
       color: blue;
       font-size: 16px;
   }
   ```

---

#### **Seletores CSS**
Seletores são usados para identificar quais elementos serão estilizados. Aqui estão alguns dos mais comuns:

- **Seletor de Elemento:**
  Aplica estilos a todas as ocorrências de um elemento.
  ```css
  p {
      color: green;
  }
  ```

- **Seletor de Classe:**
  Aplica estilos a elementos com uma classe específica. Classes são precedidas por um ponto (`.`).
  ```html
  <p class="destaque">Texto em destaque</p>
  ```
  ```css
  .destaque {
      font-weight: bold;
  }
  ```

- **Seletor de ID:**
  Aplica estilos a um elemento com um ID específico. IDs são precedidos por uma cerquilha (`#`).
  ```html
  <p id="importante">Texto importante</p>
  ```
  ```css
  #importante {
      color: red;
  }
  ```

- **Seletor Universal:**
  Aplica estilos a todos os elementos.
  ```css
  * {
      margin: 0;
      padding: 0;
  }
  ```

- **Seletores Combinados:**
  - **Descendente:** Estiliza elementos dentro de outro elemento.
    ```css
    div p {
        color: blue;
    }
    ```

  - **Grupo:** Aplica o mesmo estilo a diferentes seletores.
    ```css
    h1, h2, h3 {
        font-family: Arial, sans-serif;
    }
    ```

---

#### **Propriedades e Valores Comuns**

1. **Texto:**
   - `color`: Define a cor do texto.
   - `font-size`: Define o tamanho da fonte.
   - `text-align`: Alinha o texto (`left`, `center`, `right`).
   - `font-family`: Define a família da fonte.
   ```css
   p {
       color: #333;
       font-size: 18px;
       text-align: justify;
       font-family: 'Arial', sans-serif;
   }
   ```

2. **Caixas e Layout:**
   - `margin`: Espaço externo ao redor de um elemento.
   - `padding`: Espaço interno dentro de um elemento.
   - `border`: Define uma borda ao redor do elemento.
   - `width` e `height`: Define a largura e altura do elemento.
   ```css
   div {
       margin: 10px;
       padding: 15px;
       border: 1px solid #000;
       width: 200px;
       height: 100px;
   }
   ```

3. **Cores e Fundo:**
   - `background-color`: Cor de fundo do elemento.
   - `background-image`: Adiciona uma imagem de fundo.
   ```css
   body {
       background-color: #f4f4f4;
       background-image: url('imagem.jpg');
       background-size: cover;
   }
   ```

4. **Display e Posicionamento:**
   - `display`: Controla como o elemento é exibido (`block`, `inline`, `flex`, etc.).
   - `position`: Define o posicionamento (`static`, `relative`, `absolute`, `fixed`).
   - `z-index`: Controla a ordem de sobreposição de elementos.
   ```css
   .container {
       display: flex;
       justify-content: center;
       align-items: center;
   }
   ```

---

#### **Boas Práticas no Uso de CSS**
1. **Organização do Código:** Utilize indentção e comentação para tornar o código legível.
   ```css
   /* Estilos para o cabeçalho */
   header {
       background-color: #333;
       color: #fff;
       padding: 20px;
   }
   ```

2. **Evite Estilos Inline:** Prefira estilos em arquivos externos para facilitar a manutenção.

3. **Nomes Significativos:** Use nomes de classes e IDs descritivos.
   ```css
   .botao-primario {
       background-color: blue;
       color: white;
   }
   ```

4. **Mobile First:** Planeje o design para dispositivos móveis antes de adaptá-lo para telas maiores.
   ```css
   @media (max-width: 768px) {
       body {
           font-size: 14px;
       }
   }
   ```

---

#### **Exemplo de CSS em uma Página Completa**
```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exemplo de CSS</title>
    <link rel="stylesheet" href="estilos.css">
</head>
<body>
    <header>
        <h1>Bem-vindo ao Meu Site</h1>
    </header>
    <main>
        <section>
            <h2>Sobre Nós</h2>
            <p>Conteúdo da seção.</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2025 Meu Site</p>
    </footer>
</body>
</html>
```
```css
/* estilos.css */
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
}

header {
    background: #333;
    color: #fff;
    padding: 20px;
    text-align: center;
}

main {
    padding: 20px;
}

footer {
    background: #111;
    color: #fff;
    text-align: center;
    padding: 10px;
}
```

---

CSS é uma ferramenta poderosa para transformar simples estruturas HTML em experiências visuais cativantes. Com prática e aprendizado contínuo, é possível dominar conceitos fundamentais e avançados para criar interfaces modernas e responsivas.

