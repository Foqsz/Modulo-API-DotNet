# API de Agenda Telefônica

Esta API foi desenvolvida em .NET utilizando Entity Framework para fornecer um serviço de gerenciamento de contatos telefônicos. Com esta API, você pode realizar operações básicas de CRUD (Create, Read, Update, Delete) em contatos telefônicos.

## Recursos Principais

- **Gerenciamento de Contatos**: Adicione, visualize, atualize e remova contatos da agenda telefônica.
- **Pesquisa de Contatos**: Pesquise contatos por nome, número de telefone ou qualquer outra informação relevante.
- **Autenticação e Autorização**: Utilize autenticação para controlar o acesso aos recursos da API.
- **Segurança de Dados**: Proteja os dados dos contatos com medidas de segurança fornecidas pelo Entity Framework.

## Requisitos

- .NET Core SDK
- Microsoft SQL Server (ou outro banco de dados suportado pelo Entity Framework)

## Configuração

1. Clone o repositório para sua máquina local.
2. Abra o projeto no Microsoft Visual Studio.
3. Configure a conexão com o banco de dados no arquivo `appsettings.json`.
4. Execute as migrações do Entity Framework para criar o esquema do banco de dados:

```bash
dotnet ef database update
```

5. Inicie a aplicação.

## Endpoints
 
- **GET /api/contatos/{id}**: Retorna um contato específico pelo ID.
- **GET /api/contatos/{ObterPorNome}**: Retorna um contato específico pelo Name.
- **POST /api/contato**: Adiciona um novo contato à agenda.
- **PUT /api/contatos/{id}**: Atualiza as informações de um contato existente.
- **DELETE /api/contatos/{id}**: Remove um contato da agenda.

## Exemplos de Uso

### Adicionar um Contato

```http
POST /api/contatos
Content-Type: application/json

{
    "id": 4,
    "name": "Vez",
    "telefone": "233",
    "ativo": true
}
```

### Atualizar um Contato Existente

```http
PUT /api/contatos/1
Content-Type: application/json

{
    "id": 4,
    "name": "Vez",
    "telefone": "233",
    "ativo": true
}
```

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir problemas (issues) e enviar pull requests para melhorar esta API de agenda telefônica.

## Contato

- LinkedIn: [Victor Vinicius](https://www.linkedin.com/in/victor-vinicius-2a9166255/)
- Email: contatovictorvinicius05@gmail.com

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
 
