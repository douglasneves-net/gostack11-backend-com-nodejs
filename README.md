## :computer: Projeto
<p>Projeto do zero utilizando o node.js e o framework express, instalamos o nodemon para realizar o reset da aplicação em cada modificação.</p>
<p>Os conceitos de métodos, parâmetros e middlewares foram aplicados, incluindo a utilização do middlewares em toda aplicação ou somente em algumas funções.</p>
<p>https://www.douglasneves.net/projetos/25-gostack11-noje-js-reactjs-e-react-native/41-back-end-com-node-js</p>

## :rocket: Tecnologias
- Node.js
- Express
- Nodemon 
- uuidv4

## Como usar ? 
<p>Baixe o projeto do github, depois execute o comando abaixo que vai baixar as dependencias.</p>
```bash yarn ```
<p>Agora execute o seguinte comando para executar a aplicação:</p>
```bash yarn dev ```

## Detalhes sobre a criação
yarn init -y // Inicia Projeto
node src/index.js //Executa node
yarn add nodemon -D
yarn add uuidv4

### Métodos HTTP
GET: Busca informações do back-end.
POST: Cria uma informação do back-end.
PUT: Altera uma informação no back-end(geral)
PATCH: Altera parte de uma informação no back-end(especifico)
DELETE: Deletar uma informação no back-end.


### Tipos de Parâmetros
Query Params: Filtros e paginação
Route params: Identifica recursos (Atualizar/Deletar).
Request Body: Conteúdo na hora de criar ou editar um recurso. (JSON)


## Middleware
Interceptador de requisições que pode interromper totalmente a requisição ou alterar dados da requisição.

## Ponto Importante
Sempre que vemos uma função com um request e um response podemos chamar de middleware.
Existe 3 formas de utilizar o middleware.
 No formato global com app.use(nomemiddleware());
 Direto em um outro middleware: app.put('/projects/:id', validateProjectId, (request, response)
 Ou declarando app.use('projects/:id', validateProjectId);
