
<body>

<h1>📌 To-Do API com .NET, DDD e Entity Framework</h1>

<p>
API de gerenciamento de tarefas (To-Do) desenvolvida em <strong>C# com .NET</strong>, utilizando 
<strong>Entity Framework Core</strong> e <strong>SQL Server</strong>, estruturada com base nos princípios de 
<strong>Domain-Driven Design (DDD)</strong>.
</p>

<p>
O objetivo deste projeto é aplicar boas práticas de arquitetura, organização de código e separação de responsabilidades.
</p>

<hr>

<h2>🧱 Arquitetura do Projeto</h2>

<pre>
src
 ┣ To_Do.API
 ┃ ┣ Controllers
 ┃ ┣ Program.cs
 ┃ ┗ appsettings.json
 ┣ To_Do.Application
 ┃ ┣ DTOs
 ┃ ┗ Services
 ┣ To_Do.Domain
 ┃ ┣ Entities
 ┃ ┣ Enums
 ┃ ┗ Interfaces
 ┣ To_Do.Infrastructure
 ┃ ┣ DataBase
 ┃ ┣ Migrations
 ┃ ┗ Repository
</pre>

<hr>

<h2>🔎 Descrição das Camadas</h2>

<h3>🔹 API (Presentation Layer)</h3>
<ul>
  <li>Controllers</li>
  <li>Configurações da aplicação</li>
  <li>Endpoints HTTP</li>
</ul>

<h3>🔹 Application</h3>
<ul>
  <li>DTOs (Data Transfer Objects)</li>
  <li>Services (regras de aplicação)</li>
  <li>Comunicação entre API e Domain</li>
</ul>

<h3>🔹 Domain</h3>
<ul>
  <li>Entidades</li>
  <li>Interfaces (contratos)</li>
  <li>Enums</li>
  <li>Regras de negócio</li>
</ul>

<h3>🔹 Infrastructure</h3>
<ul>
  <li>Acesso a dados com Entity Framework</li>
  <li>Repositórios</li>
  <li>Migrations</li>
  <li>Configuração do banco de dados</li>
</ul>

<hr>

<h2>🚀 Tecnologias utilizadas</h2>

<ul>
  <li>C#</li>
  <li>.NET</li>
  <li>ASP.NET Core Web API</li>
  <li>Entity Framework Core</li>
  <li>SQL Server</li>
  <li>LINQ</li>
</ul>

<hr>

<h2>⚙️ Funcionalidades</h2>

<ul>
  <li>✅ Criar tarefas</li>
  <li>📋 Listar tarefas</li>
  <li>✏️ Atualizar tarefas</li>
  <li>❌ Remover tarefas</li>
</ul>

<hr>

<h2>🛠️ Como executar o projeto</h2>

<h3>Pré-requisitos</h3>
<ul>
  <li>.NET SDK</li>
  <li>SQL Server</li>
  <li>Visual Studio ou VS Code</li>
</ul>

<h3>Passo a passo</h3>

<ol>
  <li>Clone o repositório:
    <pre><code>git clone https://github.com/Joao-V36/Task_List</code></pre>
  </li>

  <li>Acesse a pasta:
    <pre><code>cd seu-repositorio</code></pre>
  </li>

  <li>Configure a string de conexão no <code>appsettings.json</code>:
    <pre><code>{
  "ConnectionStrings": {
    "DefaultConnection": "Server=SEU_SERVIDOR;Database=ToDoDb;Trusted_Connection=True;"
  }
}</code></pre>
  </li>

  <li>Execute as migrations:
    <pre><code>dotnet ef database update --project To_Do.Infrastructure --startup-project To_Do.API</code></pre>
  </li>

  <li>Execute a aplicação:
    <pre><code>dotnet run --project To_Do.API</code></pre>
  </li>
</ol>

<hr>

<h2>📚 Conceitos aplicados</h2>

<ul>
  <li>Domain-Driven Design (DDD)</li>
  <li>Separação de responsabilidades (SoC)</li>
  <li>Inversão de dependência (DIP)</li>
  <li>Repository Pattern</li>
  <li>DTOs</li>
  <li>Migrations com Entity Framework</li>
</ul>

<hr>


<h2>📷 Exemplo de endpoints</h2>

<pre><code>
GET    /api/Tarefa
POST   /api/Tarefa
PUT    /api/Tarefa/{id}
DELETE /api/Tarefa/{id}
</code></pre>

<hr>

<h2>🤝 Contribuição</h2>

<p>Sinta-se à vontade para contribuir com melhorias ou sugestões!</p>

<hr>

<h2>📄 Licença</h2>

<p>Este projeto está sob a licença MIT.</p>

</body>
</html>
