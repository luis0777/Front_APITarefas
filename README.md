# Tarefas - Sistema de Cadastro e Listagem

Este é um projeto simples para o cadastro, visualização e gerenciamento de tarefas, desenvolvido com HTML, CSS e JavaScript. O sistema permite cadastrar tarefas com nome, descrição e prioridade, e visualizá-las em uma lista filtrável.

## Funcionalidades

- **Cadastro de Tarefa**: Permite adicionar uma nova tarefa informando seu nome, descrição e prioridade (alta, média ou baixa).
- **Listagem de Tarefas**: Exibe as tarefas cadastradas em uma tabela.
- **Filtros**: Permite filtrar as tarefas por status de realização (realizado ou não realizado) ou por prioridade (alta, média, baixa).
- **Edição de Tarefa**: Permite editar uma tarefa já cadastrada.
- **Autenticação**: O sistema utiliza autenticação básica (username: admin, password: teste123).

## Estrutura do Projeto

O projeto é dividido em dois arquivos principais:

- **Cadastro de Tarefas** (`cadastro.html`): Formulário para adicionar novas tarefas.
- **Lista de Tarefas** (`listarTarefas.html`): Página que exibe as tarefas e possibilita filtrá-las.

## Tecnologias Utilizadas

- **HTML5**: Estrutura da página.
- **CSS3**: Estilos e layout da página.
- **JavaScript**: Lógica para adicionar, listar, editar e filtrar as tarefas.
- **Fetch API**: Para realizar requisições HTTP e interagir com uma API externa para manipulação das tarefas.
- **Autenticação Básica**: Para proteger o acesso à API com credenciais codificadas em base64.

## Como Usar

### 1. Cadastro de Tarefa

Para cadastrar uma nova tarefa:
- Acesse a página `cadastro.html`.
- Preencha o nome, descrição e prioridade da tarefa.
- Clique em "Adicionar" para salvar a tarefa.

### 2. Visualizar Tarefas

Para visualizar as tarefas cadastradas:
- Acesse a página `listarTarefas.html`.
- Você verá uma tabela com as tarefas cadastradas.
- Utilize os botões de filtro para visualizar tarefas realizadas, não realizadas ou por prioridade.
- Clique no botão "Ir para a Lista" para acessar a lista de tarefas a partir da página de cadastro.

### 3. Edição de Tarefa

Para editar uma tarefa:
- Clique na tarefa que deseja editar.
- O formulário de edição será exibido, permitindo que você altere o nome, descrição, prioridade e status de realização da tarefa.
- Clique em "Salvar" para aplicar as mudanças ou "Cancelar" para fechar o formulário sem salvar.

## Endpoints da API

A API utilizada para gerenciar as tarefas está disponível na URL base `http://localhost:8080/tarefas`. Ela suporta os seguintes métodos:

- **POST /tarefas**: Criação de uma nova tarefa.
- **GET /tarefas**: Listagem de todas as tarefas.
- **GET /tarefas/search/realizado**: Busca tarefas filtradas pelo status de realização.
- **GET /tarefas/search/prioridade**: Busca tarefas filtradas pela prioridade.
- **PUT /tarefas/{id}**: Edição de uma tarefa existente.
