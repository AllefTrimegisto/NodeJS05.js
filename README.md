# NodeJS05.js

Crie um código Node.JS usando a biblioteca Express. Nele, você deve receber quatro tipos de requisições e responder cada uma com strings diferentes. Por fim, explique como rodar o código.

const express = require('express');
const app = express();
const port = 8080;

app.get('/', (req, res) => {
  res.send('Bem-vindo ao servidor');
});

app.post('/', (req, res) => {
  res.send('Requisição POST recebida com sucesso');
});

app.put('/', (req, res) => {
  res.send('Requisição PUT recebida com sucesso');
});

app.delete('/', (req, res) => {
  res.send('Requisição DELETE recebida com sucesso');
});

app.listen(port, () => {
  console.log(`Servidor rodando na porta ${port}`);
});
