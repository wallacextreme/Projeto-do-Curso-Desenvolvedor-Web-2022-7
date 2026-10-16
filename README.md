# App Orçamento Pessoal — Modelagem em JavaScript ES6+ & LocalStorage

[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+_Classes-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)
[![HTML5](https://img.shields.io/badge/HTML5-Semântico-E34F26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-4.0.0-7952B3?style=flat-square&logo=bootstrap&logoColor=white)](https://getbootstrap.com/)
[![LocalStorage](https://img.shields.io/badge/Storage-Web_Storage_API-005C84?style=flat-square)](https://developer.mozilla.org/pt-BR/docs/Web/API/Window/localStorage)
[![Status](https://img.shields.io/badge/Status-Study_Project-blue?style=flat-square)](#)

Aplicação web desenvolvida para prática de **JavaScript Orientado a Objetos (ES6+)**, estruturando a modelagem de entidades financeiras, rotinas de validação de formulários, controle de armazenamento local com a **Web Storage API (`localStorage`)** e interface com **Bootstrap 4**.

---

## 🎯 Objetivo

Exercitar a transição de scripts procedurais para a programação orientada a objetos no JavaScript moderno, demonstrando a criação de classes para representação de dados (`Despesa`) e abstração da camada de persistência (`Bd`), além de manipulação dinâmica de modais para feedback visual.

---

## ✨ Estrutura & Funcionalidades

- **Modelagem de Entidade (`Classe Despesa`)**: Construtor com propriedades (ano, mês, dia, tipo, descrição, valor) e método `validarDados()` para checagem de preenchimento obrigatório.
- **Camada de Armazenamento Local (`Classe Bd`)**: Métodos `getProximoId()`, `gravar()` e `recuperarTodosRegistros()` com serialização JSON e manipulação de chaves no `localStorage`.
- **Feedback Visual com Modais Bootstrap**: Diálogos modais (`#modalRegistraDespesa`) manipulados dinamicamente via DOM para alertar sobre sucesso no preenchimento ou necessidade de correção.
- **Interface de Consulta Preparada (`consulta.html`)**: Tela com filtros por período e categoria, estruturada para listagem tabular.

---

## 🧰 Stack Tecnológica

- **JavaScript Moderno (ES6+)**: Classes com `class`, `constructor`, instanciação com `new`, iteração de propriedades e serialização JSON.
- **HTML5**: Estrutura dos formulários de lançamento e telas de consulta.
- **Bootstrap 4.0, jQuery & Popper.js**: Componentes de modais, inputs e barra de navegação.
- **Font Awesome 5**: Ícones de suporte visual.

---

## 📁 Estrutura de Arquivos

```text
Projeto-do-Curso-Desenvolvedor-Web-2022-7/
├── index.html        # Tela de inclusão e cadastro de despesas
├── consulta.html     # Tela de consulta com filtros
├── app.js            # Classes Despesa e Bd, funções de captura e modais
├── logo.png          # Logotipo da aplicação
└── README.md         # Documentação técnica
```

---

## 🚀 Como Visualizar

1. Clone o repositório:
   ```bash
   git clone https://github.com/wallacextreme/Projeto-do-Curso-Desenvolvedor-Web-2022-7.git
   ```
2. Abra `index.html` em qualquer navegador web moderno.

---

## 📌 Status

- **Maturidade**: Projeto de Estudo de JavaScript OOP.
- **Competências em evidência**: Classes em JavaScript ES6+, métodos de validação, manipulação do `localStorage` e integração com componentes modais Bootstrap.

---

## 👨‍💻 Autor

Desenvolvido por **[Wallace Soares](https://github.com/wallacextreme)**.

---
## ☕ Apoie este Projeto

Se este projeto ou código foi útil para você, considere apoiar o meu trabalho com uma doação espontânea de qualquer valor. Sua contribuição ajuda a manter o desenvolvimento de novas ferramentas e soluções open-source!

<details>
<summary><strong>💠 Clique aqui para exibir os dados do PIX (Doação Voluntária)</strong></summary>

<br>

- **Chave PIX (ALEATORIA):** `91afe4f0-a466-4423-9d9c-d6a0ffea9b3e`
- **Banco:** C6 Bank
- **Titular:** Wallace de Paulo Soares

> *Nota Legal: Contribuição 100% voluntária e espontânea de apoio ao desenvolvedor (Art. 538 do Código Civil).*
</details>
