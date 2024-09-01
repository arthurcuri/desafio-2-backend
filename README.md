# Desafio 2 - Backend e APIs

Este projeto é uma API REST desenvolvida em Spring Boot para interagir com o banco de dados AdventureWorks. A API fornece funcionalidades para gerenciar produtos e inclui um conjunto de testes automatizados para garantir a qualidade do código.

## Funcionalidades da API

### Tarefa 1: Funcionalidades Básicas

A API oferece as seguintes rotas para gerenciamento de produtos:

1. **Criar Produto**
   - **Método:** `POST`
   - **Rota:** `/produtos`
   - **Descrição:** Adiciona um novo produto à tabela de produtos.
   - **Corpo da Requisição:**
     ```json
     {
       "nome": "Nome do Produto",
       "numeroProduto": "Número do Produto",
       "cor": "Cor do Produto",
       "precoPadrao": 100.00,
       "precoPromo": 80.00,
       "tamanho": "Tamanho do Produto",
       "peso": 1.5
     }
     ```

2. **Listar Produtos**
   - **Método:** `GET`
   - **Rota:** `/produtos`
   - **Descrição:** Retorna uma lista de todos os produtos com paginação, filtragem e ordenação.
   - **Parâmetros de Consulta:**
     - `page` (opcional): Número da página para paginação.
     - `size` (opcional): Número de itens por página.
     - `sort` (opcional): Critério de ordenação.

3. **Obter Produto por ID**
   - **Método:** `GET`
   - **Rota:** `/produtos/{id}`
   - **Descrição:** Retorna os detalhes de um único produto baseado no ID do produto.

4. **Atualizar Produto**
   - **Método:** `PUT`
   - **Rota:** `/produtos/{id}`
   - **Descrição:** Atualiza o produto com o ID correspondente.
   - **Corpo da Requisição:**
     ```json
     {
       "nome": "Novo Nome do Produto",
       "numeroProduto": "Novo Número do Produto",
       "cor": "Nova Cor do Produto",
       "precoPadrao": 120.00,
       "precoPromo": 90.00,
       "tamanho": "Novo Tamanho do Produto",
       "peso": 1.8
     }
     ```

5. **Excluir Produto**
   - **Método:** `DELETE`
   - **Rota:** `/produtos/{id}`
   - **Descrição:** Remove o produto com o ID correspondente da tabela de produtos.

## Testes

Os testes são implementados para garantir que todas as funcionalidades da API estejam funcionando corretamente e que todos os casos de erro sejam tratados de forma adequada.

### Configuração do Ambiente de Testes

- **Banco de Dados:** Utiliza um banco de dados H2 em memória para testes isolados.
- **Framework de Testes:** JUnit 5 e Spring Boot Test.

### Testes Implementados

**Testes Unitários:**
   - Testes para cada rota da API (`POST /produtos`, `GET /produtos`, `GET /produtos/{id}`, `PUT /produtos/{id}`, `DELETE /produtos/{id}`).
   - Verificação de entradas válidas e inválidas.
   - Verificação dos erros esperados.

## Linguagem e tecnologias ultilizadas

<div>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original-wordmark.svg" alt="Java" width="120" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/spring/spring-original-wordmark.svg" alt="Spring" width="120" />
  <br>
</div>

## Contato

Arthur Curi Kramberger - [arthur1curi@gmail.com](mailto:arthur1curi@gmail.com)
