# 🧾 Client CRUD API

Este projeto é uma **API RESTful de gerenciamento de clientes (CRUD)** desenvolvida com **Spring Boot** e **Java 17**.  
Foi criada para exercitar conceitos fundamentais como:
- Implementação de operações CRUD completas;
- Tratamento de exceções customizadas;
- Validação de dados com **Bean Validation**;
- Paginação e ordenação de resultados;
- Retorno de respostas HTTP adequadas (404, 422, etc.).

---

## 🧩 Funcionalidades

✅ Listagem paginada de clientes  
✅ Busca de cliente por **ID**  
✅ Inserção de novo cliente  
✅ Atualização de cliente existente  
✅ Exclusão de cliente  
✅ Tratamento completo de exceções e mensagens customizadas  

---

## ⚙️ Regras de Validação

| **name** | Não pode ser vazio: `@NotBlank(message = "O nome não pode estar vazio.")`
| **birthDate** | Não pode ser uma data futura: `@PastOrPresent(message = "A data de nascimento não pode ser futura.")` 

---

## 🚦 Respostas HTTP testadas:

| GET /clients/{id} | Sucesso | 200 | Retorna o cliente |
| GET /clients/{id} | Erro | 404 | Cliente não encontrado |
| POST /clients | Sucesso | 201 | Cliente criado com sucesso |
| POST /clients | Erro | 422 | Dados inválidos |
| PUT /clients/{id} | Sucesso | 200 | Cliente atualizado |
| PUT /clients/{id} | Erro | 404 / 422 | Cliente inexistente ou dados inválidos |
| DELETE /clients/{id} | Sucesso | 204 | Cliente excluído |
| DELETE /clients/{id} | Erro | 404 | Cliente inexistente |

---

## 🧠 Tecnologias Utilizadas

- ☕ **Java 17**  
- 🌱 **Spring Boot 3.5.7**  
- 🧩 **Spring Data JPA**  
- 🗄️ **H2 Database (em memória)**  
- 📄 **Bean Validation (Jakarta Validation)**  
- 🧱 **Maven**
- 🌙 **Insomnia**
- 🧰 **IntelliJ IDEA**

---
---

# 🧾 Client CRUD API

This project is a **RESTful Client Management API (CRUD)** developed with **Spring Boot** and **Java 17**.  
It was created to practice fundamental concepts such as:
- Implementation of complete CRUD operations;  
- Handling of custom exceptions;  
- Data validation using **Bean Validation**;  
- Pagination and sorting of results;  
- Returning proper HTTP responses (404, 422, etc.).

---

## 🧩 Features

✅ Paginated client listing  
✅ Retrieve client by **ID**  
✅ Insert a new client  
✅ Update an existing client  
✅ Delete a client  
✅ Full exception handling with custom messages  

---

## ⚙️ Validation Rules

| **Field** | **Rule** |
|------------|-----------|
| **name** | Cannot be blank: `@NotBlank(message = "Name cannot be blank.")` |
| **birthDate** | Cannot be a future date: `@PastOrPresent(message = "Birth date cannot be in the future.")` |

---

## 🚦 Tested HTTP Responses

| **Endpoint** | **Status** | **Code** | **Description** |
|---------------|------------|-----------|-----------------|
| GET /clients/{id} | ✅ Success | 200 | Returns the client |
| GET /clients/{id} | ❌ Error | 404 | Client not found |
| POST /clients | ✅ Success | 201 | Client successfully created |
| POST /clients | ❌ Error | 422 | Invalid data |
| PUT /clients/{id} | ✅ Success | 200 | Client updated |
| PUT /clients/{id} | ❌ Error | 404 / 422 | Client not found or invalid data |
| DELETE /clients/{id} | ✅ Success | 204 | Client deleted |
| DELETE /clients/{id} | ❌ Error | 404 | Client not found |

---

## 🧠 Technologies Used

- ☕ **Java 17**  
- 🌱 **Spring Boot 3.5.7**  
- 🧩 **Spring Data JPA**  
- 🗄️ **H2 Database (in-memory)**  
- 📄 **Bean Validation (Jakarta Validation)**  
- 🧱 **Maven**  
- 🌙 **[Insomnia](https://insomnia.rest)**  
- 🧰 **IntelliJ IDEA**

---
