## Endpoints

Assim como a documentação do JSON-Server-Auth traz (https://www.npmjs.com/package/json-server-auth), existem 3 endpoints que podem ser utilizados para cadastro e 2 endpoints que podem ser usados para login.

### Cadastro
--------------------------------------------------------------------------
POST /register - Registrar um novo usuário <br/>

Formato de Envio <br/>

{
	"email": "teste@teste.com",
	"password": "123456",
	"name": "Teste",
	"age": 26
}


--------------------------------------------------------------------------
POST /techs - Postar tecnologias do usuário (REQUIRED BEARER TOKEN) <br/>

Formato de Envio <br/>

{
	userId: "id do usuário",
	title: "tecnologia",
	nivel: "nivel"
}


Você pode ficar a vontade para adicionar qualquer outra propriedade no corpo do cadastro dos usuários.


### Techs

GET /techs - Obter todas as tecnologias criadas<br/>

--------------------------------------------------------------------------<br/>

### Login

--------------------------------------------------------------------------<br/>
POST /login ou POST /signin - Fazer login com conta de usuário (REQUIRED EMAIL AND PASSWORD) <br/>

Formato de Envio <br/>

{
	email: "email",
	password: "password"
}
--------------------------------------------------------------------------<br/>
