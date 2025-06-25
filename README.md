Sistema Helpdesk
Este é um projeto de um sistema de Helpdesk completo, desenvolvido com as tecnologias Angular 12 para o front-end e Spring Boot para o back-end. O sistema permite o gerenciamento de chamados de suporte, clientes e técnicos, com autenticação e autorização baseadas em token JWT.

🚀 Funcionalidades
O sistema oferece um conjunto robusto de funcionalidades para a gestão de suporte técnico:

Autenticação de Usuários:

Sistema de login com validação de credenciais (e-mail e senha).
Segurança de rotas com AuthGuard para garantir que apenas usuários autenticados acessem as páginas internas.
Uso de tokens JWT para autorização, com um interceptor que anexa o token a cada requisição HTTP.
Gerenciamento de Técnicos:

Funcionalidades de CRUD completo: criar, listar, atualizar e deletar técnicos.
Atribuição de perfis de usuário (Admin, Técnico) no momento do cadastro e atualização.
Gerenciamento de Clientes:

Funcionalidades de CRUD completo para os clientes do sistema.
Gerenciamento de Chamados:

Abertura de novos chamados com título, observações, prioridade e status.
Lista de chamados com paginação e filtros dinâmicos.
Capacidade de filtrar chamados por status (Aberto, Em Andamento, Encerrado).
Atualização e leitura detalhada de chamados existentes.
🛠️ Tecnologias Utilizadas
Este projeto foi construído com as seguintes tecnologias e bibliotecas:

Front-end:
Angular 12: Framework principal para a construção da SPA.
TypeScript: Superset do JavaScript que adiciona tipagem estática.
Angular Material: Biblioteca de componentes de UI para um design moderno e responsivo.
ngx-toastr: Biblioteca para a exibição de notificações e alertas.
ngx-mask: Para a aplicação de máscaras em campos de formulário (como CPF).
Back-end:
Java com Spring Boot 2 (Conforme mencionado no home.component.html).
⚙️ Pré-requisitos
Antes de começar, garanta que você tenha os seguintes softwares instalados:

Node.js (versão 14.15.0+ ou 12.14.1+).
Angular CLI v12.0.3: npm install -g @angular/cli@12.0.3
🏁 Como Rodar o Projeto
Clone o repositório

Bash

git clone https://github.com/icaropaixao/helpFrontSystem.git
cd helpFrontSystem
Instale as dependências
Este comando irá instalar todas as dependências listadas no package-lock.json para garantir a compatibilidade.

Bash

npm install
Configure o Back-end

Abra o arquivo src/app/config/api.config.ts.
Altere o valor da baseUrl para o endereço da sua API local (ex: http://localhost:8080).
Execute o projeto
O comando ng serve irá iniciar o servidor de desenvolvimento.

Bash

ng serve
Acesse a aplicação em http://localhost:4200/.