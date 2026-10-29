# 🍃 Aprendendo Spring — API com Spring Security & JWT

API RESTful desenvolvida em **Java** com **Spring Boot**, focada no aprendizado de conceitos avançados como **Segurança com JWT (JSON Web Token)**, **Spring Security**, arquitetura em camadas e integração de **CI/CD via GitHub Actions**.

---

## 🚀 Funcionalidades

- **Autenticação & Segurança (JWT):**
  - Geração e validação de tokens JWT (`JwtUtil`)[cite: 8].
  - Filtro customizado de requisições (`JwtRequestFilter`)[cite: 8].
  - Configuração centralizada de segurança via Spring Security (`SecurityConfig`)[cite: 8].
- **Gestão de Usuários:** Cadastro e gerenciamento de usuários com suporte a dados de endereço e telefone[cite: 8].
- **Pipeline de CI/CD:** Integração contínua automatizada via GitHub Actions para build e testes com Maven (`.github/workflows/maven.yml`)[cite: 8].
- **Arquitetura Clean & DDD-like:** Divisão clara entre regras de negócio (`business`), pontos de entrada (`controller`) e infraestrutura (`infrastructure`)[cite: 8].

---

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** Java 17+[cite: 8]
- **Framework:** Spring Boot 3.x[cite: 8]
- **Módulos Spring:**
  - Spring Web (APIs RESTful)[cite: 8]
  - Spring Security (Autenticação e Autorização)[cite: 8]
  - Spring Data JPA (Persistência de Dados)[cite: 8]
- **Segurança:** JJWT (Java JWT) / HMAC SHA[cite: 8]
- **DevOps & CI/CD:** GitHub Actions (Workflows de Build Maven)[cite: 8]
- **Ferramentas:** Maven, IntelliJ IDEA, Git & GitHub[cite: 8]

---

## 📂 Estrutura do Projeto

```text
src/main/java/com/javanauta/aprendendospring
├── business/               # Regras de negócio da aplicação (Ex: UsuarioService)
├── controller/             # Endpoints REST e DTOs (UsuarioController, UsuarioDTO)
├── infrastructure/         
│   ├── entity/             # Entidades JPA (Usuario, Endereco, Telefone)
│   ├── exceptions/         # Tratamento de exceções customizadas
│   ├── repository/         # Interfaces Spring Data JPA
│   └── security/           # Filtros, utilitários JWT e configurações do Spring Security
└── AprendendoSpringApplication.java
