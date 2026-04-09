# Desafio Técnico - Gerenciador de Tarefas

Aplicação web simples para cadastro e gerenciamento de tarefas, construída com Angular, ASP.NET Core Web API e SQL Server.

## Tecnologias Utilizadas
- **Front-end:** Angular 17+
- **Back-end:** ASP.NET Core Web API (C# / .NET 8)
- **Banco de Dados:** SQL Server
- **ORM:** Entity Framework Core

## Pré-requisitos
- .NET 8 SDK
- Node.js e Angular CLI
- SQL Server Express

## Como rodar o projeto

### 1. Configurando o Back-end (API)
1. Navegue até a pasta da API: `cd TarefasApi`
2. Configure a string de conexão no `appsettings.json` para o seu SQL Server local.
3. Restaure as dependências e rode as migrations:
   ```bash
   dotnet restore
   dotnet ef database update
   ```
4. Inicie o servidor: dotnet run (A API rodará na porta especificada no console, ex: http://localhost:5000).

### 2. Configurando o Front-end (Angular)

1. Navegue até a pasta do client: cd tarefas-app

2. Instale as dependências: npm install

3. Verifique o arquivo src/app/services/tarefa.service.ts para garantir que a variável apiUrl corresponde à porta que a sua API .NET está rodando.

4. Inicie a aplicação Angular: ng serve -o


### Funcionalidades

[x] CRUD Completo de Tarefas.

[x] Validação simples de campos obrigatórios.

[x] Mensagens de sucesso ao executar ações.

[x] Organização em Componentes e Services.

[x] Uso de HTTP Client (REST em JSON).