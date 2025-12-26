# zpErp
Controle total da sua vida em um só lugar. Simples assim.

O que é isso?
Eu cansei de ter meus dados espalhados em mil apps diferentes. Gastos no Excel, tarefas no Google Keep, treinos no caderninho... Um caos total.
Daí pensei: por que não fazer um sistema só pra mim? Um lugar onde eu tenho controle de tudo que importa na minha vida.
Não é sobre ser perfeito. É sobre funcionar e me ajudar de verdade.

O que ele faz?
Por enquanto, o básico que eu preciso:

Financeiro

Anoto todas as receitas e despesas
Vejo onde tá indo minha grana (spoiler: sempre é ifood)
Acompanho se tô conseguindo economizar
Relatórios simples pra entender o mês

Tarefas

Lista do que preciso fazer
Kanban básico (a fazer → fazendo → feito)
Filtros pra não me perder
Nada de gamificação ou firula

Dashboard

Resumo de tudo numa tela só
Gráficos que fazem sentido
Dados que eu realmente uso

Por que fiz isso?

Aprender fazendo - Teoria é legal, mas sujar a mão é melhor
Resolver meu problema - Se funciona pra mim, já valeu
Ter algo pra mostrar - Portfólio que não é todo list genérico
Controlar meus dados - Meus dados, meu servidor, minhas regras

Stack
Escolhi tecnologias que eu quero dominar de verdade:
Frontend:

Vue 3 (Composition API)
TypeScript (java pros fracos)
shadcn-vue (componentes prontos e bonitos)
Vite (react é pra emocionado)
pnpm (gerenciador de pacote que funciona & eficiente)

Backend:

NestJS (estrutura que faz sentido)
TypeScript (consistência é bom)
Sequelize ORM (falar com banco de forma humana)
JWT (autenticação sem segredo)
Docker (ambiente reproduzível)

Banco:

MariaDB (confiável e rápido)

Como rodar
Pré-requisitos

Node.js 18+
pnpm (npm install -g pnpm)
Docker & Docker Compose

Setup
bash# Clona o repo
git clone https://github.com/seu-usuario/personal-erp.git
cd personal-erp

# Sobe o banco
docker-compose up -d

# Backend
cd backend
pnpm install
pnpm run start:dev

# Frontend (em outro terminal)
cd frontend
pnpm install
pnpm run dev
Acessa http://localhost:5173 e pronto.
Estrutura
personal-erp/
├── frontend/           # Vue 3 + shadcn
├── backend/            # NestJS
├── docker-compose.yml  # MariaDB
└── README.md           # você está aqui
Cada módulo é independente. Financeiro não depende de Tarefas. Se eu quebrar algo, não quebra tudo.
Roadmap
Não é promessa, é intenção:

 Autenticação básica
 Módulo Financeiro
 Módulo Tarefas
 Dashboard com resumo geral
 Módulo Saúde (treinos, peso)
 Módulo Estudos (livros, cursos)
 Relatórios em PDF
 App mobile (talvez?)

Vou adicionando conforme sinto necessidade. Sem pressão.
Aprendizados
O que tô tirando desse projeto:

Arquitetura modular na prática
Relacionamentos de banco de dados
Autenticação JWT do jeito certo
Gerenciamento de estado no Vue
Docker pra desenvolvimento
TypeScript em projeto real

Contribuindo
Por enquanto é só meu. Mas se você quer fazer um fork e adaptar pro seu uso, vai fundo. Código tá aí pra isso.

Licença
MIT - faça o que quiser

Contato
Se quiser trocar ideia sobre o projeto ou sobre desenvolvimento em geral, me chama.

Feito com café, música e tentativa e erro.
