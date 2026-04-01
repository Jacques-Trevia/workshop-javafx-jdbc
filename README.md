![Java](https://img.shields.io/badge/Java-17-blue.svg)
![JavaFX](https://img.shields.io/badge/JavaFX-17-2B4D6E.svg)
![JDBC](https://img.shields.io/badge/JDBC-Database-4479A1.svg)

# 🖥️ Workshop JavaFX + JDBC - Aplicação Desktop
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/Jacques-Trevia/workshop-javafx-jdbc/blob/main/LICENSE)

**Workshop JavaFX JDBC** é uma aplicação desktop para gerenciamento de departamentos e vendedores, desenvolvida com **JavaFX** para a interface gráfica e **JDBC** para comunicação com banco de dados relacional. O projeto demonstra na prática como construir sistemas desktop completos com arquitetura em camadas e boas práticas de desenvolvimento.

* * *

## 📋 Sobre a Aplicação

A aplicação consiste em um sistema de gerenciamento de vendas, permitindo o cadastro, edição e remoção de **departamentos** e **vendedores**. Os dados são persistidos em um banco de dados relacional (MySQL/PostgreSQL) utilizando **JDBC** para operações de CRUD.

### Principais funcionalidades

- ✅ Cadastro, listagem, atualização e remoção de departamentos
- ✅ Cadastro, listagem, atualização e remoção de vendedores
- ✅ Associação de vendedores a departamentos
- ✅ Interface gráfica moderna com JavaFX e FXML
- ✅ Tratamento de exceções e feedback visual para o usuário
- ✅ Arquitetura em camadas (UI, Service, Model, DAO)

* * *

## 🛠️ Tecnologias Utilizadas

| Categoria | Tecnologia |
|-----------|------------|
| **Linguagem** | Java 17 |
| **Interface Gráfica** | JavaFX 17, Scene Builder, FXML, CSS |
| **Banco de Dados** | MySQL / PostgreSQL |
| **Acesso a Dados** | JDBC (Java Database Connectivity) |
| **Build** | Maven / JavaFX Build Tool |
| **Design Pattern** | MVC (Model-View-Controller), DAO (Data Access Object) |

* * *

## 📂 Estrutura do Projeto

O projeto segue uma arquitetura organizada em camadas:

| Pacote | Descrição |
|--------|-----------|
| `application` | Classe principal que inicia a aplicação JavaFX |
| `gui` | Controladores (controllers) e layouts FXML |
| `model` | Entidades (Department, Seller) |
| `model.dao` | Interfaces e implementações do padrão DAO |
| `db` | Conexão com banco de dados e tratamento de exceções |
| `util` | Classes utilitárias (Alertas, mudança de telas, etc.) |

* * *

## 🚀 Como Rodar o Projeto

### 🔧 Pré-requisitos

- [JDK 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [JavaFX SDK](https://gluonhq.com/products/javafx/) (ou configurado no Maven)
- Banco de dados: [MySQL](https://www.mysql.com/downloads/) ou [PostgreSQL](https://www.postgresql.org/download/)
- IDE: Eclipse (com e(fx)clipse) ou IntelliJ

### 💾 Banco de Dados

1. Crie um banco de dados (ex: `workshop-javafx-jdbc`)
2. Execute o script SQL de criação das tabelas (disponível em `/db-script.sql`)
3. Configure o arquivo `db.properties` com suas credenciais:

```properties
db.url=jdbc:mysql://localhost:3306/workshop-javafx-jdbc
db.user=root
db.password=sua_senha
```
---

### ▶️ Executando a Aplicação
Clone o repositório:

git clone https://github.com/Jacques-Trevia/workshop-javafx-jdbc.git
Importe o projeto na sua IDE como um projeto Maven/JavaFX

Execute a classe application.Main.java

A interface gráfica será aberta com as opções de gerenciamento

---

### 📌 Funcionalidades
✅ Departamentos

Listagem completa

Cadastro de novos departamentos

Edição de departamentos existentes

Remoção de departamentos (com verificação de vendedores associados)

✅ Vendedores

Listagem completa com departamento associado

Cadastro com seleção de departamento

Edição de dados

Remoção segura

✅ Interface

Tabelas dinâmicas com dados do banco

Formulários modais para cadastro/edição

Alertas de confirmação e erro

Navegação entre telas

---

### 🎯 Aprendizados e Desafios
Este projeto foi fundamental para consolidar:

JavaFX – Criação de interfaces gráficas com FXML, Scene Builder, CSS

JDBC – Conexão com banco, execução de queries, tratamento de exceções

Padrão DAO – Separação da lógica de acesso a dados da regra de negócio

Arquitetura MVC – Organização clara entre Model, View e Controller

Integração – Comunicação entre interface gráfica e banco de dados relacional

---

## 📜 Licença

Este projeto é parte do curso da **DevSuperior** e tem propósito educacional.

---

## 👨‍💻 Autor

**Jacques Araujo Trevia Filho**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jacques-trevia)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Jacques-Trevia)
