# 📘 API de Alunos — FastAPI + Jinja2

Este projeto é uma aplicação simples desenvolvida com **FastAPI** e **Jinja2**, que permite listar e cadastrar alunos com suas respectivas notas.  
A aplicação utiliza templates HTML para exibir os dados e possibilita a inclusão de novos registros via formulário.

---

## 🚀 Tecnologias Utilizadas

- [FastAPI](https://fastapi.tiangolo.com/) — Framework web moderno e rápido em Python  
- [Uvicorn](https://www.uvicorn.org/) — Servidor ASGI para executar aplicações FastAPI  
- [Jinja2](https://jinja.palletsprojects.com/) — Template engine para renderização de páginas HTML  

---

## ⚙️ Instalação

Clone o repositório e instale as dependências necessárias:

```bash
git clone https://github.com/seu-usuario/api-alunos.git
cd api-alunos
pip install fastapi uvicorn jinja2


---

▶️ Como Executar

Execute o servidor localmente com o comando:

uvicorn main:app --reload


Acesse no navegador:

👉 http://127.0.0.1:8000


---


📂 Estrutura de Pastas
api-alunos/
│
├── main.py               # Arquivo principal da aplicação
│
├── templates/            # Diretório de templates HTML
│   ├── alunos.html
│   └── cadastro.html
│
├── static/               # Arquivos estáticos (CSS, JS, imagens)
│
└── README.md


---


🧠 Funcionalidades

Listar alunos: Exibe uma tabela com nome e nota dos alunos cadastrados

Cadastrar novo aluno: Formulário simples para inserir novos registros

Renderização dinâmica: Utiliza Jinja2 para atualizar a lista em tempo real

🧩 Rotas da API
Método	Rota	Descrição
GET	/	Exibe a lista de alunos cadastrados
GET	/cadastro	Exibe o formulário de cadastro
POST	/cadastro	Salva um novo aluno na lista e redireciona para /
