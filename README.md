# App Orçamento Pessoal — Controle Financeiro com JavaScript ES6+ & LocalStorage

[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)
[![HTML5](https://img.shields.io/badge/HTML5-Semântico-E34F26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-4.0.0-7952B3?style=flat-square&logo=bootstrap&logoColor=white)](https://getbootstrap.com/)
[![LocalStorage](https://img.shields.io/badge/Storage-Web_Storage_API-005C84?style=flat-square)](https://developer.mozilla.org/pt-BR/docs/Web/API/Window/localStorage)
[![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)](LICENSE)

Aplicação web interativa para gestão e controle de despesas financeiras cotidianas, construída com **JavaScript Orientado a Objetos (ES6+)**, persistência local no navegador via **Web Storage API (`localStorage`)** e interface dinâmica com **Bootstrap 4**.

---

## 🎯 Objetivo

Oferecer uma ferramenta prática para cadastro, validação e consulta de despesas domésticas ou pessoais sem necessidade de infraestrutura de servidor, demonstrando conceitos fundamentais de modelagem orientada a objetos, manipulação do DOM e persistência no client-side.

---

## ✨ Principais Funcionalidades

- **Cadastro de Despesas**: Formulário completo com categorização por data (ano, mês, dia), tipo (alimentação, educação, lazer, saúde, transporte), descrição e valor monetário.
- **Validação de Dados**: Verificação prévia de campos obrigatórios via método da classe `Despesa`, impedindo o registro de valores nulos ou vazios.
- **Feedback Visual com Modais**: Diálogos modais do Bootstrap dinamicamente customizados para notificar o usuário em caso de sucesso ou erro no preenchimento.
- **Persistência Local (Offline)**: Classe `Bd` dedicada que gerencia IDs sequenciais e armazena registros serializados em formato JSON no `localStorage`.
- **Consulta e Listagem**: Tela dedicada (`consulta.html`) preparada para exibição tabular dos dados gravados.

---

## 🧰 Stack Tecnológica

- **JavaScript Moderno (ES6+)**:
  - Programação Orientada a Objetos com `class`, `constructor` e métodos de instância.
  - Serialização e desserialização com `JSON.stringify` e `JSON.parse`.
  - Manipulação de coleções (`Array`, iteração, filtros).
  - Manipulação da API DOM (`document.getElementById`, manipulação de classes CSS).
- **HTML5**: Estrutura semântica dos formulários e tabelas.
- **Bootstrap 4.0 & jQuery/Popper**: Grid responsivo, tipografia e componentes de modais.
- **Font Awesome 5**: Ícones para botões e sinalizações visuais.

---

## 🏗️ Arquitetura

O projeto adota uma separação simples e elegante entre o modelo de domínio e o armazenamento:

```text
[ Interface do Usuário (HTML + Bootstrap) ]
                     │
          [ Evento: cadastrarDespesa() ]
                     │
                     ▼
          ┌─────────────────────┐
          │   Classe Despesa    │  <-- Representa a entidade financeira
          │  .validarDados()    │      e suas regras de integridade
          └──────────┬──────────┘
                     │ (Se válido)
                     ▼
          ┌─────────────────────┐
          │      Classe Bd      │  <-- Camada de acesso a dados (DAO/Repository)
          │  .gravar()          │      Gerencia chaves, IDs e serialização
          │  .recuperarTodos()  │
          └──────────┬──────────┘
                     │
                     ▼
             [ localStorage ]
```

---

## 📁 Estrutura de Arquivos

```text
Projeto-do-Curso-Desenvolvedor-Web-2022-7/
├── index.html        # Página de inclusão e cadastro de novas despesas
├── consulta.html     # Página de consulta e filtragem das despesas salvas
├── app.js            # Regras de negócio, classes Despesa e Bd, manipulação DOM
├── logo.png          # Logotipo da aplicação
└── README.md         # Documentação técnica do projeto
```

---

## 🚀 Como Executar

Por ser uma aplicação 100% estática client-side, não há necessidade de compiladores ou servidores de back-end:

1. Clone o repositório ou faça o download dos arquivos:
   ```bash
   git clone https://github.com/wallacextreme/Projeto-do-Curso-Desenvolvedor-Web-2022-7.git
   ```
2. Abra o arquivo `index.html` diretamente em qualquer navegador moderno (Chrome, Edge, Firefox, Safari) ou utilize uma extensão como o *Live Server* do VS Code.

---

## 📌 Status

- **Status**: Concluído / Projeto de Consolidação de JavaScript OOP.
- **Competências demonstradas**: JavaScript ES6+, Web Storage API, manipulação de eventos e DOM, componentização de modais com Bootstrap.

---

## 👨‍💻 Autor

Desenvolvido por **[Wallace Soares](https://github.com/wallacextreme)**.