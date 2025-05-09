📌 Visão Geral

Este aplicativo web, desenvolvido com Flask, oferece uma solução simples e eficiente para organizar projetos e tarefas. Os usuários podem criar, editar e excluir projetos, além de gerenciar tarefas vinculadas a cada projeto com diferentes status. Os dados são persistidos localmente em arquivos CSV, e a interface é construída com HTML + Tailwind CSS para garantir responsividade e usabilidade.

⚙ Funcionalidades Disponíveis

📁 Projetos

Criar Projetos: Insira nome, descrição e data de criação.

Visualizar Projetos: Veja todos os projetos cadastrados.

Editar Projetos: Altere as informações de projetos existentes.

Excluir Projetos: Remove o projeto e todas as suas tarefas vinculadas.

✅ Tarefas

Adicionar Tarefas: Crie tarefas com título, descrição e status (Pendente, Em andamento, Concluída).

Editar Tarefas: Atualize os dados das tarefas conforme necessário.

Excluir Tarefas: Remova tarefas específicas de um projeto.

Visualizar Tarefas: Veja as tarefas associadas a um projeto.

Filtrar por Status: Exiba tarefas com base em seu status atual.


### 📀 Armazenamento

O sistema utiliza exclusivamente arquivos CSV (projetos.csv e tarefas.csv) para guardar os dados.

### 🧰 Requisitos Técnicos

Backend: Python (Flask)

Frontend: HTML com Tailwind CSS (via CDN)

Banco de Dados: Arquivos CSV

Organização de Rotas: Padrão RESTful

### 📁 Estrutura de Pastas

gerenciador_projetos/
│
├── static/                   # Arquivos estáticos (CSS, imagens etc.)
├── templates/                # Templates HTML para as páginas
│   ├── base.html
│   ├── index.html
│   ├── projeto.html
│   ├── nova_tarefa.html
│   ├── editar_projeto.html
│   └── editar_tarefa.html
├── projetos.csv              # Dados dos projetos
├── tarefas.csv               # Dados das tarefas
├── app.py                    # Código principal da aplicação Flask
└── README.md                 # Documentação do projeto

### 🚀 Como Executar o Projeto
'''
git clone <URL_DO_REPOSITORIO>
cd gerenciador_projetos
'''
'''
(Opcional) Crie um ambiente virtual:

python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
'''
Instale o Flask:
'
pip install flask

Execute a aplicação:

python app.py
'
Acesse no navegador:http://127.0.0.1:5000/

### 🧪 Exemplos de Uso

Tela InicialVeja a lista de projetos, com opções para editar ou excluir cada um.

Visualização de ProjetosClique em um projeto para ver e gerenciar suas tarefas.

Adicionar TarefaUse o botão “Nova Tarefa” para incluir uma nova atividade.

Filtrar TarefasSelecione o status para filtrar tarefas (por exemplo, só as "Concluídas").

Editar e ExcluirAtualize ou remova tarefas conforme a necessidade.

Acompanhamento VisualBarra de progresso mostra a porcentagem de tarefas finalizadas no projeto.


## 🌍Imagens Do Funcionamento Do Projeto

-Página Inicial:

![1.png](https://github.com/pjaneri300/RECUPERA--O-FLASK/blob/main/static/img/1.png)

-Páginas das tarefas:

![6.png](https://github.com/pjaneri300/RECUPERA--O-FLASK/blob/main/static/img/2.png)

-Páginas para criar novas tarefas:

![2.png](https://github.com/pjaneri300/RECUPERA--O-FLASK/blob/main/static/img/3.png)

-Página com as novas tarefas:

![3.png](https://github.com/pjaneri300/RECUPERA--O-FLASK/blob/main/static/img/4.png)

-Página para editar as tarefas existentes:

![Captura de tela 2025-05-09 085643.png](https://github.com/pjaneri300/RECUPERA--O-FLASK/blob/main/static/img/5.png)

-Página com a tarefa editada:

![Captura de tela 2025-05-09 085741.png](https://github.com/pjaneri300/RECUPERA--O-FLASK/blob/main/static/img/6.png)

-Página com a tarefa excluida:

![6.png](https://github.com/pjaneri300/RECUPERA--O-FLASK/blob/main/static/img/7.png)
