## ✈ Gerenciador de Projetos

** Descrição do Projeto 
Este é um sistema web de gerenciamento de projetos desenvolvido com Flask. Ele permite que os usuários criem, editem e visualizem projetos, além de gerenciar tarefas associadas a cada projeto. As tarefas podem ser adicionadas, editadas, excluídas e categorizadas por status (Pendente, Em Andamento, Concluído). Os dados são armazenados em arquivos CSV (projetos.csv e tarefas.csv), e o frontend utiliza HTML com Tailwind CSS para uma interface moderna, responsiva e amigável.
🛴 Funcionalidades Implementadas

Cadastrar Projetos: Crie projetos com nome e descrição.
Listar Projetos: Visualize todos os projetos em uma interface de cartões.
Editar Projetos: Modifique nome e descrição de projetos existentes.
Adicionar Tarefas aos Projetos: Adicione tarefas com nome e status.
Editar e Remover Tarefas: Atualize ou exclua tarefas de um projeto.
Visualizar Tarefas de um Projeto: Veja todas as tarefas associadas a um projeto específico.
Armazenamento: Utiliza arquivos CSV para persistência de dados.

Observação: A funcionalidade de remover projetos (e suas tarefas associadas) não está implementada no código atual.
🚤 Requisitos Técnicos

Backend: Flask (framework Python)
Frontend: HTML com Tailwind CSS (via CDN)
Armazenamento: Arquivos CSV (projetos.csv e tarefas.csv)
Rotas: Organizadas de forma simples e funcional

🚗 Estrutura do Projeto
gerenciador_projetos/
│
├── templates/              # Templates HTML
│   ├── base.html           # Template base com layout comum
│   ├── index.html          # Página inicial (lista de projetos)
│   ├── projeto.html        # Página de detalhes de um projeto
│   ├── nova_tarefa.html    # Formulário para nova tarefa
│   ├── editar_projeto.html # Formulário para editar projeto
│   └── editar_tarefa.html  # Formulário para editar tarefa
├── projetos.csv            # Arquivo CSV para armazenar projetos
├── tarefas.csv             # Arquivo CSV para armazenar tarefas
├── app.py                  # Código principal do Flask
└── README.md               # Documentação do projeto

Nota: A pasta static/ não é utilizada, pois o Tailwind CSS é carregado via CDN.
🚅 Instruções de Instalação e Execução

Clonar o Repositório (se aplicável):
git clone <URL_DO_REPOSITORIO>
cd gerenciador_projetos

Alternativamente, copie os arquivos para um diretório local.

Criar e Ativar um Ambiente Virtual (opcional, mas recomendado):
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows


Instalar Dependências:
pip install flask


Executar o Projeto:
python app.py


Acessar o Sistema:
Abra o navegador e acesse http://127.0.0.1:5000/.


🚒 Exemplos de Uso

Listar e Gerenciar Projetos:

Acesse a página inicial (/) para ver todos os projetos em um layout de cartões.
Clique em "Ver Projeto" para visualizar detalhes e tarefas ou em "Editar" para modificar nome e descrição.


Gerenciar Tarefas:

Na página de um projeto, clique em "Nova Tarefa" para adicionar uma tarefa com nome e status.
Edite ou exclua tarefas usando os links "Editar" e "Excluir" ao lado de cada tarefa.



Observações

A interface utiliza um esquema de cores roxo e branco.
Os arquivos CSV (projetos.csv e tarefas.csv) são criados automaticamente na primeira execução, se não existirem.
Certifique-se de que o diretório do projeto tenha permissões de escrita para manipulação dos arquivos CSV.
A funcionalidade de remover projetos não foi implementada no código fornecido.

