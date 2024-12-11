### Guia de Estudo: Fundamentos de HTML

#### **O que é HTML?**
HTML (HyperText Markup Language) é a linguagem de marcação utilizada para criar a estrutura e o conteúdo de páginas na web. Ela organiza o conteúdo em elementos que podem incluir texto, imagens, links, tabelas, vídeos e muito mais.

---

#### **Estrutura Básica de um Documento HTML**
Todo documento HTML segue uma estrutura padrão:

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Primeiro Site</title>
</head>
<body>
    <h1>Bem-vindo ao meu site!</h1>
    <p>Este é o meu primeiro parágrafo em HTML.</p>
</body>
</html>
```

##### **Descrição dos Elementos:**
- `<!DOCTYPE html>`: Declara que o documento usa HTML5.
- `<html>`: Elemento raiz que engloba todo o conteúdo.
- `<head>`: Contém informações meta sobre a página (não visíveis ao usuário).
- `<meta charset="UTF-8">`: Define a codificação de caracteres (UTF-8).
- `<title>`: Define o título da página exibido na aba do navegador.
- `<body>`: Contém todo o conteúdo visível da página.

---

#### **Principais Elementos HTML**

##### **1. Títulos**
Os títulos organizam o conteúdo em hierarquias, variando de `<h1>` (mais importante) a `<h6>` (menos importante).

```html
<h1>Meu Título Principal</h1>
<h2>Subtítulo</h2>
<h3>Seção Menor</h3>
```

##### **2. Parágrafos e Textos**
Use o elemento `<p>` para criar parágrafos e `<br>` para quebras de linha.

```html
<p>Este é um parágrafo.</p>
<p>Outro parágrafo com uma<br>quebra de linha.</p>
```

##### **3. Links**
O elemento `<a>` cria links.

```html
<a href="https://example.com" target="_blank">Visite o Example</a>
```
- `href`: URL do destino.
- `target="_blank"`: Abre o link em uma nova aba.

##### **4. Imagens**
O elemento `<img>` exibe imagens.

```html
<img src="caminho-da-imagem.jpg" alt="Descrição da imagem">
```
- `src`: Caminho da imagem.
- `alt`: Texto alternativo para acessibilidade.

##### **5. Listas**
- **Ordenadas (`<ol>`)**

```html
<ol>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ol>
```

- **Não ordenadas (`<ul>`)**

```html
<ul>
    <li>Item A</li>
    <li>Item B</li>
    <li>Item C</li>
</ul>
```

##### **6. Formulários**
Formulários capturam dados do usuário.

```html
<form action="/enviar" method="post">
    <label for="nome">Nome:</label>
    <input type="text" id="nome" name="nome">
    <button type="submit">Enviar</button>
</form>
```
- `action`: URL para onde os dados serão enviados.
- `method`: Método HTTP (ex.: `get` ou `post`).

---

#### **Boas Práticas de HTML**
1. **Use tags semânticas:** Substitua `<div>` genéricos por tags como `<header>`, `<footer>`, `<section>` e `<article>`.
2. **Adicione descrições:** Use atributos como `alt` em imagens para acessibilidade.
3. **Valide seu código:** Utilize ferramentas como o [W3C Validator](https://validator.w3.org/) para garantir que seu código está correto.
4. **Organize o código:** Indente adequadamente para facilitar a leitura.

---

#### **Exercícios Práticos**
1. **Crie um site pessoal simples:**
   - Título com `<h1>` e subtítulos com `<h2>` ou `<h3>`.
   - Parágrafos para falar sobre você.
   - Uma imagem com `<img>`.
   - Uma lista ordenada ou não ordenada.

2. **Adicione links:**
   - Um link para seu perfil no GitHub.
   - Um link para abrir uma página externa em uma nova aba.

3. **Inclua um formulário:**
   - Campos para nome, e-mail e uma mensagem.
   - Botão de envio.

---

#### **Recursos Adicionais**
- [MDN Web Docs: HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
- [HTML Tutorial - W3Schools](https://www.w3schools.com/html/)

Comece a explorar e praticar para solidificar seu conhecimento de HTML! Este guia é apenas o primeiro passo para criar páginas web incríveis.

Aprenda também sobre [HTML Semântico](https://github.com/hitalloazevedo/trilhas/blob/main/frontend/html-semantico.md)