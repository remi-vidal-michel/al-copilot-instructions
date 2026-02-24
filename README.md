# AL Agent features

AL Agent is a specialized agent designed for Microsoft Dynamics 365 Business Central (AL) development.
It generates, reviews, refactors, and optimizes AL code while enforcing strict architectural boundaries, SQL-aware performance practices, and high code quality standards.

The agent  enforces a clear separation of concerns between Tables, Codeunits, and Pages. It systematically prevents architectural drift such as UI logic inside processes or business rules inside pages.

From a performance standpoint, the agent assumes a SQL-first mindset. It minimizes database roundtrips and avoids inefficient record access patterns.

Regarding code quality, the agent enforces single-responsibility procedures, guard clauses (early exits), XML documentation on public procedures, consistent naming conventions, proper Enum usage instead of Option fields, strict foreign key integrity via TableRelation, and disciplined error/message handling through labels.

# How to Use with GitHub Copilot in VS Code

1. Place the agent configuration file in your repository (.github/agents/al.agent.md).
2. Open Copilot Chat and select the AL Agent.