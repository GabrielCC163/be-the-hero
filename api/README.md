Be The Hero API (NodeJS) \
DB: SQlite \
Query Builder: Knex.js

Step for create knexfile.js: npx knex init

Steps for create a table: \
Create the migrations folder inside database dir. \
Run npx knex migrate:make create_ongs \
Write the createTable method inside "up" and dropTable method inside "down" in database/migrations/migration_file_example.js \
Run npx knex migrate:latest for creating the table on DB. \
*Note: npx knex migrate:rollback for undo the last migration \
*Note: npx knex migrate:status for list all the migrations

Steps for setup Jest: \
npx jest --init (run it once) \
yarn test (for running the tests) \
*Teste de integração: Testa por completo uma funcionalidade da aplicação. \
*Teste unitário: Testa uma função isolada.

 * Tipos de parâmetros:
 
 * Query Params: enviados na rota após o "?" (Filtros, paginação)
 *      req.query; name=Gabriel&idade=25 => {name: 'Gabriel', idade: '25'}
 
 * Route Params: utilizados para identificar recursos
 *      req.params; /users/1 => {id: '1'}
 
 * Request Body: Corpo da requisição, utilizado para criar ou alterar recursos
 *      req.body; {"name": "Gabriel", "idade": 25}

 To implement: \
 ESLint, Prettier \
 Auth with JWT \
 Styled Components (React e React Native) 