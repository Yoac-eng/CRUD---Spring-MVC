<h1 align="center">CRUD - Spring - Thymeleaf</h1>

<h3>Descrição do projeto</h3>
Primeiros passos utilizando Spring MVC e thymeleaf - CRUD;<br>
Projeto apresentado na matéria de POO, na UEMA;

<h3>Configuração do projeto</h3>
Criar novo schema, schema name: regescweb, character set: utf8<br>
SQL Script: CREATE SCHEMA `regescweb` DEFAULT CHARACTER SET utf8;<br>
<br>
No projeto: regescweb/src/main/java/resources/application.properties<br>
Editar as linhas com os respectivos dados do usuário:<br>
spring.datasource.username=UsuarioDoBanco<br>
spring.datasource.password=SenhaDoBanco<br>

Feito isso, basta rodar o projeto pela IDE, que as entidades serão feitas via Spring Data e
o projeto será inicializado pelo tomcat, podendo ser acessado pelo localhost na porta 8080
localhost:8080

*Caso queira colocar algum dado para testar as funcionalidades diretamente, rode as seguintes queries
no banco:<br>
INSERT INTO `regescweb`.`professor`(`nome`, `salario`, `status_professor`) VALUES ('Professor1', '5000.0', 'ATIVO');<br>
INSERT INTO `regescweb`.`professor`(`nome`, `salario`, `status_professor`) VALUES ('Professor2', '10000.0', 'APOSENTADO');<br>

<h3>Utilizando</h3>
URLs para acesso das páginas: localhost:8080/professores || Read<br>
localhost:8080/professores/new || Create<br>
