# 🚀 CodeTutor

**CodeTutor** é uma plataforma leve de documentação interativa para tutoriais técnicos, focada em oferecer uma experiência moderna, didática e multiplataforma (Windows, Linux, etc).

O projeto utiliza uma abordagem simples e poderosa baseada em:

* Vue via CDN (sem build)
* TailwindCSS + DaisyUI
* Estrutura orientada a dados (JSON-like)

---

## 🎯 Objetivo

Facilitar o aprendizado técnico com tutoriais claros, interativos e organizados por contexto (ex: sistema operacional), seguindo padrões de documentação profissional.

---

## ✨ Funcionalidades

* 🔥 Alternância de tutoriais por sistema operacional (Tabs)
* 🧠 Detecção automática do sistema (Windows/Linux)
* 💾 Persistência de preferência do usuário (localStorage)
* 💻 Blocos de código estilo terminal (mockup)
* 📋 Botão "copiar código"
* 🎯 Separação de contexto:

  * Comando (terminal)
  * Código (editor)
  * Saída (resultado)
* ⚠️ Destaque para passos importantes (ex: configuração PATH)
* 🎬 Transições suaves (UX nível SaaS)

---

## 🧱 Estrutura do Projeto

```
/codetutor
  ├── index.html
  ├── README.md
```

> Futuro (recomendado):

```
/codetutor
  ├── index.html
  ├── /tutorials
  │     ├── cpp-windows.json
  │     ├── cpp-ubuntu.json
  ├── app.js
```

---

## 🧠 Estrutura dos Tutoriais

Os tutoriais são definidos como objetos estruturados:

```js
{
  titulo: "Hello World em C++",
  descricao: "Guia por sistema operacional",
  passos: [
    {
      titulo: "Instalar compilador",
      texto: "Descrição do passo",
      cor: "blue",
      codigo: ["comando 1", "comando 2"]
    }
  ]
}
```

---

## 🧩 Tipos de Passo

Cada passo pode conter diferentes tipos:

### 🔹 Comando (Terminal)

```js
{
  codigo: ["sudo apt install build-essential"]
}
```

### 🔹 Código (Editor)

```js
{
  tipo: "codigo",
  prefixo: "",
  codigo: [
    "#include <iostream>",
    "int main() { return 0; }"
  ]
}
```

### 🔹 Saída (Output)

```js
{
  tipo: "output",
  codigo: ["Hello, World!"]
}
```

### 🔹 Configuração

```js
{
  tipo: "configuracao",
  codigo: ["C:\\mingw64\\bin"]
}
```

---

## 🎨 Stack Tecnológica

* Vue 3 (CDN)
* TailwindCSS
* DaisyUI
* Font Awesome

---

## ⚡ Como usar

1. Clone ou baixe o projeto
2. Abra o arquivo `index.html` no navegador
3. Pronto — não precisa instalar nada 🎉

---

## 🚀 Roadmap

* 📦 Suporte a JSON externo (modo CMS)
* 🔎 Busca de tutoriais
* 🌙 Dark mode automático
* 🔗 URLs com parâmetros (`?os=linux`)
* 📚 Múltiplas categorias (Backend, DevOps, etc.)
* 🎨 Syntax Highlight (estilo VS Code)
* 🧠 Detecção inteligente de ambiente

---

## 💡 Filosofia do Projeto

CodeTutor segue os princípios:

* Simplicidade > Complexidade
* Clareza > Abstração
* Experiência do usuário > Implementação técnica

---

## 🤝 Contribuição

Sinta-se livre para:

* Sugerir melhorias
* Criar novos tutoriais
* Melhorar a UI/UX

---

## 📄 Licença

MIT License

---

## ❤️ Autor

Desenvolvido para facilitar o ensino técnico de forma moderna e acessível.
