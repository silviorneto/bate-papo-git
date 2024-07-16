# Git / Github

## O que é o GIthub

- Sistema de controle de versão distribuído.
- Criado por Linus Torvalds em 2005.
- Usado para rastrear mudanças no código-fonte durante o desenvolvimento de software.

## Qual problema ele resolve?

- Mantém o histórico de alterações.
- Facilita o trabalho colaborativo em projetos.
- Permite reverter mudanças e experimentar novas funcionalidades sem risco.

## **Configuração Inicial**

- **Instalação do Git**
    - Download e instalação (Windows, macOS, Linux).
- **Configuração Básica**

    ```bash

    git config --global user.name "Seu Nome"
    git config --global user.email "seu.email@exemplo.com"

    ```


## Conceitos Básicos e Comandos

- **Iniciando um repositório**
    - `git init`
        - Cria um novo repositório Git.
- **Clonando um repositório**
    - `git clone <url-do-repositorio>`
        - Copia um repositório existente.
- **Rastreando mudanças**
    - `git status`
        - Mostra o estado das alterações.
    - `git add <arquivo>`
        - Adiciona arquivos ao índice (staging area).
    - `git commit -m "mensagem"`
        - Grava as mudanças no repositório.
- **Visualizando histórico**
    - `git log`
        - Mostra o histórico de commits.
- **Stash (Guardar Trabalhos em Progresso)**
    - `git stash`
        - Armazena temporariamente mudanças não commitadas.
    - `git stash pop`
        - Restaura as mudanças guardadas.


## Trabalho Colaborativo

- **Branches**
    - Conceito de branch.
    - Criando uma nova branch:

        ```bash

        git checkout -b nome-da-branch

        ```

    - Mudando de branch:

        ```bash

        git checkout nome-da-branch

        ```

- **Mesclagem de branches**
    - `git merge nome-da-branch`
        - Mescla a branch especificada na branch atual.
- **Rebase**
    - `git rebase nome-da-branch`
        - Reaplica commits da branch atual sobre a base da `nome-da-branch`.
- **Resolução de conflitos**
    - Conceito de conflitos e como resolvê-los.
- **Revertendo mudanças**
    - `git revert <commit>`
        - Cria um novo commit que desfaz as mudanças de um commit específico.


## Diferença entre Merge e Rebase

- **Merge**
    - Mescla duas branches, criando um commit de merge.
    - Mantém o histórico completo, incluindo merges.
- **Rebase**
    - Reaplica commits de uma branch sobre outra.
    - Cria um histórico linear, sem commits de merge.
- **Quando usar?**
    - `merge`: Quando o histórico de merges é importante.
    - `rebase`: Para um histórico mais limpo e linear.


## GitHub

- **O que é o GitHub?**
    - Plataforma de hospedagem de código.
    - Facilita a colaboração e o gerenciamento de repositórios Git.
- **Configurando GitHub**
    - Criando uma conta no GitHub.
    - Criando um novo repositório.
    - Conectando repositório local com GitHub:

        ```bash

        git remote add origin <url-do-repositorio-github>
        git push -u origin main

        ```

- **Colaborando no GitHub**
    - Pull Requests.
    - Revisão de código.
    - Issues e gerenciamento de projetos.
