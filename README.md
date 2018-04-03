
#Teste para candidatos à vaga de desenvolvedor FullStack

##Objetivo
Desenvolver uma aplicação que administre candidatos.

## Pre-requisitos
* Git
* NodeJS
* NPM/Yarn
* MongoDB

 
##Instruções
* Desenvolva a aplicação utilizando as tecnologias: ReactJs, NodeJS, Express e MongoDB.
* Após terminar seu teste submeta o projeto em um repositório no Github para guilherme@bartdigital.com.br.
 
##Especificações técnicas

1. Utilizar componentes http://materializecss.com/

2. A aplicação deve conter as seguintes telas:
	*	2.1 **Tela de cadastro de candidato**. 
		* 2.1.1 O formulário deve conter os campos de acordo com a tabela abaixo:
		
		 _| nome | cpf | telefone | endereco | sexo | idade | termoResponsabilidade
		--- | --- | --- | --- | --- | --- | --- | ---
		Type | Text | Number | Number | Text | Radio | Number | Checkbox
		Required | true | true | true | false | true | false | false

		* 2.1.2 Os campos de formulário devem possuir **validação** de **preenchimento** e **tipos de valores**.

		* 2.1.3 Os dados do preenchimento do formulário devem ser enviados para o serviço adequado.

		* 2.1.4 Os campos do formulário **não pode possuir** como **model** os valores da tabela **x.x.x**, logo deve-se realizar uma normalização dos dados antes de envia-los para o serviço.
	* 2.2 **Tela com as informações do candidato.**
		* 2.2.1 A tela deve possuir um botão de atualizar os dados, utilizando o protocolo **PUT**.
	* 2.3 **Tela com a listagem dos candidatos cadastrado**.
		* 2.3.1 A listagem dos candidatos deve listar apenas os candidatos que possuírem o registro **termoResponsabilidade** selecionado como **TRUE**.
		* 2.3.2 O candidato listado deve ser um link para acessar a página(view/route) com as informações daquele candidato.
* O serviço/back-end deve possuir uma rota para realizar as operações dos candidatos. 
* O serviço/back-end(NodeJS) deve expor uma API no modelo RESTful para ser utilizado no ReactJS e e possuir os métodos de **get**, **post**, **put** e **delete**.
* O banco de dados(MongoDB) deve possuir uma **Colleciton**(Tabela) de acordo com o modelo abaixo:
		
		 _| nome | cpf | telefone | endereco | sexo | idade | termoResponsabilidade
		--- | --- | --- | --- | --- | --- | --- | ---
		Type | String | Number | Number | String | String | Number | Boolean
		Required | true | true | true | false | true | false | false
		
* Os erros do serviço/back-end(NodeJS) devem ser tratados e enviados no modelo de **Status HTTP** para o ReactJS.
* O serviço/back-end(NodeJS) deve realizar uma **validação** no cadastro de candidato, para **permitir apenas um cadastro** por **CPF**.

##Pontos extras
- Seguir as boas práticas com ReactJS e NodeJS.
- Desenvolver HTML semântico.
- Componentizar elementos reutilizáveis.
- Utilizar testes automatizados. Framework livre a sua escolha.
- Implementar autenticação com JWT.
- Gerar a documentação da aplicação desenvolvida.



