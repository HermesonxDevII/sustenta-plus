# Atividade Parcial (Projeto Aplicado a Multiplataformas Etapa 2)

## 1. Título e descrição do projeto

### Nome do sistema:
- Sustenta Plus

### Breve descrição do propósito:
- Este trabalho apresenta o desenvolvimento de uma aplicação web voltada à coleta de denúncias ambientais relacionadas ao descarte inadequado de resíduos sólidos em áreas urbanas. O sistema permite que usuários registrem ocorrências por meio de formulários estruturados e envio de imagens, armazenando as informações em um banco de dados para posterior análise.

- As denúncias são disponibilizadas em um painel administrativo acessado por representantes do setor público, possibilitando a triagem, o acompanhamento e a tomada de decisões. A aplicação visa fortalecer a participação cidadã, otimizar a gestão pública e contribuir para práticas urbanas mais sustentáveis.

### Problema solucionado:
- O problema solucionado por este sistema é a dificuldade que os cidadãos enfrentam para informar às autoridades sobre pontos de descarte irregular de lixo e falhas na coleta urbana. Muitas dessas ocorrências não são registradas oficialmente, o que dificulta a tomada de providências e contribui para a poluição e a degradação do ambiente urbano.

---

## 2. Funcionalidades implementadas

### Lista de funcionalidades principais
- Cadastro de denúncias por parte dos cidadãos através de formulário.
- Armazenamento e organização dos registros em banco de dados.
- Exibição das denúncias em um painel administrativo destinado aos órgãos responsáveis.
- Possibilidade de acompanhamento e controle das denúncias recebidas.

### Status de implementação
- Parcial

### Screenshots das telas principais
![Home](./docs/img/Home.png)
![Reports](./docs/img/Reports.png)

## Mais fotos
🖼️[Screenshots](./docs/screenshots/screenshots.md)

---
## 3. Tecnologias utilizadas

### Linguagens de programação
- 🔷 Typescript — Tipagem estática para maior segurança e organização do código.

### Frameworks e bibliotecas

#### Frontend
- ⚛️ React — Biblioteca para construção da interface do usuário.
- 🎨 Tailwind CSS — Estilização rápida e responsiva com classes utilitárias.

#### Backend
- 🚂 Express.js — Framework para construção da API.
- 🗄️ Sequelize — ORM para manipulação do banco de dados.

### Banco de Dados
- 🐬 MySQL

###  Ferramentas de desenvolvimento
- 🟦 VsCode

---

## 4. Arquitetura do sistema

### Visão geral da arquitetura implementada

- A aplicação foi desenvolvida utilizando uma arquitetura do tipo cliente-servidor, onde o front-end é responsável pela interface com o usuário e o back-end realiza o processamento das informações, a comunicação com o banco de dados e as regras de negócio.

### Componentes principais

#### Frontend
- Formulário de denúncia, responsável pela coleta das informações e imagens.
- Componentes de input e upload de imagens, utilizados para preencher os dados necessários.
- Página de listagem de reportes, onde é possível visualizar as denúncias registradas.

#### Backend
- Servidor Express, responsável pelo gerenciamento das rotas da aplicação.
- Controladores (Controllers), que tratam as requisições recebidas.
- Models, definidos pelo Sequelize para manipulação dos dados no banco.
- Banco de dados relacional, utilizado para armazenar as informações das denúncias.

### Integrações realizadas

#### Frontend
- React e API, por meio de requisições HTTP (GET e POST).

#### Backend
- API e banco de dados relacional utilizando o ORM Sequelize.

---

## 5. Instruções de instalação e execução

### Pré-requisitos
### Passo a passo para instalação
### Comandos para execução
### Configurações necessárias

---

## 6. Acesso ao sistema

### Acesso ao sistema
### Credenciais de teste

---

## 7. Validação com Público-Alvo

### Definição específica do público-alvo
### Resumo do processo de validação
### Principais feedbacks recebidos
### Ajustes implementados

---

## 8. Equipe de desenvolvimento

| Nome                                     | Matricula  | Constribuição              |
| ---------------------------------------- | ---------- | -------------------------- |
| [Francisco Hermeson O. dos Santos]       | [2326241]  | Desenvolvedor(a)           |
| [Maria Joselene da Costa C. de Barcelos] | [2314797]  | Desenvolvedor(a)           |
| [Francisco Clay Oliveira]                | [2317574]  | Documentação               | 
| [Francisco Tayson Araujo santos]         | [2323799]  | Testes                     | 
| [Leonardo Estevão Silva Dos Santos]      | [2315238]  | Testes                     | 
---

## 📦 Instalação e Configuração

### ✅ Clonar o repositório
```bash
git clone https://github.com/HermesonxDevII/sustenta-plus.git
cd sustenta-plus
```

### ✅ Criar ambiente virtual
```bash
python -m venv venv
```

## ✅ Acessar ambiente virtual

#### ✅ Windows
```bash
venv\Scripts\activate
```

#### ✅ Linux/Mac
```bash
source venv/bin/activate
```

### ✅ Instalar dependências
```bash
pip install -r requirements.txt
```

### ✅ Configurando variáveis de ambiente

- Após os passos acima abra o projeto no vs code para editar as variáveis de ambiente, se ja estiver no diretorio dele no terminal basta digitar `code .` que o projeto sera aberto.

- Dentro do projeto basta editar o nome do arquivo `.env.example` para `.env` e preencher as variáveis de la que são essas abaixo.

```bash
DATABASE_URL=
TEST_DATABASE_URL=
AUTH_SECRET_KEY=
AUTH_ALGORITHM=
```

- As variáveis de banco (`DATABASE_URL` e `TEST_DATABASE_URL`) não são obrigatorias pois ja esta configurado como padrão para usar sqlite na aplicação, mas se quiser usar outro banco coloque o `DSN` dele nessas duas variáveis.

- Para gerar sua `AUTH_SECRET_KEY` para digitar no terminal o comando abaixo, e copiar e colar o resultado dele na variavel.

```bash
python generate_secret.py
```

- E sobre o `AUTH_ALGORITHM` você pode usar o que quiser, por padrão usamos `HS256`.

### ✅ Executar aplicação
```bash
uvicorn src.main:app --reload
```

---

## 👩‍💻 Atribuição de funções:


---

## 📚 Documentação de Rotas
- 🗂️ [Arquitetura](docs/architecture.md)
- 🔐 [Authenticação](docs/authentication.md)
- 🏢 [Empresas](docs/companies.md)
- 🏫 [Instituições](docs/institutions.md)
- 🎁 [Doações](docs/donations.md)

---

## 📥 Coleção Postman

Na raiz do projeto existe uma pasta chamada **`/postman`** contendo a coleção completa de requisições para facilitar os testes da API.

---

## 🐳 Tecnologias Utilizadas

- Python
- FastAPI

---