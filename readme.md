# Documentação da API

* Escolher um local do computador para criar o projeto
* Abrir o gitBash nesta pasta

Com o gitBash aberto executar o comando para criar a raiz do projeto:

```
mkdir NOME_PROJETO
```
Acessar a pasta
```
cd NOME_PROJETO
```
Comando para abrir o VSCode
```
code .
```
Criar o arquivo gerenciador de pacotes node
```
npm init -y
```
Criar arquivo .gitignore na raiz do projeto
```
touch .gitignore
```
Criar arquivo .env: arquivo para reservar variaveis do projeto
```
touch .env
```

## Instalar os pacotes do projeto

Instalar os pacotes para o projeto
```
npm i express nodemon dotenv
```
# express: será o servidor da api
# nodemon: atualizar os arquivos alterados sem parar o servidor
# dotenv: gerenciador de variaveis do ambiente

Criar pasta src
```
mkdir src
```
Criar arquivo server.js
```
touch src/server.js
```

Adicionar arquivos e pastas no gitignore
```
node_modules
.env
```
Adicionar a porta do servidor no .env
```
PORT = 3004
```
Configuração básica da api com express
```
app.listen(PORT, () => console.log('Servidor rodando na porta ${PORT}'));
```
Criar comando para rodar o servidor no arquivo package.json
```
"start":"nodemon src/server.js"
```
Rodar o servidor 
```
npm start
```
