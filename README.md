Avaliação Prática: Sistema de Gerenciamento de Turmas e Atividades
Finalidade

Desenvolver um sistema web completo (front-end e back-end) voltado ao controle de turmas e atividades docentes, possibilitando que professores realizem o cadastro, consulta e exclusão de suas turmas e tarefas de forma simples e eficiente.

Contexto

A desorganização no registro das atividades aplicadas pelos professores pode comprometer o acompanhamento do aprendizado e dificultar a gestão pedagógica.
Em escolas localizadas em regiões com poucos recursos tecnológicos, a falta de um sistema de controle adequado acaba impactando negativamente o processo de ensino e o desempenho dos alunos.

Proposta

O desafio consiste em criar uma aplicação que permita ao professor:

Fazer login de forma segura;

Consultar, cadastrar e remover suas turmas;

Registrar atividades vinculadas a cada turma;

Efetuar logout de maneira confiável.

Requisitos Técnicos do Ambiente

Para garantir o funcionamento correto da aplicação, o ambiente deve atender aos seguintes pré-requisitos:

1. Banco de Dados

SGBD utilizado: MySQL

Versão mínima recomendada: 8.0

Observação: Criar um banco de dados exclusivo para o projeto, configurando o usuário e senha conforme necessidade.

2. Servidor e Sistema Operacional

Sistema Operacional sugerido: Windows 10 ou 11

Servidor de aplicação: Node.js

Versão recomendada: 18 ou superior

3. Linguagens e Ferramentas

Back-end: JavaScript com Node.js, Express e Prisma ORM

Front-end: HTML e CSS

Banco de Dados: MySQL

Etapas de Instalação e Execução

Siga as etapas abaixo para configurar e executar o sistema em ambiente local:

1. Clonar o Repositório
git clone https://github.com/Leozin99/escolaavaliacao.git
cd escolaavaliacao

2. Instalar as Dependências
npm install


ou

npm i

3. Configurar o Banco de Dados

Crie um banco de dados MySQL destinado ao sistema;

No arquivo .env, defina o acesso conforme o exemplo:

DATABASE_URL="mysql://root@localhost:3306/nome_do_banco"

4. Executar as Migrations do Prisma
npx prisma migrate dev --name init

5. Iniciar o Servidor
npm run dev


Após isso, o sistema estará disponível no endereço: http://localhost:3001.

6. Realizar os Testes

O sistema pode ser testado diretamente pelo navegador ou utilizando ferramentas como Insomnia ou Postman;

Funcionalidades que devem ser verificadas:

Criação, listagem, edição e exclusão de turmas;

Registro, visualização, edição e exclusão de atividades;

Login e logout de professores.
