# Graphic Tracker

![License](https://img.shields.io/badge/license-MIT-blue.svg) ![Python Version](https://img.shields.io/badge/python-3.9%2B-blue) ![Node.js Version](https://img.shields.io/badge/node-18%2B-green)

Um aplicativo de desktop para gerenciar sua coleção pessoal de HQs, com sincronização na nuvem e um monitor de preços para sua lista de desejos.


## Sobre o Projeto

Este é um projeto pessoal para criar uma solução para gestão de quadrinhos. O objetivo é ter um local centralizado para catalogar todas as HQs adquiridas, acompanhar o status de leitura, avaliações e, principalmente, ajudar a economizar na hora de comprar novos itens através de um sistema de monitoramento de preços na lista de desejos.

A aplicação é construída com uma arquitetura local-first, onde todos os dados pertencem ao usuário e são salvos localmente, com a conveniência da sincronização entre dispositivos via Google Drive.


## Funcionalidades
  - **Gerenciamento da Coleção:** Adicione, edite e remova HQs da sua coleção.
  - **Controle Detalhado:** Salve informações como editora, preço pago, preço de capa, data da compra e uma imagem da capa.
  - **Status de Leitura:** Marque suas HQs como "Lido", "Lendo" ou "Não Lido".
  - **Avaliações:** Dê uma nota de 1 a 5 para as HQs que você já leu.
  - **Lista de Desejos (Wishlist):** Mantenha uma lista das HQs que você deseja comprar.
  - **Monitor de Preços:** Automatize a busca por preços dos itens da sua wishlist nos principais e-commerces do Brasil, como:
    - Amazon
    - Panini
    - Mundos Infinitos
    - Mercado Livre
    - Magazine Luiza
    - Comix
  - **Sincronização Segura:** Sincronize seu banco de dados entre diferentes computadores usando sua própria conta do Google Drive.
  - **Relatórios e Dashboard:** Visualize estatísticas sobre sua coleção, como total gasto, HQs lidas no ano, etc.


🛠️ **Tecnologias Utilizadas**

Este projeto combina o poder do Python para lógica de backend com tecnologias web modernas para uma interface de usuário rápida e agradável.

| Categoria | Tecnologia |
| --- | --- |
| **Estrutura** | ![Electron](https://img.shields.io/badge/Electron-47848F?style=for-the-badge&logo=electron&logoColor=white) |
| **Interface (Frontend)** | ![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB) ![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white) ![Vite](https://img.shields.io/badge/Vite-B73BFE?style=for-the-badge&logo=vite&logoColor=FFD62E) |
| **Lógica (Backend)** | ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) |
| **Banco de Dados** | ![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white) |
| **Web Scraping** | Playwright & Beautiful Soup |
| **APIs** | Google Drive API |
        
## 🚀 Rodando o Projeto Localmente

Para clonar e rodar esta aplicação no seu ambiente de desenvolvimento, siga os passos abaixo.

#### Pré-requisitos

  - **Node.js** (v18+)
  - **Python** (v3.9+)
  - Acesso a um terminal (bash, zsh, PowerShell)

#### Guia de Instalação

1.  **Clone o repositório:**

    ```bash
    git clone https://github.com/[seu-usuario]/[seu-repositorio].git
    cd [seu-repositorio]
    ```

2.  **Configure o Backend (Python):**
    *É altamente recomendado usar um ambiente virtual.*

    ```bash
    cd backend
    python -m venv venv
    source venv/bin/activate  # No Windows: venv\Scripts\activate
    pip install -r requirements.txt
    cd ..
    ```

3.  **Configure o Frontend (Electron):**

    ```bash
    npm install
    ```

4.  **Configure as Chaves de API:**

      - Para a sincronização, siga o guia do Google para obter seu arquivo `credentials.json` e coloque-o na pasta `backend`.

5.  **Execute a Aplicação:**

    ```bash
    npm start
    ```

    Isso iniciará a aplicação em modo de desenvolvimento com hot-reload.

## 📄 Licença

Este projeto é distribuído sob a Licença MIT. Veja o arquivo `LICENSE` para mais detalhes.
