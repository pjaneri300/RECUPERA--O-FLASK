# Projeto-Flask

-
Web App de Gerenciamento de Projetos

-Descrição do Projeto:
Este é um sistema web de gerenciamento de projetos desenvolvido com Flask. Ele permite que os usuários criem, editem e removam projetos, além de gerenciar tarefas associadas a cada projeto. As tarefas podem ser adicionadas, editadas, removidas e filtradas por status. Os dados são armazenados em arquivos CSV (projetos.csv e tarefas.csv), e o frontend utiliza HTML com Tailwind CSS para uma interface amigável e responsiva.

-Funcionalidades Implementadas:

-Cadastrar Projetos: Crie projetos com nome, descrição e data de criação.

-Listar Projetos: Visualize todos os projetos em uma lista.

-Editar Projetos: Altere nome e descrição de projetos existentes.

-Remover Projetos: Exclua projetos (remove também as tarefas associadas).

-Adicionar Tarefas aos Projetos: Adicione tarefas com título, descrição e status (Pendente, Em andamento, Concluída).

-Editar e Remover Tarefas: Modifique ou exclua tarefas.

-Visualizar Tarefas de um Projeto: Veja todas as tarefas de um projeto específico.

-Filtro por Status das Tarefas: Filtre tarefas por status dentro de um projeto.

-Barra de Progresso do Projeto: Exiba o progresso do projeto com base nas tarefas concluídas.

-Funcionalidades Não Implementadas (Extras)

-Upload de Imagem por Projeto: Não implementado.
-Migração para MySQL: O projeto utiliza apenas CSV para armazenamento.

-Requisitos Técnicos:
Backend: Flask (Python)
Frontend: HTML com Tailwind CSS (via CDN)
Armazenamento: Arquivos CSV (projetos.csv e tarefas.csv)
Rotas: Organizadas de forma RESTful

Estrutura do Projeto:

```
gerenciador_projetos/
│
├── static/                 # Arquivos estáticos (CSS, JS, imagens, etc.) - vazio neste projeto
├── templates/              # Templates HTML
│   ├── base.html           # Template base
│   ├── index.html          # Página inicial (lista de projetos)
│   ├── projeto.html        # Página de detalhes de um projeto
│   ├── nova_tarefa.html    # Formulário para nova tarefa
│   ├── editar_projeto.html # Formulário para editar projeto
│   └── editar_tarefa.html  # Formulário para editar tarefa
├── projetos.csv            # Arquivo CSV para armazenar projetos
├── tarefas.csv             # Arquivo CSV para armazenar tarefas
├── [app.py](http://app.py/)                  # Código principal do Flask
└── [README.md](http://readme.md/)               # Documentação do projeto
```

Pré-requisitos:

Python 3.8 ou superior
Flask (pip install flask)

-Instruções de Instalação e Execução:

-Clone o repositório:
git clone <URL_DO_REPOSITORIO>
cd gerenciador_projetos

-Crie e ative um ambiente virtual (opcional, mas recomendado):
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows

-Instale as dependências:
pip install flask

-Execute o projeto:
python [app.py](http://app.py/)

-Acesse o sistema:
Abra o navegador e acesse http://127.0.0.1:5000/.

-Exemplos de Uso:

-1. Listar e Criar Projetos

Acesse a página inicial (/) para ver a lista de projetos.
Use os botões "Editar" e "Excluir" para gerenciar projetos.

-2. Gerenciar Tarefas

Clique em um projeto para ver suas tarefas.
Use o botão "Nova Tarefa" para adicionar tarefas.
Filtre tarefas por status usando o menu suspenso.
Edite ou exclua tarefas conforme necessário.

-3. Barra de Progresso

Na página inicial, cada projeto exibe uma barra de progresso baseada na porcentagem de tarefas concluídas.

-Arquivos CSV de Exemplo:

-projetos.csv:
id,nome,descricao,data_criacao
1,Projeto Exemplo,Um projeto de exemplo para demonstração,2025-05-09

-tarefas.csv:
id,projeto_id,nome,descricao,status
1,1,Tarefa Exemplo,Descrição da tarefa exemplo,Pendente
2,1,Tarefa 2,Segunda tarefa do projeto,Concluída

-IMAGENS DO FUNCIONAMENTO DO PROJETO

-Página Inicial:

![1.png](attachment:3d055cb4-6b9f-46fc-8d18-4263a24d7b1c:1.png)

-Páginas das tarefas:

![6.png](attachment:7131c113-cfbe-46b1-ae09-d1c9488f34ad:6.png)

-Páginas para criar novas tarefas:

![2.png](attachment:e0c41638-8a62-4121-98b7-00fa2550c8a8:2.png)

-Página com as novas tarefas:

![3.png](attachment:59025daf-fe41-4c34-adf7-6bbabd755536:3.png)

-Página para editar as tarefas existentes:

![Captura de tela 2025-05-09 085643.png](attachment:02b901c3-a4d8-45b4-848e-1c0aba3a2cdb:Captura_de_tela_2025-05-09_085643.png)

-Página com a tarefa editada:

![Captura de tela 2025-05-09 085741.png](attachment:e4709b0a-9486-4de0-95a3-d5297d3a7872:Captura_de_tela_2025-05-09_085741.png)

-Página com a tarefa excluida:

![6.png](attachment:8f5b1997-ddc2-4336-b675-48c8fb4c60fb:6.png)
