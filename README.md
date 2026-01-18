# 🚀 Portfólio Pessoal - Arquitetura com LESS

![Status](https://img.shields.io/badge/Status-Finalizado-green)
![LESS](https://img.shields.io/badge/Style-LESS-1d365d?logo=less&logoColor=white)
![Grunt](https://img.shields.io/badge/Build-Grunt-fba919?logo=grunt&logoColor=white)
![HTML5](https://img.shields.io/badge/Code-HTML5-orange?logo=html5&logoColor=white)

> Uma vitrine profissional desenvolvida sob a ótica da Engenharia de Software, priorizando a organização, reutilização de código e automação de processos de build.

## 🎯 Motivação e Propósito

Um portfólio não serve apenas para mostrar projetos passados, mas para demonstrar a habilidade técnica atual. O propósito deste repositório foi construir uma aplicação web robusta, abandonando o CSS monolítico em favor de uma **Arquitetura Modular**.

Este projeto resolve o problema de manutenção de estilos em interfaces complexas. Utilizando **LESS**, o código visual é quebrado em componentes lógicos (Header, Hero, Projetos), facilitando a escala e a alteração de temas através de variáveis globais, tudo automatizado via **Grunt**.

## 🖼️ Demonstração Visual



## 🛠️ Tecnologias Utilizadas

A stack foi escolhida para demonstrar domínio sobre pré-processadores e task runners:

* **[LESS (Leaner Style Sheets)](https://lesscss.org/):** Pré-processador CSS dinâmico.
    * **Variáveis:** Controle global de cores e tipografia.
    * **Mixins:** Reutilização de blocos de estilo (ex: botões, breakpoints).
    * **Nesting:** Hierarquia visual clara no código.
* **[Grunt.js](https://gruntjs.com/):** Automatizador de tarefas.
    * `grunt-contrib-less`: Compilação de `.less` para `.css`.
    * `grunt-contrib-watch`: Monitoramento em tempo real para desenvolvimento ágil.
    * `grunt-replace` (se aplicável): Injeção de scripts/estilos no HTML.
* **[HTML5 Semântico](https://developer.mozilla.org/pt-BR/docs/Web/HTML):** Estrutura acessível e otimizada para SEO.

## ✨ Funcionalidades

O projeto conta com:

1.  **Pipeline de Build:** Transformação automática de código de desenvolvimento (`src`) para código de produção (`dev` ou `dist`).
2.  **Design Responsivo:** Layout fluido adaptável a Mobile, Tablet e Desktop.
3.  **Modularização de Estilos:** Separação física de arquivos por responsabilidade (evita arquivos CSS gigantes e ilegíveis).
4.  **Seções Interativas:** Navegação suave (Smooth Scroll) entre as seções de Sobre, Habilidades e Contato.

## 📂 Estrutura de Arquivos

A organização reflete um ambiente profissional de desenvolvimento, separando o código fonte dos artefatos compilados:

```text
_meu_portfolio_less/
├── src/                 # SOURCE: Onde o desenvolvimento acontece
│   ├── styles/          # Arquivos .less (main.less importa os demais)
│   ├── scripts/         # Scripts JavaScript originais
│   └── images/          # Ativos visuais brutos
├── dev/ (ou dist)       # BUILD: Código gerado pelo Grunt (Browser Read)
│   ├── styles/          # main.css final compilado
│   └── scripts/         # Scripts minificados
├── gruntfile.js         # Configuração das tarefas de automação
├── package.json         # Dependências do projeto
└── index.html           # Ponto de entrada
