# Claude Code Skills

[![Skills](https://img.shields.io/badge/skills-67-5267DF?style=flat-square)](#skills-catalog)
[![Reference guides](https://img.shields.io/badge/reference%20guides-371-0F766E?style=flat-square)](#repository-layout)
[![License: MIT](https://img.shields.io/badge/license-MIT-2E7D32?style=flat-square)](./LICENSE)

A practical library of **67 Claude Code skills** for full-stack software engineering, with **371 focused reference guides**. The collection covers programming languages, frameworks, architecture, testing, security, infrastructure, data, and more.

Each skill is a self-contained `SKILL.md` with supporting references. Install the skills you need, or install the entire collection for automatic activation in Claude Code.

## Install the skills

Clone the repository and copy all skill folders into your user-level Claude Code skills directory:

```bash
git clone https://github.com/ecr17dev/claude-code-skills.git /tmp/claude-code-skills
mkdir -p "$HOME/.claude/skills"

for skill_dir in /tmp/claude-code-skills/*; do
  [ -d "$skill_dir" ] || continue
  [ -f "$skill_dir/SKILL.md" ] || continue
  cp -R "$skill_dir" "$HOME/.claude/skills/"
done
```

To install a single skill, copy only its folder. For example:

```bash
cp -R /tmp/claude-code-skills/python-pro "$HOME/.claude/skills/"
```

For project-specific skills, use the project's `.claude/skills/` directory instead of `$HOME/.claude/skills/`. Restart or reopen Claude Code after installation if a newly added skill is not immediately available.

## Skills catalog

| Area | Skills |
| --- | --- |
| **Languages** | [C++ Pro](./cpp-pro/SKILL.md) · [C# Developer](./csharp-developer/SKILL.md) · [Go Pro](./golang-pro/SKILL.md) · [Java Architect](./java-architect/SKILL.md) · [JavaScript Pro](./javascript-pro/SKILL.md) · [Kotlin Specialist](./kotlin-specialist/SKILL.md) · [PHP Pro](./php-pro/SKILL.md) · [Python Pro](./python-pro/SKILL.md) · [Rust Engineer](./rust-engineer/SKILL.md) · [SQL Pro](./sql-pro/SKILL.md) · [Swift Expert](./swift-expert/SKILL.md) · [TypeScript Pro](./typescript-pro/SKILL.md) |
| **Backend frameworks** | [Django Expert](./django-expert/SKILL.md) · [Django Storages S3](./django-storages-s3/SKILL.md) · [FastAPI Expert](./fastapi-expert/SKILL.md) · [Laravel Specialist](./laravel-specialist/SKILL.md) · [NestJS Expert](./nestjs-expert/SKILL.md) · [Rails Expert](./rails-expert/SKILL.md) · [.NET Core Expert](./dotnet-core-expert/SKILL.md) · [Spring Boot Engineer](./spring-boot-engineer/SKILL.md) |
| **Frontend and mobile** | [Angular Architect](./angular-architect/SKILL.md) · [Flutter Expert](./flutter-expert/SKILL.md) · [Next.js Developer](./nextjs-developer/SKILL.md) · [React Expert](./react-expert/SKILL.md) · [React Native Expert](./react-native-expert/SKILL.md) · [Vue Expert](./vue-expert/SKILL.md) · [Vue Expert JS](./vue-expert-js/SKILL.md) |
| **Infrastructure and databases** | [Cloud Architect](./cloud-architect/SKILL.md) · [Database Optimizer](./database-optimizer/SKILL.md) · [Kubernetes Specialist](./kubernetes-specialist/SKILL.md) · [Postgres Pro](./postgres-pro/SKILL.md) · [Terraform Engineer](./terraform-engineer/SKILL.md) |
| **APIs and architecture** | [API Designer](./api-designer/SKILL.md) · [Architecture Designer](./architecture-designer/SKILL.md) · [GraphQL Architect](./graphql-architect/SKILL.md) · [MCP Developer](./mcp-developer/SKILL.md) · [Microservices Architect](./microservices-architect/SKILL.md) · [WebSocket Engineer](./websocket-engineer/SKILL.md) |
| **Quality and testing** | [Code Documenter](./code-documenter/SKILL.md) · [Code Reviewer](./code-reviewer/SKILL.md) · [Playwright Expert](./playwright-expert/SKILL.md) · [Test Master](./test-master/SKILL.md) |
| **DevOps and operations** | [Chaos Engineer](./chaos-engineer/SKILL.md) · [CLI Developer](./cli-developer/SKILL.md) · [DevOps Engineer](./devops-engineer/SKILL.md) · [Monitoring Expert](./monitoring-expert/SKILL.md) · [SRE Engineer](./sre-engineer/SKILL.md) |
| **Security** | [Secure Code Guardian](./secure-code-guardian/SKILL.md) · [Security Reviewer](./security-reviewer/SKILL.md) |
| **Data and machine learning** | [Fine-Tuning Expert](./fine-tuning-expert/SKILL.md) · [ML Pipeline](./ml-pipeline/SKILL.md) · [Pandas Pro](./pandas-pro/SKILL.md) · [Prompt Engineer](./prompt-engineer/SKILL.md) · [RAG Architect](./rag-architect/SKILL.md) · [Spark Engineer](./spark-engineer/SKILL.md) |
| **Platforms** | [Atlassian MCP](./atlassian-mcp/SKILL.md) · [Salesforce Developer](./salesforce-developer/SKILL.md) · [Shopify Expert](./shopify-expert/SKILL.md) · [WordPress Pro](./wordpress-pro/SKILL.md) |
| **Specialized domains** | [Embedded Systems](./embedded-systems/SKILL.md) · [Game Developer](./game-developer/SKILL.md) · [Legacy Modernizer](./legacy-modernizer/SKILL.md) |
| **Workflow and reasoning** | [Debugging Wizard](./debugging-wizard/SKILL.md) · [Feature Forge](./feature-forge/SKILL.md) · [Fullstack Guardian](./fullstack-guardian/SKILL.md) · [Spec Miner](./spec-miner/SKILL.md) · [The Fool](./the-fool/SKILL.md) |

## Repository layout

Every skill has its own directory and entry point:

```text
skill-name/
├── SKILL.md
└── references/
    └── topic-specific-guidance.md
```

The skill file describes its purpose and activation cues. Reference guides provide deeper, topic-specific instructions that can be loaded when needed.

## Contributing

Contributions are welcome. Keep each skill focused, preserve its `SKILL.md` entry point, and place detailed supporting material in that skill's `references/` directory. Include links to upstream sources when adapting existing material, and retain applicable copyright notices and license terms.

## Attribution and license

The skill collection is redistributed from [Jeff Allan's Claude Skills project](https://github.com/jeffallan/claude-skills) under the MIT License. Original skill metadata and the upstream license are preserved. See [NOTICE.md](./NOTICE.md) for provenance details and [LICENSE](./LICENSE) for the full license text.

This repository is maintained by [ecr17dev](https://github.com/ecr17dev) as a convenient distribution of the skills; it does not claim authorship of the upstream skill content.
