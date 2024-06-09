# Primeiros passos

primeiramente clone o repositorio,

Em seguida no terminal digite - `npm i` para instalar todas as dependências,

Em seguida no mesmo terminal digite - `npm start` para iniciar a aplicação,

Se ainda não tem o thunder instalado, então instale a extensão Thunder Client,



### Registrndo usuario:

No thunder, na are de colocar o link você colocara o seguinte link:

`http://localhost:3000/register`

tenha a certeza de estar utilizando o metodo `POST`,

Cadastra um novo Usuario da seguinte forma: (OBS: deve digitar o codigo abaixo na aba body)

#### Corpo da Requisição (HTTP BODY)

```json
{

 "username": "exemplo",

"email": "exemplo@gmail.com",

"password": "exemplo"

}
```

### Logando no usuario:

Se tudo estiver correto você tera o seu usario cadatrado com sua senha criptografada,

Em seguida utilize o link:

http://localhost:3000/login

para logar no seu usuario, 

Forma correta de logar: (OBS: deve digitar o codigo abaixo na aba body)

#### Corpo da Requisição (HTTP BODY)

```json
{

"email": "exemplo@gmail.com",

"password": "exemplo"

}
```
isso ira gerar um token.

### Utilizando meu usuario:

Em seguida utilize o seguinte link: 

http://localhost:3000/users

Depois va na aba `auth`, e depois `bearer`, no campo de texto cole o token gerado no login,

Aqui você ira fazer a autenticação do seu usuario, com isso você tera uma lista de todos os usuarios cadastrados no seu banco de dados.
