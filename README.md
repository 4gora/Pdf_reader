# Leitor de PDF Minimalista

Um leitor de PDF minimalista, moderno e de alta performance para desktop (Windows e Linux), construído com tecnologias web e Rust.

## Visão Geral

Este projeto tem como objetivo criar uma experiência de leitura de PDFs que seja rápida, leve e com uma interface de usuário limpa, utilizando o poder do Rust para o processamento de arquivos e a flexibilidade das tecnologias web para a interface.

## Tecnologias Utilizadas

A stack principal do projeto é composta por:

* **Framework Core:** [**Tauri**](https://tauri.app/)
    * *Papel:* É a base que nos permite criar uma aplicação desktop nativa usando um frontend web. Ele gerencia a janela, a comunicação entre o frontend e o backend, e empacota tudo em um executável pequeno.

* **Linguagem do Backend:** [**Rust**](https://www.rust-lang.org/)
    * *Papel:* Responsável por toda a lógica pesada e de performance. Ele cuida de abrir, ler e processar os arquivos PDF, garantindo segurança e velocidade.

* **Framework Frontend:** [**Svelte**](https://svelte.dev/)
    * *Papel:* Utilizado para construir a interface de usuário que o usuário vê e interage. Foi escolhido por ser um compilador que gera código JavaScript otimizado, resultando em uma interface extremamente rápida e leve.

* **Linguagem do Frontend:** [**TypeScript**](https://www.typescriptlang.org/)
    * *Papel:* Adiciona um sistema de tipos ao JavaScript, o que torna o código do frontend mais robusto, mais fácil de manter e com menos bugs.

* **Renderização de PDF (Crate Rust):** [**`pdfium-render`**](https://crates.io/crates/pdfium-render)
    * *Papel:* Esta é a biblioteca Rust específica que usaremos no backend para "desenhar" as páginas de um arquivo PDF. Ela utiliza o motor de PDF do Google Chrome (PDFium), que é muito poderoso e confiável.