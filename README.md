# What is Aurora project?
It's an open source project, written in .NET Core, currently in version 3.1.

The project's goals is to show that is possible to create an architecture more simple than others and using some concepts like DDD (Design Driven Design).

## Business proposal:
This project is a simple PPE (Personal Protective Equipament) Management. The principle idea is to register workers and PPE and, with this data, allow to transfer PPE to a worker.
Besides that, this system allow that you see all PPE and who has a PPE and notify if the PPE is near to expire.

### Abbreviations:
* NIN: National Insurance Number (as CPF in Brazil)

## How to use:
1. Clone this project to into your machine
2. Use the default connection string or:
    2.1. Install and configure [MySql](https://dev.mysql.com/downloads/mysql/), if you want.
    2.2. Inform the connection string on Aroura.Infra.Data/Context/MySqlContext.cs, if necessary
    * Put the server name on [SERVER] tag
    * Put the port number on [PORT] tag
    * Put the user name database on [USER] tag
    * Put the password database on [PASSWORD] tag
4. Finally, build and run the application

## MySql Migrations:
1. Open your Package Manager Console
2. Change the default project to Aurora.Infra.Data
3. Run command "Add-Migration [NAME OF YOUR MIGRATION]"
4. Run command "Update-Database"

For more information about this project, sse this [article](https://medium.com/@alexalves_85598/criando-uma-api-em-net-core-baseado-na-arquitetura-ddd-2c6a409c686).

## Technologies implemented:
* ASP.NET Core 3.1 (com .NET Core 3.1)
* Entity Framework Core 3.1.5
* Flunt Validation 1.0.5
* Swagger UI 5.5.0
* MySql Database Connection
* .NET Core Native DI
* SpecFlow for BDD
* GitHub Actions

## Architecture:
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

![Architecture](https://miro.medium.com/max/962/1*qpHCIA7RDfW89KtSUXGJog.png)

