# To-Do List API com Spring Boot

Este projeto é uma aplicação **To-Do List** desenvolvida com **Spring Boot**, que fornece uma API RESTful para gerenciar tarefas.
O objetivo é permitir a criação, consulta, atualização e remoção de tarefas através de endpoints HTTP. A aplicação é ideal para quem está iniciando com o desenvolvimento de APIs utilizando o ecossistema Spring.

## 📋 Conhecendo o Projeto

A **To-Do List API** é uma aplicação backend que permite gerenciar tarefas, oferecendo funcionalidades como:
- **Listar tarefas**: Obter uma lista de todas as tarefas cadastradas.
- **Adicionar tarefas**: Inserir novas tarefas na lista.
- **Atualizar tarefas**: Modificar detalhes de tarefas existentes.
- **Remover tarefas**: Excluir tarefas da lista.
- **Limpar a lista**: Excluir todas as tarefas cadastradas de uma só vez.


## 🚀 Tecnologias Utilizadas

- **Java 17**
- **Spring Boot**
- **HTTP Client Bruno** (alternativas: [Insomnia](https://insomnia.rest/download) ou [Postman](https://www.postman.com/downloads/))

<div style="border: 2px solid #C2C2C2; padding: 10px; border-radius: 5px; padding: 20px;">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" height="40" alt="java logo"  />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/spring/spring-original.svg" height="40" alt="spring logo"  />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/apache/apache-original.svg" height="40" alt="apache logo"  />
</div>

## 🛠️ Pré-requisitos

Certifique-se de ter o **Java** (JDK) instalado em sua máquina.

## 🧰 Instalação e Configuração

### 1. Iniciando o Projeto

Para criar o projeto com **Spring Boot**, utilize o [Spring Initializr](https://start.spring.io). Configure as dependências necessárias, como:
- Projeto: **Maven**
- Linguagem: **Java**
- Sprint Boot: Versão LTS (3.3.5)
- Dependências: **Spring Web**
- Packing: **Jar**
- Java: **21**

### 2. Instalando o HTTP Client Bruno

Para testar sua API, recomendamos o uso do [HTTP Client Bruno](https://www.usebruno.com/).

Para instarlar o Bruno (via npm)

``` bash

npm install -g usebruno
```

## 📦 Funcionalidades da API

### 1. Criar API de Tarefas
Utilizamos as annotations `@RestController` e `@RequestMapping` para criar uma API RESTful que gerencia tarefas.

### 2. Endpoints Disponíveis

#### a) Listar Tarefas
- **Método:** `GET/api/tasks`
- **Descrição:** Retorna uma lista de todas as tarefas.
- **Anotação:** `@GetMapping`

#### b) Criar Tarefa
- **Método:** `POST/api/tasks`
- **Descrição:** Adiciona uma nova tarefa.
- **Anotação:** `@PostMapping`
- **Corpo da Requisição (JSON):**

  ```json
  {
    "titulo": "Aprender Spring Boot",
    "descricao": "Estudar o guia oficial de Spring"
  }
  ```
  
#### c) Atualizar Tarefa
- **Método:** `PUT/api/tasks`
- **Descrição:** Atualizar uma nova tarefa.
- **Anotação:** `@PutMapping`
- **Corpo da Requisição (JSON):**

``` json
{
  "titulo": "Aprender Spring Boot",
  "descricao": "Estudar o guia oficial de Spring (atualizado)"
}
```

#### d) Remover Tarefa
- **Método:** `DELETE /api/tasks/{id}`
- **Descrição:** Remove uma tarefa específica.
- **Anotação:** `@DeleteMapping`
- **Parâmetro:** {id} - ID da tarefa a ser removida.

#### e) Limpar Lista de Tarefas
- **Método:** `DELETE /api/tasks`
- **Descrição:** Remove todas as tarefas cadastradas.


## Desenvolvedor

#### Osmar J. Facin Junior
<div>
  <a href="www.linkedin.com/in/osmarjosefacinjr" target="_blank">
    <img src="https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&label=&color=0077B5&logoColor=white&labelColor=&style=for-the-badge" height="40" alt="linkedin logo"  />
  </a>
</div>
