![Aurora Project](https://repository-images.githubusercontent.com/128673011/f6ebdd80-b6da-11ea-94bb-9d141944b257)

# O que é o projeto Aurora?
É um projeto de código aberto, escrito em .NET Core, atualmente na versão 3.1. O objetivo do projeto é mostrar que é possível criar uma arquitetura mais simples que as outras e utilizando alguns conceitos como DDD (Design Driven Design).

## Proposta de negócio:
Este projeto é uma gestão simples de EPI (Equipamentos de Proteção Individual). A ideia principal é cadastrar trabalhadores e EPIs e, com esses dados, permitir a transferência de EPIs para um trabalhador. Além disso, este sistema permite que você veja todos os EPIs e quem tem um EPI e avise se o EPI está prestes a expirar.

### Abreviações:
* NIN: Número do Seguro Nacional (como CPF no Brasil)

## Como usar:
1. Clone este projeto em sua maquina 
2. Use a String de conexão padrão ou:
    2.1.  Instale e configure [MySql] (https://dev.mysql.com/downloads/mysql/), se desejar.
    2.2. Informe a string de conexão em Aroura.Infra.Data/Context/MySqlContext.cs, se necessário
    * Coloque o nome do servidor na tag [SERVER]
    * Coloque o numero da porta na tag [PORT]
    * Coloque o nome de usuário do banco de dados na teg [USER]
    * Coloque a senha do banco de dados na tag [PASSWORD]
3. Finalmente, construa e execute sua aplicação

## Migração MySQL:
1. Abra o console do gerenciador de pacotes
2. Altere o projeto padrão para Aurora.Infra.Data
3. Execute o comando "Add-Migration [NAME OF YOUR MIGRATION]"
4. Execute o comando "Update-Database"

Para mais informações sobre este projeto, consulte este [artigo] (https://medium.com/@alexalves_85598/criando-uma-api-em-net-core-baseado-na-arquitetura-ddd-2c6a409c686).

## Tecnologias implementadas:
* ASP.NET Core 3.1 (com .NET Core 3.1)
* Entity Framework Core 3.1.5
* Flunt Validation 1.0.5
* Swagger UI 5.5.0
* MySql Database Connection
* .NET Core Native DI
* SpecFlow for BDD
* GitHub Actions

## Arquitetura:
* Layer architecture
* S.O.L.I.D. principles
* Clean Code
* Domain Validations
* Domain Notifications
* Domain Driven Design
* Repository Pattern
* Notification Pattern
* Mapper by Extension Methods
* Value Types
* BDD (Behavior Driven Development)

![miro](C:\Users\vkada\Desktop\miro.png)

## News:
**v1.4 --- 2020-09-28**
* CI/CD by GitHub Actions
* Include integration tests using BDD with SpecFlow
    * scenario of register a worker
    * scenario of update a worker
* Bug corrections

**v1.3 --- 2020-07-30**
* Changed some Primitive Types to Value Types
* Changed the business idea principle

**v1.2 --- 2020-06-30**
* Implemented Notification Pattern
* Implemented Domain Validations and Notifications
* Using some concepts of Clean Architecture
    * Entities
    * Interface Adapters
* Changed the framework validations to Flunt
* Using mapper by extension methods

**v1.1 --- 2020-06-24**
* Updated the project name
* Updated the project's SDK to .NET Core 3.1 version
* Added the Swagger framework to document the API
* Corrections to end-points
* Published in [Azure](http://aurora-project.azurewebsites.net/swagger/index.html)

**v1.0 --- 2018-06-09**
* Create the project in .NET Core 2.0 version
* Structured the project on layer architecture 
* Used the Service layer to business rules
* Used the FluentValidation library
* Configured the connection to MySql database
* Used EntityFramework

## Por que Aurora?
O nome Aurora veio do evento natural chamado Aurora Borealis. É um evento científico descrito pela interação entre a camada magnética da Terra e as partículas energizadas do vento solar.

Uma curiosidade sobre tal evento é que o que vemos nas fotos nem sempre é a mesma imagem que vemos ao vivo.

Para obter mais informações, consulte este [link] (https://www.hipercultura.com/fenomenos-naturais/).

## Estamos online!
Veja o projeto em [Azure](http://aurora-project.azurewebsites.net/swagger/index.html).

## Sobre:
O projeto Aurora foi desenvolvido por [Alex Alves](https://www.linkedin.com/in/alexalvess/).

