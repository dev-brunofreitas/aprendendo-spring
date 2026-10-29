# 🍃 Aprendendo Spring — API com Spring Security & JWT

API RESTful desenvolvida em **Java** com **Spring Boot**, focada no aprendizado de conceitos avançados como **Segurança com JWT (JSON Web Token)**, **Spring Security**, arquitetura em camadas e integração de **CI/CD via GitHub Actions**.

---

## 🚀 Funcionalidades

- **Autenticação & Segurança (JWT):**
  - Geração e validação de tokens JWT (`JwtUtil`).
  - Filtro customizado de requisições (`JwtRequestFilter`).
  - Configuração centralizada de segurança via Spring Security (`SecurityConfig`).
- **Gestão de Usuários:** Cadastro e gerenciamento de usuários com suporte a dados de endereço e telefone.
- **Pipeline de CI/CD:** Integração contínua automatizada via GitHub Actions para build e testes com Maven (`.github/workflows/maven.yml`).
- **Arquitetura Clean & DDD-like:** Divisão clara entre regras de negócio (`business`), pontos de entrada (`controller`) e infraestrutura (`infrastructure`).

---

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** Java 17+
- **Framework:** Spring Boot 3.x
- **Módulos Spring:**
  - Spring Web (APIs RESTful)
  - Spring Security (Autenticação e Autorização)
  - Spring Data JPA (Persistência de Dados)
- **Segurança:** JJWT (Java JWT) / HMAC SHA
- **DevOps & CI/CD:** GitHub Actions (Workflows de Build Maven)
- **Ferramentas:** Maven, IntelliJ IDEA, Git & GitHub

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
```
⚙️ Como Executar Localmente

1. Clona o repositório:
git clone [https://github.com/dev-brunofreitas/aprendendo-spring.git](https://github.com/dev-brunofreitas/aprendendo-spring.git)

2. Acesse à pasta do projeto:
cd aprendendo-spring

3. Executa a aplicação via Maven:
 mvn spring-boot:run

   📌 Projeto desenvolvido por Bruno de Freitas durante os estudos de Java e Spring Boot.

