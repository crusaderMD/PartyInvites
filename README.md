# PartyInvites

## Sobre o projeto
O **PartyInvites** é uma aplicação web desenvolvida com **ASP.NET Core MVC**, que permite aos usuários confirmarem presença em um evento. Os convidados podem preencher um formulário de RSVP, e suas respostas são armazenadas temporariamente em um repositório em memória.

## Tecnologias Utilizadas
- **ASP.NET Core MVC**
- **C#**
- **Entity Framework Core** (caso queira adicionar persistência no banco de dados no futuro)
- **Bootstrap** (para estilização)
- **jQuery Validation** (para validação de formulários no frontend)

## Funcionalidades
- Formulário de RSVP para confirmação de presença.
- Validação de dados do formulário.
- Exibição de mensagem de agradecimento após a submissão.
- Lista de convidados que confirmaram presença.

## Estrutura do Projeto
```
PartyInvites/
│-- Controllers/
│   ├── HomeController.cs
│-- Models/
│   ├── GuestResponse.cs
│   ├── Repository.cs
│-- Views/
│   ├── Home/
│   │   ├── Index.cshtml
│   │   ├── RsvpForm.cshtml
│   │   ├── ListResponses.cshtml
│   ├── Shared/
│   │   ├── _Layout.cshtml
│   │   ├── _ValidationScriptsPartial.cshtml
│   ├── Thanks.cshtml
│   ├── Error.cshtml
│-- wwwroot/
│   ├── css/
│   ├── js/
│-- appsettings.json
│-- Program.cs
```

## Como Executar o Projeto
### 1. Clonar o Repositório
```sh
git clone https://github.com/seu-usuario/PartyInvites.git
cd PartyInvites
```

### 2. Restaurar Dependências
```sh
dotnet restore
```

### 3. Executar o Projeto
```sh
dotnet run
```
O projeto será iniciado e estará acessível em `http://localhost:5000` ou na porta configurada.

## Melhorias Futuras
- Armazenamento das respostas em um banco de dados SQL.
- Autenticação para administrador visualizar os convidados.
- Integração com APIs para envio de e-mails de confirmação.

---
Feito com ♥ por Luiz R. Bortolotti Jr. usando **ASP.NET Core MVC**!

