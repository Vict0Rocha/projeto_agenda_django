# Agenda

## Como executar o projeto

1. Clonar o repositório. <br/>
```
git clone https://github.com/Vict0Rocha/projeto_agenda_django.git
```
2. Criar o ambiente virtual.
```python
python -m venv venv
```
3. Ativar o ambiente "windows".
```python
.\venv\Scripts\activate
```
4. Instalar o Django
```python
pip install django
```
5. Iniciar o projeto
```python
django-admin startproject project .
```
6. Subir o servidor local
```python
python manage.py startapp contact
```
7. Migrando a base de dados do Django
```python
python manage.py makemigrations
python manage.py migrate
```
8. Criando e modificando a senha de um super usuário Django
```python
python manage.py createsuperuser
python manage.py changepassword USERNAME
```
Para rodar o projeto.
```python
python manage.py runserver
```
