# 📒 Agenda telefônica

Este repositório contém uma aplicação de Agenda Telefônica desenvolvida com o __framework Django.__
O projeto vai além de um simples CRUD, oferece funcionalidades como...

*  Autenticação de usuários – Criação de conta, login e logout
*  Gerenciamento de contatos – Criar, editar, excluir e listar contatos
*  Categorias – Organize contatos por categorias personalizadas
*  Upload de foto – Salve imagens para cada contato
*  Busca e filtros – Localize contatos
*  Validação de dados – Garantia de consistência nas informações

---

## 🛠️ Tecnologias utilizadas

* Python
* Django
* SQLite (banco de dados padrão do Django)
* HTML5, CSS3 (para o front-end)

---

## 📂 Estrutura do projeto

```bash
projeto_agenda_django/
│
├── base_static/                 # Arquivos estáticos (CSS)
│
├── base_templates/              # Templates base e parciais
│   └── global/partials/         # Cabeçalho, mensagens, paginação etc...
│
├── contact/                     # Aplicação principal
│   ├── models.py                # Modelos: Contact, Category
│   ├── views/                   # Views organizadas em múltiplos arquivos
│   │   ├── __init__.py          # Import central de todas as views
│   │   └── user_forms.py        # Formulários de registro/edição de usuário
│   ├── urls.py                  # Rotas da aplicação
│   └── templates/contact/       # Templates específicos da app
│
├── utils/                       # Scripts auxiliares
│   └── create_contacts.py       # Gera dados falsos para popular o banco
│
├── media/                       # Pasta para upload de imagens de contatos
│
├── project/                     # Configurações do projeto Django
│   ├── settings.py              # Configurações globais (templates, static, media)
│   ├── urls.py                  # Rotas principais
│   └── wsgi.py
│
├── manage.py                    # Comando principal do Django
└── requirements.txt             # Dependências do projeto
```

---

## ⚙️ Como Executar o Projeto

Siga os passos abaixo para rodar o projeto LOCALMENTE.


1. Clone este repositório. <br/>
```
git clone https://github.com/Vict0Rocha/projeto_agenda_django.git
```

2. Crie e ative um ambiente virtual.
```python
python -m venv venv         # Para criar
venv\Scripts\activate       # Ativar no windows
source venv/bin/activate    # Ativar no Linux/Mac
```

3. Instale as dependências
```python
pip install -r requirements.txt
```

4. Execute as migrações
```python
python manage.py makemigrations
python manage.py migrate
```

5. Inicie o servidor de desenvolvimento
```python
python manage.py runserver
```

6. Acesse no navegador
```python
http://127.0.0.1:8000/
```

### Caso queira criar um superusuário (opcional, para acessar o admin)
```python
python manage.py createsuperuser
```

---

## 🖼️ Demonstração

<img width="1000" height="800" alt="image" src="https://github.com/user-attachments/assets/74bea5ed-a2d3-4cda-932b-30db6f5b38ed" />


---

## 📄 Licença

Este projeto está licenciado sob a licença MIT – veja o arquivo LICENSE
 para mais detalhes.

---

## 👨‍💻 Autor

Desenvolvido por [Victor Cordeiro](https://portfolio-victor-cordeiro.vercel.app/) 
