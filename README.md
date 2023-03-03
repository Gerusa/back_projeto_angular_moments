# Sobre
* Esta api é um clone do repositório do Matheus Battisti: https://github.com/matheusbattisti/curso_angular_yt. Ela refere-se ao back do projeto do angular (repositório 'angular').

# O que é AdonisJS
* AdonisJS é uma estrutura MVC do Node.js que oferece ao usuário um ecossistema estável para escrever aplicativos web. Em síntese, é uma estrutura de back-end para Node.js, escrita em TypeScript.
* Ele é um framework robusto e com uma biblioteca completa para facilitar a vida da pessoa desenvolvedora, que não precisa utilizar outros recursos.
* Ele vem com várias funcionalidades prontas, como ORM, autenticação, validação, envio de e-mail, logging, entre outras.

## Passos
 - 1 - Após o projeto aberto no vs code, foi executado o comando 'npm install' para baixar as dependências
- 2 - Em seguida executado o comando 'node ace serve' para rodar a api
	- Este comando falhou, devido a ausência da variável 'APP_KEY'
		- Executado 'node ace generate:key'
		- Copiado o arquivo '.env.example' e colado com o nome de '.env'
		- Substituído o valor da APP_KEY pela gerada após a execução do comando
		- Reexecutado o comando 'node ace serve'
- 3 - Passos para o banco
* O projeto possui os arquivos de banco dentro da pasta database/migrations.
* Executado o comando 'node ace migration:run'
* O banco é o sqlite -> foi instalada a extensão 'sqlite viewr' dentro do vsCode
	* Após isso, foi possível visualizar os dados gerados com o comando acima, ao clicar em 'tmp/db.sqlite3'

- 4 - Executado o comando 'node ace serve' para subir a aplicação
- 5 - Criada collection Adonis Api no Postman