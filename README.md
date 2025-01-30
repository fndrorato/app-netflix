# 🎬 Streamlit Frontend para API Netflix

Este projeto é um frontend desenvolvido com **Streamlit** para interagir com a [API Netflix](https://github.com/fndrorato/api-netflix), permitindo o gerenciamento de:

- 🎭 Atores e atrizes
- 🎞️ Gêneros de filmes
- 🎬 Filmes
- ⭐ Avaliações dos filmes
- 📊 Dashboard com estatísticas

## 🚀 Como rodar o projeto

### 1️⃣ Clonar o repositório
```bash
git clone https://github.com/seu-usuario/streamlit-netflix.git
cd streamlit-netflix
```

### 2️⃣ Criar e ativar um ambiente virtual
```bash
python -m venv venv
source venv/bin/activate  # No Windows: venv\Scripts\activate
```

### 3️⃣ Instalar as dependências
```bash
pip install -r requirements.txt
```

### 4️⃣ Configurar a API
Antes de iniciar o frontend, certifique-se de que a [API Netflix](https://github.com/fndrorato/api-netflix) está rodando localmente:

```bash
git clone https://github.com/fndrorato/api-netflix.git
cd api-netflix
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

A API estará disponível em: `http://127.0.0.1:8000/api/v1/`

### 5️⃣ Configurar o token de autenticação
Após rodar a API, obtenha um token de autenticação e adicione-o ao **Streamlit** na variável de sessão:

1. Acesse `http://127.0.0.1:8000/admin/` e crie um usuário.
2. Faça login na API e obtenha um token.
3. Adicione-o ao Streamlit na sessão `st.session_state.token`.

### 6️⃣ Rodar o Streamlit
```bash
streamlit run app.py
```

Acesse a aplicação no navegador pelo link exibido no terminal.

---

## 📌 Funcionalidades
✅ Cadastrar, listar e gerenciar atores/atrizes
✅ Cadastrar, listar e gerenciar gêneros
✅ Cadastrar, listar e gerenciar filmes
✅ Cadastrar e visualizar avaliações
✅ Dashboard interativo

---

## 🔧 Tecnologias utilizadas
- **Frontend:** Streamlit, Pandas, AgGrid
- **Backend:** Django REST Framework ([API Netflix](https://github.com/fndrorato/api-netflix))
- **Banco de dados:** PostgreSQL ou SQLite (dependendo da API)

---

## 🤝 Contribuição
Fique à vontade para contribuir! Basta abrir um **Pull Request** ou sugerir melhorias via **Issues**.

📩 **Contato:** [[LinkedIn](https://www.linkedin.com/in/fernandororato/)]

---

🚀 **Divirta-se criando sua lista de filmes favoritos!** 🎥🍿


