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
    public string Name => "Nikola Perisic";
    public string Role => "Full Stack Engineer at Vega IT";
    public string[] Industries => ["Pharma", "Construction", "Banking"];

    public Stack Backend  => new(".NET 8/10", "ASP.NET Core", "EF Core", "Redis");
    public Stack Frontend => new("React", "Next.js", "TypeScript", "TanStack Query", "Storybook");
    public Stack Security => new("OAuth 2.0 / OIDC", "Entra ID", "Keycloak", "Key Vault");
    public Stack Delivery => new("Azure", "Docker", "Azure DevOps", "xUnit", "Vitest");

    // I own features end to end, not just the code.
    public async Task<Release> DeliverAsync(Requirement requirement)
    {
        var solution = Design(requirement);
        await BuildAsync(solution);
        await TestAsync(solution);          // unit, integration, CI gates
        return await DeployAsync(solution); // CI/CD → production
    }
}
```

## Selected impact

| Result | What I did |
|:--|:--|
| **776 → 38 ms** | Traced a production outage to an EF Core Cartesian explosion; covering indexes cut the query by 95% |
| **11.5 → 2.3 min** | Azure DevOps pipeline, 80% faster with parallel jobs and caching |
| **−60% time, +35% completion** | Regulated digital identity verification flow for a banking platform |
| **8 modules, 0 downtime** | Legacy to React 18 micro-frontends, plus a 27-component Storybook UI library now shared org-wide |

## Projects

<details>
<summary><b>Microservices .NET Bank System</b> · .NET 8 reference architecture with gRPC, RabbitMQ and full observability · <i>open source</i></summary>

<br/>

Customers, accounts and transactions as independent services, wired together synchronously and asynchronously.

- **Sync:** gRPC (Account verifies that a customer exists). **Async:** RabbitMQ via MassTransit, every deposit or withdrawal publishes an event stored by the Transaction service in MongoDB
- **Clean Architecture + CQRS** (MediatR, FluentValidation) with layering rules enforced by architecture tests (NetArchTest)
- **Ocelot API gateway** with caching and rate limiting; Serilog + Elasticsearch + Kibana; Health Checks UI
- **CI on every PR:** build, formatting check, tests

**Stack:** .NET 8, ASP.NET Core, EF Core, PostgreSQL, MongoDB, gRPC, RabbitMQ, MassTransit, Ocelot, Docker Compose

[View repository →](https://github.com/perisicnikola37/microservices-dotnet-bank-system)

</details>

<details>
<summary><b>Scalable ASP.NET Core platform for 5,000+ concurrent users</b> · 94% faster load · UK client campaign · <i>Aug – Sep 2024</i></summary>

<br/>

Full stack for a flagship conference campaign (Unity WebGL front end, custom ASP.NET Core backend), played by 5,000+ users at once during a live public presentation.

- Load time cut from **20+ s to 1.2 s (~94%)** by caching large WebAssembly assets with service workers
- C#/.NET REST API for a real-time scoreboard and points system, tuned for 5,000+ concurrent players
- Cache invalidation automated in CI/CD (old service worker unregistered and cache cleared on every build)
- SEO-friendly Razor Pages (SSR), Web Workers for non-blocking performance, cross-browser fixes

**Stack:** C#, .NET, ASP.NET Core, Razor Pages, WebGL, WebAssembly, Service Workers, Web Workers, CI/CD

[Read the write-up →](https://medium.com/@perisicnikola37/how-i-optimized-slow-loading-time-using-service-workers-in-frontend-79d0ca013394)

</details>

<details>
<summary><b>Zero-downtime migration of a nonprofit's legacy platform</b> · WordPress → modern web architecture · <i>Mar 2024 – Nov 2025</i></summary>

<br/>

Owned the data migration and contributed full stack features while moving the platform off legacy WordPress with zero downtime.

- Migrated **1,071 locations, 3,783 gallery images and 206 accessibility tags** into a normalized relational database (9 SQL scripts + seeders), re-syncing as the dataset nearly doubled (579 → 1,071)
- Built core Next.js features: document management, dynamic Google Maps accessibility legends, advanced admin filters
- Containerized with Docker and Nginx, set up Prometheus monitoring, worked with automated CI/CD
- Reviewed pull requests across the team to keep architecture and standards consistent

**Stack:** Next.js, Spring Boot, Nginx, Docker, CI/CD, Prometheus, GA4, Google Maps API

</details>

## Featured writing

<p>
  <img src="https://img.shields.io/badge/READERS-220K%2B-0ea5e9?style=for-the-badge" alt="220K+ readers" />
  <img src="https://img.shields.io/badge/COMMUNITY-19K%2B%20ENGINEERS-0ea5e9?style=for-the-badge" alt="19K+ engineers" />
  <img src="https://img.shields.io/badge/MEDIUM%20FOLLOWERS-1.1K-000000?style=for-the-badge&logo=medium&logoColor=white" alt="1.1K Medium followers" />
</p>

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://medium.com/@perisicnikola37/dont-use-react-imports-like-this-use-wrapper-pattern-instead-b7a49b864ff4"><img src="https://miro.medium.com/v2/resize:fill:320:214/1*eVAb-mlDjE9hqrndSgD8eg.png" width="100%" alt="Wrapper Pattern article" /></a>
      <br/><br/>
      <b><a href="https://medium.com/@perisicnikola37/dont-use-react-imports-like-this-use-wrapper-pattern-instead-b7a49b864ff4">Don't use React imports like this. Use Wrapper Pattern instead</a></b><br/>
      An inefficient import strategy from a real project, and the right way to do it.<br/>
      <sub>📌 Pinned · Feb 21, 2025 · 62 responses</sub>
    </td>
    <td width="50%" valign="top">
      <a href="https://medium.com/@perisicnikola37/dont-use-typescript-types-like-this-use-map-pattern-instead-bed75a0e986e"><img src="https://miro.medium.com/v2/resize:fill:320:214/0*dLiPy0pJrbsowuuH.png" width="100%" alt="Map Pattern article" /></a>
      <br/><br/>
      <b><a href="https://medium.com/@perisicnikola37/dont-use-typescript-types-like-this-use-map-pattern-instead-bed75a0e986e">Don't use TypeScript types like this. Use Map Pattern instead</a></b><br/>
      Replacing rigid types with a more dynamic Map-based design.<br/>
      <sub>📌 Pinned · Feb 17, 2025 · 25 responses</sub>
    </td>
  </tr>
</table>

<p align="center">
  <a href="https://medium.com/@perisicnikola37">All articles on Medium →</a> · <a href="https://dev.to/perisicnikola37">DEV Community →</a>
</p>

---

<p align="center">
  Open to conversations about enterprise web platforms and remote collaboration with UK and international teams.<br/>
  <a href="mailto:nikola@perisic.digital">nikola@perisic.digital</a> · <a href="https://perisic.digital">perisic.digital</a>
</p>
