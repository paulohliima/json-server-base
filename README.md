## Endpoints

Assim como a documentação do JSON-Server-Auth traz (https://www.npmjs.com/package/json-server-auth), existem 3 endpoints que podem ser utilizados para cadastro e 2 endpoints que podem ser usados para login.

### Cadastro
--------------------------------------------------------------------------
POST /register - Registrar um novo usuário <br/>

Formato de Envio <br/>

{<br/>
	"email": "teste@teste.com",<br/>
	"password": "123456",<br/>
	"name": "Teste",<br/>
	"age": 26<br/>
}<br/>


--------------------------------------------------------------------------
POST /techs - Postar tecnologias do usuário (REQUIRED BEARER TOKEN) <br/>

Formato de Envio <br/>

{<br/>
	userId: "id do usuário",<br/>
	title: "tecnologia",<br/>
	nivel: "nivel"<br/>
}<br/>


Você pode ficar a vontade para adicionar qualquer outra propriedade no corpo do cadastro dos usuários.


### Techs

GET /techs - Obter todas as tecnologias criadas<br/>

--------------------------------------------------------------------------<br/>

### Login

--------------------------------------------------------------------------<br/>
POST /login ou POST /signin - Fazer login com conta de usuário (REQUIRED EMAIL AND PASSWORD) <br/>

Formato de Envio <br/>

{<br/>
	email: "email",<br/>
	password: "password"<br/>
}<br/>
--------------------------------------------------------------------------<br/>
