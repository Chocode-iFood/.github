# Desafio iLab - Ifood
<br />

O programa iLab tem como objetivo construir o futuro no curto prazo da área de Tecnologia e Data do iFood acelerando pessoas com perfil Junior para atuarem plenamente como um Foodlover.
Os Foodlovers do programa iLab foram organizados em grupos para realizar um desafio que consiste na criação de uma aplicação de telemetria.
<br />

## 🚀 Sobre o Desafio
<br />

**Track History - Telemetria dos entregadores do Ifood**

Neste projeto deve-se manter todo o histórico de telemetria de um entregador para um determinado pedido. A telemetria é encerrada quando há um evento de conclusão ou cancelamento (por parte do entregador).
<br />

## 💻 Desenvolvedores do Grupo Chocode
<br />

- [Claudia Nogueira dos Anjos](https://github.com/AnjosClaudia)
- [Daniel Silveira](https://github.com/smarticogit)
- [Raphaela Leite](https://github.com/Raphaella-leite)
- [Silvano Araújo](https://github.com/Silvanoeng)
- [Vitor Eleuterio](https://github.com/SevenSecRS)

### ✒️ Metodologia

Para priorizar a produtividade e a organização das entregas utilizamos a metodologia Kanban no Github.

[Acesso ao Kanban do grupo](https://github.com/orgs/Chocode-iFood/projects/1)
<br />

## 📋 Projeto
<br />

O projeto foi desenvolvido utilizando as seguintes tecnologias:
<br />

##### 🛠 [Back End](https://github.com/Chocode-iFood/back): Java, Spring Boot, JWT
 
##### 🛠 [Front End](https://github.com/Chocode-iFood/front): HTML, CSS, JavaScript
<br />

## 💻 Front End
<br />

A composição das telas segue a seguinte estrutura:
<br />

- Autenticação do entregador

[Colocar]
<br />
- Consulta de pedidos

[Colocar]
<br />
- Atribuição de pedido pelo entregador

[Colocar]
<br />
- Alteração de status do pedido (cancelado/concluído)

[Colocar]
<br />

## 💻 Back End
<br />
Iniciamos com a importação de dependências necessárias pelo [Spring Initializr](https://start.spring.io/), conforme segue abaixo:
- Spring Initializr 
- Maven Project
- Spring Boot 2.6.4
- Packaging Jar 
- Java 17
<br />

**Dependências:** 
- Spring Web, MySQL Driver
- Spring Data JPA
- Spring Boot DevTools
- Lombok
- Spring Security
- H2 Database
- MySQL Driver
- PostgreSQL Driver
- Dependências do JWT sinalizado no arquivo pom.xml
<br />

### ⚙️ Modelagem do Banco de Dados
<br />

Realizamos a modelagem do banco de dados em consonância com a descrição do desafio.
Utilizamos o banco relacional H2 e MySQL para os testes iniciais e posteriormente o Postgres. As configurações estão nos arquivos properties.
<br />

<img height="380" src="https://github.com/Chocode-iFood/dados-complementares/blob/main/Diagrama.png?raw=true">

<br />

## 📦 Estrutura dos Pacotes
<br />
A estrutura dos pacotes, com as classes e interfaces, está descrita a seguir:
<br />
📦 Model
<br />
📦 DAO → JpaRepository
<br />
📦 DTO
<br />
📦 Services 
<br />
📦 Security → JWT
<br />
📦 Controller 
<br />

### 🖇 Endpoints do desafio: 
<br />

- Endpoint para receber geolocalização do entregador

	*POST “/geolocalizacao”*

- Endpoint para alteração dos status dos pedidos
	
	*PUT “/pedidos/{id}/status”* 

- Endpoint para consulta de pedidos 
	
	*GET “/pedido/listar”* 

- Endpoint para consultas de geolocalização por pedido 
	
	*GET “/pedidos/{id}/geolocalizacao”* 

- Endpoint para atribuição do entregador para o pedido
	
	*POST “/pedidos/{id_pedido}/entregador/{id_entregador}”*

- Endpoint para Autenticação de entregador 
         
	 *POST “/entregador/login”*
<br />


## 📋 Agradecimentos
<br />
Agradecemos a Ifood, Foodlover Danilo De Luca, professor Danilo da Gama Academy e todos que também contribuíram para o desenvolvimento do projeto.

