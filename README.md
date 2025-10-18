# 💘 Backend - Rede Social para Encontros

## 🧩 Contexto do Projeto
Este projeto tem como objetivo desenvolver o **backend de uma rede social para encontros**, inspirada em plataformas como **Tinder** e **Happn**, mas abrangentes a outros grupos e tipos de encontros.  
A priori o sistema permitirá o **cadastro de usuários**, **criação de perfis**, **sistema de matches**, **troca de mensagens** e outras funcionalidades.

---

## ⚙️ Decisões Arquiteturais

### 🖥️ Renderização: **CSR (Client-Side Rendering)**
A aplicação utilizará **Client-Side Rendering**, pois o foco está na **interatividade** e na **atualização dinâmica dos dados**.  
O backend será responsável apenas por fornecer **APIs RESTful** que serão consumidas pelo frontend (SPA ou aplicativo mobile).

**Justificativa:**
- Melhor experiência do usuário em aplicações dinâmicas;
- Maior compatibilidade com apps mobile e web;
- Backend desacoplado, atuando como provedor de dados.

---

### 🧠 Paradigma de Programação: **Orientado a Objetos (OO)**
A aplicação segue o paradigma **Orientado a Objetos**, já que o domínio possui **entidades bem definidas** como:
- `Usuário`
- `Perfil`
- `Match`
- `Mensagem`
- `Notificação`

**Benefícios:**
- Modelagem mais próxima da regra de negócio;
- Facilita manutenção e testes;
- Organização clara em camadas e classes reutilizáveis.

---

### 🧱 Arquitetura: **Monolítica Modular**
O backend será inicialmente desenvolvido de forma **monolítica**.  

**Motivação:**
- Simplicidade e rapidez no desenvolvimento inicial;

---

### ☕ Linguagem e Framework: **Java com Spring Boot**
O backend será implementado em **Java**, utilizando o framework **Spring Boot**, que oferece uma base sólida e produtiva para aplicações web modernas.

**Motivos da escolha:**
- Ecossistema maduro e consolidado;
- Excelente suporte a APIs REST, autenticação (Spring Security) e persistência (Spring Data JPA);
- Alta escalabilidade e fácil manutenção;
- Alinhamento com boas práticas de arquitetura, SOLID e Clean Code.

---

## 🚀 Resumo das Decisões

| Tema | Escolha | Justificativa |
|------|----------|---------------|
| **Renderização** | **CSR (Client-Side Rendering)** | Foco em interatividade e integração com apps web/mobile |
| **Paradigma** | **Orientado a Objetos (OO)** | Entidades e regras de negócio bem definidas |
| **Arquitetura** | **Monolítica Modular** | Simples, organizada e escalável para o futuro |
| **Linguagem/Framework** | **Java (Spring Boot)** | Robustez, maturidade e padrão de mercado para backends |

---

## 🧰 Tecnologias Principais

- **Java 21+**
- **Spring Boot 3+**
- **Spring Web / Spring Data JPA / Spring Security**
- **PostgreSQL**
- **Docker**
- **Maven**
- **Swagger**
- **Angular ?**

---

## 🗺️ Estrutura Inicial do Projeto

```text
src/
├── main/
│ ├── java/com/br/social-network/
│ │ ├── controller/
│ │ ├── service/
│ │ ├── model/
│ │ ├── repository/
│ │ └── config/
│ └── resources/
│ ├── application.properties
│ └── static/
└── test/
