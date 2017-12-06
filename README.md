# Desafio Mulesoft

Modele e construa uma API de Banco em RAML que tenha as seguintes operações:

1) Listar Clientes do Banco
2) Criar um novo Cliente do Banco
3) Listar todas as Contas de um determinado Cliente
4) Criar uma nova conta para um determinado Cliente
5) Alterar uma conta de um determinado Cliente

Modelo de tipos:
  Cliente:
    Deve conter um nome, cpf e endereço
  Conta:
    Deve conter agência, número da conta, tipo (uma opção entre poupança e conta corrente) e saldo

Uma vez definido o RAML importe seu conteúdo para o Anypoint Studio e gere uma API.

A API de Banco também deverá conter:

6) Uma busca de Empresas listadas no mercado de ações (EUA)
  Sua API deve ser capaz de retornar o resultado em JSON para a requisição:

  GET http://localhost:8080/api/banco/mercado/pesquisa?codigo=GOOGL

7) O último preço da ação da empresa:

  GET GET http://localhost:8080/api/banco/mercado/preco?codigo=GOOGL

Use como fonte de dados a API documentada em

 http://dev.markitondemand.com/MODApis/Api/v2/doc

Você deve usar o "Company Lookup API" e o "Stock Quote API". O resultado deve ser apresentado em JSON.

NOTA IMPORTANTE:
- Os itens de 1 a 5 não precisam ser implementados dentro do Anypoint Studio, apenas definido no RAML.
- Os itens 6 e 7 não precisam estar no RAML. Leia a documentação da Mulesoft para utilizar conectores HTTP como servidor e como cliente.