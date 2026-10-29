<div align="center">

# Easy Starters

**Production-ready software foundations for web, API, mobile, extensions, services, and documentation.**

[![Website](https://img.shields.io/badge/website-live-6C63FF?logo=githubpages&logoColor=white)](https://fonijbuild.github.io/easy-starters/)
[![Browse Starters](https://img.shields.io/badge/browse-starters-0B1020)](#starters)
[![License: MIT](https://img.shields.io/badge/license-MIT-yellow.svg)](LICENSE)
![Spec Driven](https://img.shields.io/badge/development-spec--driven-3178C6)
![AI Agent Friendly](https://img.shields.io/badge/AI-agent%20friendly-1F883D)

[Website](https://fonijbuild.github.io/easy-starters/) · [FonijBuild](https://github.com/FonijBuild) · [Discussions](https://github.com/orgs/FonijBuild/discussions) · [Issues](https://github.com/FonijBuild/easy-starters/issues)

</div>

> “What do we build for, if not to lessen each other’s hardship?”

## What is Easy Starters?

Easy Starters is a collection of opinionated, production-ready software foundations for building real products without starting every project from an empty repository or an oversized boilerplate.

Each starter provides a focused baseline for a specific product architecture. The goal is not to include every possible library or feature. The goal is to give you a maintainable foundation with sensible defaults, clear boundaries, development tooling, documentation, and room to evolve.

Every starter works independently as a GitHub template.

**Fonij CLI is optional. You do not need Fonij to use any Easy Starter.**

## Starters

| Foundation            | Best for                                                            | Core stack                       | Repository                                                                                                                                                         |
| --------------------- | ------------------------------------------------------------------- | -------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **React SPA**         | Dashboards, internal tools, client-side products                    | React · Vite · TypeScript        | [Repository](https://github.com/FonijBuild/easy-vite-react-spa-starter) · [Use template](https://github.com/FonijBuild/easy-vite-react-spa-starter/generate)       |
| **Next.js Web**       | Web apps, SaaS applications, portals, and SEO-sensitive experiences | Next.js · React · TypeScript     | [Repository](https://github.com/FonijBuild/easy-nextjs-web-starter) · [Use template](https://github.com/FonijBuild/easy-nextjs-web-starter/generate)               |
| **Django API**        | Business APIs, admin workflows, multi-client backends               | Django · Python · PostgreSQL     | [Repository](https://github.com/FonijBuild/easy-django-api-starter) · [Use template](https://github.com/FonijBuild/easy-django-api-starter/generate)               |
| **Expo App**          | Cross-platform mobile products                                      | Expo · React Native · TypeScript | [Repository](https://github.com/FonijBuild/easy-expo-app-starter) · [Use template](https://github.com/FonijBuild/easy-expo-app-starter/generate)                   |
| **Browser Extension** | Browser tools and extension products                                | TypeScript · WebExtension APIs   | [Repository](https://github.com/FonijBuild/easy-browser-extension-starter) · [Use template](https://github.com/FonijBuild/easy-browser-extension-starter/generate) |
| **Python Service**    | Bots, workers, automations, integrations, and background services   | Python                           | [Repository](https://github.com/FonijBuild/easy-python-service-starter) · [Use template](https://github.com/FonijBuild/easy-python-service-starter/generate)       |
| **Starlight Docs**    | Developer docs, knowledge bases, and product documentation          | Astro · Starlight · TypeScript   | [Repository](https://github.com/FonijBuild/easy-starlight-doc-starter) · [Use template](https://github.com/FonijBuild/easy-starlight-doc-starter/generate)         |

## Choose the smallest foundation that fits

Start with what your product needs today.

| You are building...                                   | Start with        |
| ----------------------------------------------------- | ----------------- |
| A client-side web application                         | React SPA         |
| An API or business backend                            | Django API        |
| An iOS and Android application                        | Expo App          |
| A Chrome, Firefox, or Edge extension                  | Browser Extension |
| A Telegram bot, worker, automation, or Python service | Python Service    |
| Technical documentation or a knowledge base           | Starlight Docs    |

Do not start with a larger architecture only because you may need it someday.

A product should be able to grow when its requirements grow.

## Philosophy

Easy Starters follows a few simple principles:

**Production-capable, not kitchen-sink.**  
A starter should contain the foundations most real projects need without forcing optional product decisions on everyone.

**Architecture before libraries.**  
Clear boundaries, maintainability, and predictable project structure matter more than collecting dependencies.

**Smallest useful foundation.**  
Choose the architecture that satisfies today's requirements and evolve when the product actually needs more.

**Boring defaults are a feature.**  
Infrastructure and tooling should be understandable, replaceable, and easy to maintain.

**AI agents should understand the project.**  
Repository rules, specifications, architecture documentation, and explicit project contracts make the codebase easier for both humans and coding agents to work with.

## Built for spec-driven development

Easy Starters are designed to work well with AI coding agents without depending on a specific vendor or model.

The common project contract is:

```text
AGENTS.md
    ↓
Repository rules and development conventions

specs/
    ↓
What should be built

docs/
    ↓
Architecture and project knowledge

source code
    ↓
Implementation

quality checks
    ↓
Verification
```

A typical workflow is:

```text
Idea
  ↓
Specification
  ↓
Implementation
  ↓
Verification
  ↓
Documentation
```

`AGENTS.md` is intended to be the canonical repository-level instruction layer. Claude, Codex, Cursor, Gemini, Copilot, or another coding agent can work from the same project knowledge instead of requiring duplicated architecture instructions for every tool.

## Use a starter directly

You can create a project from any starter with GitHub's template feature.

For example:

```bash
gh repo create my-api \
  --template FonijBuild/easy-django-api-starter \
  --private \
  --clone

cd my-api
```

Then follow that starter's README for stack-specific setup.

You can also open any repository above and click **Use this template**.

## Use with Fonij

Easy Starters also form the foundation layer of [FonijBuild](https://github.com/FonijBuild), an AI-first product builder ecosystem for turning ideas into maintainable software.

Fonij can use structured foundation metadata to understand which architecture best fits a product and create projects from these foundations.

The intended product journey is:

```text
Validate
   ↓
Architect
   ↓
Build
   ↓
Evolve
```

Using Fonij is optional.

The starters remain independently usable GitHub templates.

## What belongs in a foundation?

A foundation should contain architectural decisions that are broadly useful for products in its category.

Depending on the stack, that may include:

```text
project structure
configuration
environment handling
linting and formatting
type checking
testing foundations
CI
deployment foundations
container support
architecture documentation
specification structure
AI-agent instructions
Fonij metadata
```

Product-specific features generally do **not** belong in the baseline.

Authentication providers, payments, analytics, CMS integrations, complex state management, business domains, and similar choices should only be added when a product actually requires them.

## Repository contract

Official Easy Starters use a shared repository philosophy.

```text
.fonij/starter.json
```

Describes the foundation to Fonij.

```text
AGENTS.md
```

Defines repository rules for AI coding agents.

```text
specs/
```

Contains implementation-ready specifications.

```text
docs/
```

Contains architecture and repository-specific knowledge.

The exact structure varies where the underlying technology requires it, but the intent remains consistent.

## Independent by design

Easy Starters are not wrappers around Fonij CLI.

They are ordinary repositories that can be:

- cloned,
- forked,
- used as GitHub templates,
- modified freely,
- and deployed with standard ecosystem tooling.

Fonij adds architecture selection and evolution on top of these foundations; it is not required to make them useful.

## Why FonijBuild?

Easy Starters originally began as a standalone collection of reusable software templates.

They now live under FonijBuild because they form the architectural foundation layer of a broader product-building ecosystem.

Keeping them together makes it possible to improve the same foundations for two audiences:

```text
developers using GitHub templates directly

and

developers using Fonij to plan, create, and evolve products
```

The foundations remain useful in both cases.

## Contributing

If you find a bug or want to propose an improvement to a specific foundation, open an issue in that starter's repository.

For ideas that affect the whole Easy Starters collection, use [Easy Starters Issues](https://github.com/FonijBuild/easy-starters/issues).

For broader product and architecture discussions, use [FonijBuild Discussions](https://github.com/orgs/FonijBuild/discussions).

Changes should preserve the main goal of the collection:

> Provide the smallest maintainable production foundation for the problem being solved.

## License

Easy Starters are open source under the [MIT License](https://github.com/FonijBuild/easy-starters/blob/main/LICENSE).

Individual starter repositories also include their own license files.

---

<div align="center">

**Easy Starters by [FonijBuild](https://github.com/FonijBuild)**

Production-ready foundations for building products that can evolve.

</div>
