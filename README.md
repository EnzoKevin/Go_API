# 🧩 Go_API

Uma API escrita em **Go (Golang)** com arquitetura limpa, organizada em camadas (`controller`, `usecase`, `repository`, `model`, `db`), e suporte a **Docker** e **Docker Compose**.  
Ideal para servir como base de projetos backend em Go.

---

## 🚀 Tecnologias Utilizadas

- 🦦 **Go** — Linguagem principal da aplicação  
- 🐳 **Docker** & **Docker Compose** — Containerização e orquestração  
- 🗃️ **Banco de Dados** — Suporte configurável (definido na pasta `db/`)  
- 🧱 **Arquitetura Limpa (Clean Architecture)** — Separação em camadas bem definidas

---

## 📂 Estrutura do Projeto

```
#Go_API/
        ├── cmd/ # Ponto de entrada da aplicação (main.go)
        ├── controller/ # Camada de controle (recebe requisições HTTP)
        ├── usecase/ # Lógica de negócio / casos de uso
        ├── repository/ # Acesso a dados e persistência
        ├── model/ # Estruturas de dados e modelos
        ├── db/ # Scripts e conexão de banco de dados
        ├── Dockerfile # Definição de imagem Docker
        ├── docker-compose.yml # Configuração de containers
        ├── go.mod # Dependências do projeto
        ├── go.sum # Verificação de dependências
        └── README.md # Documentação do projeto
```

---

### 🔧 Pré-requisitos

Antes de começar, certifique-se de ter instalado em sua máquina:

- [Go](https://go.dev/dl/) (versão 1.20 ou superior)  
- [Docker](https://docs.docker.com/get-docker/)  
- [Docker Compose](https://docs.docker.com/compose/install/)  
- [Git](https://git-scm.com/downloads)

### 🧩 1. Clonar o Repositório

```bash
git clone https://github.com/EnzoKevin/Go_API.git
cd Go_API
```

---


### EndPoints

     GET    - `/items`      - Lista todos os registros     
     GET    - `/items/{id}` - Busca um registro por ID     
     POST   - `/items`      - Cria um novo registro        
     PUT    - `/items/{id}` - Atualiza um registro        
     DELETE - `/items/{id}` - Remove um registro existente
