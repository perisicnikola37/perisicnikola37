<p align="center">
  <img src="https://komarev.com/ghpvc/?username=perisicnikola37&label=profile%20views&color=0ea5e9&style=for-the-badge" alt="Profile views" />
</p>

<h1 align="center">Nikola Perisic</h1>

<p align="center">
  <b>I make enterprise systems faster, safer, and easier to ship.</b><br/>
  Full Stack Engineer · C#/.NET · React · TypeScript · Azure<br/>
  <sub>Remote · full overlap with UK business hours</sub>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/perisicnikola37/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://medium.com/@perisicnikola37"><img src="https://img.shields.io/badge/Medium-000000?style=flat-square&logo=medium&logoColor=white" alt="Medium" /></a>
  <a href="https://dev.to/perisicnikola37"><img src="https://img.shields.io/badge/DEV-0A0A0A?style=flat-square&logo=devdotto&logoColor=white" alt="DEV" /></a>
  <a href="mailto:nikola@perisic.digital"><img src="https://img.shields.io/badge/nikola@perisic.digital-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

```csharp
public sealed class Engineer : IFullStackEngineer
{
    public string Role     => "Full Stack Engineer at Vega IT";
    public string[] Industries => ["Pharma", "Construction", "Banking"];
    public Stack Backend   => new(".NET 8/10", "ASP.NET Core", "EF Core", "Redis");
    public Stack Frontend  => new("React", "Next.js", "TypeScript", "TanStack Query", "Storybook");
    public Stack Security  => new("OAuth 2.0 / OIDC", "Entra ID", "Keycloak", "Key Vault");
    public Stack Delivery  => new("Azure", "Docker", "Azure DevOps", "xUnit", "Vitest");

    // I own features end to end, not just the code.
    public async Task<Release> DeliverAsync(Requirement r) { /* design → build → test → deploy */ }
}
```

## Projects

<details>
<summary><b>Microservices .NET Bank System</b> · gRPC, RabbitMQ, full observability · <i>open source</i></summary>

<br/>

- **Sync:** gRPC. **Async:** RabbitMQ via MassTransit, events stored in MongoDB
- **Clean Architecture + CQRS** (MediatR, FluentValidation), layering enforced by architecture tests
- **Ocelot gateway** with caching and rate limiting; Serilog + Elasticsearch + Kibana
- **CI on every PR:** build, formatting check, tests

**Stack:** .NET 8, PostgreSQL, MongoDB, gRPC, RabbitMQ, Ocelot, Docker Compose · [Repository →](https://github.com/perisicnikola37/microservices-dotnet-bank-system)

</details>

<details>
<summary><b>Platform for 5,000+ concurrent users</b> · 94% faster load · <i>UK client, 2024</i></summary>

<br/>

- Load time cut from **20+ s to 1.2 s** by caching large WebAssembly assets with service workers
- Real-time scoreboard API (ASP.NET Core) tuned for 5,000+ concurrent players
- Cache invalidation automated in CI/CD; SSR Razor Pages, Web Workers

**Stack:** C#, ASP.NET Core, WebGL, WebAssembly, Service Workers · [Write-up →](https://medium.com/@perisicnikola37/how-i-optimized-slow-loading-time-using-service-workers-in-frontend-79d0ca013394)

</details>

<details>
<summary><b>Zero-downtime nonprofit migration</b> · WordPress → modern stack · <i>2024 – 2025</i></summary>

<br/>

- Migrated **1,071 locations, 3,783 images, 206 accessibility tags** into a normalized relational DB
- Built Next.js features: document management, Google Maps accessibility legends, admin filters
- Docker, Nginx, Prometheus, CI/CD; reviewed PRs across the team

**Stack:** Next.js, Spring Boot, Nginx, Docker, Prometheus, Google Maps API

</details>

## Writing

<p>
  <img src="https://img.shields.io/badge/READERS-220K%2B-0ea5e9?style=flat-square" alt="220K+ readers" />
  <img src="https://img.shields.io/badge/COMMUNITY-19K%2B%20ENGINEERS-0ea5e9?style=flat-square" alt="19K+ engineers" />
  <img src="https://img.shields.io/badge/MEDIUM-1.1K%20FOLLOWERS-000000?style=flat-square&logo=medium&logoColor=white" alt="1.1K Medium followers" />
</p>

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://medium.com/@perisicnikola37/dont-use-react-imports-like-this-use-wrapper-pattern-instead-b7a49b864ff4"><img src="https://miro.medium.com/v2/resize:fill:320:214/1*eVAb-mlDjE9hqrndSgD8eg.png" width="100%" alt="Wrapper Pattern article" /></a>
      <br/>
      <b><a href="https://medium.com/@perisicnikola37/dont-use-react-imports-like-this-use-wrapper-pattern-instead-b7a49b864ff4">React imports: use the Wrapper Pattern</a></b><br/>
      <sub>An inefficient import strategy from a real project, and the right way to do it.</sub><br/>
      <sub>📌 Pinned · Feb 2025 · 62 responses</sub>
    </td>
    <td width="50%" valign="top">
      <a href="https://medium.com/@perisicnikola37/dont-use-typescript-types-like-this-use-map-pattern-instead-bed75a0e986e"><img src="https://miro.medium.com/v2/resize:fill:320:214/0*dLiPy0pJrbsowuuH.png" width="100%" alt="Map Pattern article" /></a>
      <br/>
      <b><a href="https://medium.com/@perisicnikola37/dont-use-typescript-types-like-this-use-map-pattern-instead-bed75a0e986e">TypeScript types: use the Map Pattern</a></b><br/>
      <sub>Replacing rigid types with a more dynamic Map-based design.</sub><br/>
      <sub>📌 Pinned · Feb 2025 · 25 responses</sub>
    </td>
  </tr>
</table>

<p align="center">
  <a href="https://medium.com/@perisicnikola37">All articles on Medium →</a> · <a href="https://dev.to/perisicnikola37">DEV Community →</a>
</p>

---

<p align="center">
  Open to enterprise web platform work with UK and international teams<br/>
</p>
