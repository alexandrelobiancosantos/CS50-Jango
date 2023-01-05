05/01/2023
CS50 - Django - Aula 3
Alexandre Lo Bianco


Django: Web Framework

1-Istalação
> pip install Django

2-Iniciar o projeto lecture3
>django-admin startproject lecture3

3-Estrutura do projeto criada
alguns arquivos importantes so projeto são:

manage.py
    Executa comandos no projeto
settings.py
    Configurações do django
urls.py
    tabela de conteudo da aplicação(rotas)

4-Rodar aplicação
>python manage.py runserver

5-Criar o primeiro App hello
>python manage.py startapp hello

6-Estrutura do app
Alguns arquivos importantes so projeto são:
views.py
    front-end do app

7-Instalar o app hello no projeto lecture3
No arquivo lecture3/settings.py, procurar 'INSTALED_APPS' e adicionar o hello

8-Criar um frontend em views.py
importar HttpResponse
criar função index

9-Criar url do app hello
criar urls.py dentro do diretorio hello
 importar path
 importar views.py
 criar path e nomear para facilitar refenciar a função futuramente

10-adicionar path do app no urls.py da pasta do projeto

11-Rodar projeto


12-criar nova função em views.py


----
1- Criar função com placeholders
2- Upgrade HttpResponse para Render nas funções definidas em views.py
criar template html

---
Novo app: 37:00
Fluxo de trabalho para um novo app newyear:
>python manage.py startapp newyear
Adicionar novo app, newyear, em lecture3/settings.py
Adiconar path em lecture3/urls.py
Criar urls.py na pasta da app newyear
Criar função index em views com logica em python para capturar valor da data atual
Criar template html em templates/newyear/index.html com logica de if para testar se é ano novo
---
arquivos estaticos, como style.css
---
Novo app tasks
>python manage.py startapp tasks
Adicionar novo app, tasks, em lecture3/settings.py
Adiconar path em lecture3/urls.py
Criar função index em views com logica em python que define a lista de tarefas
Criar template html em templates/tasks/index.html com logica de loop para varrer a lista de tarefas definidas na função
---
Herança

