# Contributing to ForgeOps

First of all, thank you for considering contributing to **ForgeOps**.

ForgeOps is an open source initiative focused on building an AI-native engineering platform that combines Artificial Intelligence, Autonomous Agents, Platform Engineering, Cloud Computing, DevOps, Site Reliability Engineering (SRE), Workflow Automation, and Enterprise Architecture.

Every contribution—whether code, documentation, testing, ideas, bug reports, or design discussions—helps move the project forward.

---

# 🌍 Our Philosophy

ForgeOps is built around a few fundamental principles.

## Documentation First

Documentation is not an afterthought.

Every significant feature starts with documentation before implementation.

The expected workflow is:

```text
Idea
    ↓
Discussion
    ↓
Documentation
    ↓
Architecture Decision (ADR)
    ↓
Implementation
    ↓
Tests
    ↓
Review
    ↓
Release
```

---

## Architecture Before Code

Every new module should have a documented architecture.

Contributors should understand:

* Why the feature exists
* Which problem it solves
* How it integrates with the platform
* Which APIs it exposes
* Which events it publishes
* Which dependencies it introduces
* How it should evolve

Implementation comes after architectural agreement.

---

## Small Pull Requests

We strongly encourage small, focused Pull Requests.

Good Pull Requests:

* Solve one problem
* Are easy to review
* Include tests
* Include documentation
* Do not introduce unrelated changes

---

## Quality Over Speed

ForgeOps values maintainability more than rapid feature delivery.

Before submitting code, ask yourself:

* Is it readable?
* Is it testable?
* Is it documented?
* Is it modular?
* Does it follow the project architecture?

---

# 🤝 Ways to Contribute

You do not need to write code to contribute.

We welcome contributions in many forms:

## Documentation

* Improve documentation
* Correct mistakes
* Add diagrams
* Improve examples
* Translate documentation (future)

---

## Development

* New features
* Bug fixes
* Performance improvements
* Refactoring
* API improvements

---

## Artificial Intelligence

* Prompt engineering
* Agent design
* Evaluation datasets
* Memory strategies
* Context management
* RAG improvements
* MCP integrations

---

## Platform Engineering

* Kubernetes
* Docker
* Terraform
* CI/CD
* GitHub Actions
* Infrastructure as Code

---

## Testing

* Unit tests
* Integration tests
* Contract tests
* End-to-end tests
* Performance tests

---

## Security

* Vulnerability reports
* Security reviews
* Dependency analysis
* Threat modeling

---

# 🚀 Getting Started

## Prerequisites

Before contributing, install the following tools:

* Git
* Java 24
* Maven 3.9+
* Python 3.13
* Docker
* Docker Compose
* IntelliJ IDEA (recommended)
* Visual Studio Code (optional)

---

## Clone the Repository

```bash
git clone https://github.com/<organization>/forgeops.git

cd forgeops
```

---

## Build the Project

```bash
mvn clean install
```

---

## Run Tests

```bash
mvn test
```

---

## Start Local Infrastructure

```bash
docker compose up -d
```

---

# 🌳 Git Workflow

ForgeOps follows a structured Git workflow.

## Main Branches

```text
main
develop
```

### main

* Stable releases
* Production-ready code
* Tagged versions only

---

### develop

Main integration branch.

All feature development starts here.

---

# 🌱 Feature Branches

Every contribution should use a dedicated feature branch.

Examples:

```text
feature/context-engine

feature/memory-engine

feature/workflow-runtime

feature/github-connector

feature/admin-dashboard
```

Naming convention:

```text
feature/<feature-name>
```

---

# 🐛 Bug Fixes

Bug fixes use:

```text
bugfix/<bug-name>
```

Example:

```text
bugfix/mcp-session-timeout
```

---

# 🔥 Hotfixes

Critical production fixes use:

```text
hotfix/<version>
```

Example:

```text
hotfix/1.0.1
```

---

# 🚀 Release Branches

Release preparation uses:

```text
release/1.0.0

release/1.1.0
```

---

# 📝 Branch Naming Rules

Use:

* lowercase
* hyphens
* descriptive names

Good examples:

```text
feature/openapi-generator

feature/multi-agent-runtime

feature/github-actions

feature/vector-search
```

Avoid:

```text
feature/test

feature/new

feature/update

feature/fix
```

---

# 📂 Repository Organization

Contributors should respect the repository organization.

```text
apps/
platform/
packages/
agents/
workers/
sdk/
connectors/
docs/
tests/
infrastructure/
```

Every module has a clearly defined responsibility.

Avoid introducing dependencies between unrelated modules.

---

# 📖 Documentation Requirements

Every significant feature should include documentation.

Documentation may include:

* Architecture
* Design decisions
* Sequence diagrams
* API documentation
* Examples
* Configuration guides
* Testing strategy

Documentation lives under the `docs/` directory and should evolve together with the code.

---

# ✅ Before Opening a Pull Request

Please verify that:

* The project builds successfully.
* Tests pass locally.
* New functionality includes appropriate tests.
* Documentation has been updated when necessary.
* The change follows the existing architecture and coding standards.

These checks help keep ForgeOps consistent, maintainable, and welcoming to contributors.

# Contributing to ForgeOps (Part 02)

---

# 💻 Coding Standards

ForgeOps follows a consistent set of engineering principles across all modules.

Every contribution should prioritize:

* Readability
* Simplicity
* Maintainability
* Testability
* Consistency
* Performance
* Security

We value clean, understandable code over clever or overly complex implementations.

---

# 🏛 Architecture Principles

Every contribution should respect the platform architecture.

Core principles include:

* Clean Architecture
* Domain-Driven Design (DDD)
* SOLID Principles
* Separation of Concerns
* Dependency Inversion
* Composition over Inheritance
* API-First Design
* Event-Driven Communication
* AI-Native Design

Avoid introducing unnecessary coupling between modules.

---

# ☕ Java Guidelines

Java is the primary language for the platform.

General guidelines:

* Use Java 24 language features when appropriate.
* Prefer immutable objects whenever possible.
* Keep methods focused on a single responsibility.
* Avoid static state.
* Prefer constructor injection.
* Avoid field injection.
* Favor interfaces over implementations.
* Minimize framework-specific code inside the domain layer.

Recommended package organization:

```text id="w8h0vl"
feature/

├── application/
├── domain/
├── infrastructure/
├── api/
└── configuration/
```

---

# 🐍 Python Guidelines

Python is primarily used for AI runtimes, workers, model integrations, and experimentation.

General recommendations:

* Follow PEP 8.
* Use type hints.
* Prefer dataclasses or Pydantic models.
* Keep functions small.
* Document public APIs.
* Avoid unnecessary global state.

---

# 📦 Maven Standards

ForgeOps uses Maven as its official build system.

General rules:

* Every Java module must contain its own `pom.xml`.
* Shared dependency versions should be managed centrally.
* Keep dependencies to the minimum required.
* Avoid duplicate dependency declarations.
* Prefer official Maven plugins.

Typical commands:

```bash id="f1uj1i"
mvn clean verify

mvn test

mvn spring-boot:run
```

---

# 📝 Documentation Standards

Documentation is mandatory for significant changes.

Update documentation whenever you:

* Add features
* Change APIs
* Modify architecture
* Introduce new modules
* Add integrations
* Change workflows

Documentation should be:

* Clear
* Accurate
* Up to date
* Written in English
* Easy to navigate

---

# 🧪 Testing Standards

Every contribution should include appropriate tests.

Testing pyramid:

```text id="9r2gr0"
End-to-End Tests

Integration Tests

Unit Tests
```

Expected coverage:

| Type              | Expectation     |
| ----------------- | --------------- |
| Unit Tests        | Required        |
| Integration Tests | Recommended     |
| End-to-End Tests  | When applicable |

---

# 🔍 Code Quality

Every Pull Request should satisfy quality requirements.

Recommended tooling:

* Checkstyle
* SpotBugs
* PMD
* Spotless
* JaCoCo
* OWASP Dependency Check

Static analysis issues should be resolved before merging whenever possible.

---

# 📏 Formatting

Formatting should be automated.

Never manually reformat unrelated files.

Project standards are defined through:

* `.editorconfig`
* Spotless
* IDE formatting rules

---

# 🔒 Security Guidelines

Security is everyone's responsibility.

Contributors should:

* Validate inputs.
* Avoid hardcoded credentials.
* Never commit secrets.
* Use secure defaults.
* Follow least privilege.
* Keep dependencies updated.

Potential security vulnerabilities should be reported privately following the project's security policy.

---

# 🧾 Commit Message Convention

ForgeOps follows the Conventional Commits specification.

Format:

```text id="lzy7wx"
<type>(scope): description
```

Examples:

```text id="vmtmqj"
feat(agent): add planning engine

fix(api): resolve pagination issue

docs(ai): update RAG documentation

refactor(workflow): simplify execution pipeline

test(platform): add integration tests

chore(build): update Maven plugins
```

Common commit types:

* feat
* fix
* docs
* refactor
* test
* chore
* ci
* perf
* build

---

# 🔀 Pull Request Guidelines

Each Pull Request should:

* Address a single concern.
* Be easy to review.
* Include tests when applicable.
* Update documentation when required.
* Pass all automated checks.

Avoid mixing unrelated changes in the same Pull Request.

---

# 👀 Code Review

Code reviews are collaborative.

Reviewers should focus on:

* Correctness
* Architecture
* Readability
* Maintainability
* Security
* Performance
* Documentation

Feedback should remain respectful, constructive, and focused on the code rather than the contributor.

---

# 🚫 What to Avoid

Please avoid:

* Large unrelated changes.
* Dead code.
* Commented-out code.
* Breaking public APIs without discussion.
* Unnecessary dependencies.
* Duplicate implementations.
* Premature optimization.

---

# ✅ Pull Request Checklist

Before submitting your Pull Request, verify:

* [ ] Project builds successfully.
* [ ] Tests pass locally.
* [ ] Documentation has been updated.
* [ ] Code follows project standards.
* [ ] No secrets or credentials are included.
* [ ] Commit messages follow Conventional Commits.
* [ ] Changes are focused and self-contained.
* [ ] New functionality includes appropriate tests.
* [ ] Public APIs are documented.

Meeting these expectations helps maintain a high-quality, reliable, and sustainable codebase for the entire ForgeOps community.

# Contributing to ForgeOps (Part 03)

---

# 🏛 Project Governance

ForgeOps is a community-driven, documentation-first, AI-native engineering platform.

The project is governed through transparency, technical discussion, architectural consistency, and collaborative decision-making.

Our goals are to:

* Build a sustainable open source ecosystem.
* Maintain high engineering standards.
* Encourage respectful collaboration.
* Ensure long-term project stability.
* Preserve architectural consistency.

---

# 👥 Community Roles

As the project evolves, contributors may participate in different roles.

## Community Members

Anyone who uses ForgeOps, reports issues, asks questions, or participates in discussions.

Typical activities include:

* Reporting bugs
* Suggesting improvements
* Asking questions
* Sharing feedback
* Helping other users

---

## Contributors

Contributors actively improve the project.

Examples:

* Documentation
* Code
* Tests
* Diagrams
* Tutorials
* Examples
* Performance improvements
* Security improvements

---

## Reviewers

Reviewers help maintain project quality by evaluating Pull Requests.

Responsibilities include:

* Reviewing code
* Validating architecture
* Checking documentation
* Ensuring coding standards
* Providing constructive feedback

---

## Maintainers

Maintainers are responsible for the long-term health of the project.

Typical responsibilities include:

* Reviewing major changes
* Managing releases
* Maintaining documentation
* Triaging issues
* Guiding contributors
* Preserving architectural consistency

---

# 🏗 Architecture Decision Records (ADRs)

Significant architectural decisions should be documented as ADRs before implementation.

Typical ADR topics include:

* New modules
* Breaking changes
* Technology adoption
* Architectural patterns
* Major refactorings
* Infrastructure decisions
* Security strategies

Documentation:

```text id="rrdlr8"
docs/adr/
```

---

# 💡 Proposing New Features

Before implementing a significant feature:

1. Search existing GitHub Issues.
2. Search GitHub Discussions.
3. Review existing documentation.
4. Open a discussion if necessary.
5. Propose the architecture.
6. Wait for technical feedback.
7. Begin implementation after alignment.

This process reduces duplicated work and improves architectural consistency.

---

# 🐞 Reporting Bugs

A good bug report should include:

* Clear title
* Environment information
* Reproduction steps
* Expected behavior
* Actual behavior
* Screenshots or logs (if applicable)
* Relevant configuration details

The more information provided, the easier it is to investigate the issue.

---

# 💬 Discussions

GitHub Discussions should be used for:

* Questions
* Ideas
* RFCs
* Architecture proposals
* Community conversations
* Feature brainstorming

Avoid opening Issues for general questions when a Discussion is more appropriate.

---

# 📅 Roadmap Alignment

Contributors are encouraged to review the project roadmap before starting major work.

Roadmap documents:

```text id="vr2brz"
ROADMAP.md

docs/roadmap/
```

Aligning contributions with planned milestones helps avoid duplicated efforts and improves coordination.

---

# 📖 Documentation First

Every important feature should include documentation before implementation.

Recommended documentation includes:

* Overview
* Architecture
* Design decisions
* APIs
* Configuration
* Sequence diagrams
* Examples
* Testing strategy

Good documentation accelerates onboarding and simplifies future maintenance.

---

# 🌍 International Community

ForgeOps is intended for a global audience.

Project documentation should:

* Be written in English.
* Use clear technical language.
* Avoid unnecessary abbreviations.
* Prefer internationally recognized terminology.

Future translations may be supported by the community.

---

# 🧠 Knowledge Sharing

Knowledge sharing is strongly encouraged.

Examples include:

* Tutorials
* Blog posts
* Videos
* Conference talks
* Sample projects
* Reference architectures

Community-created educational content helps grow the ecosystem.

---

# ❤️ Recognition

Every contribution is valuable.

Recognition is based on the quality and impact of contributions rather than their size.

Contributions may include:

* Documentation
* Code
* Reviews
* Testing
* Community support
* Design discussions
* Architecture proposals

---

# 📜 Code of Conduct

All participants are expected to follow the project's Code of Conduct.

Please read:

```text id="zhdc5o"
CODE_OF_CONDUCT.md
```

before participating in discussions or contributing to the project.

---

# 🔒 Security

Security vulnerabilities should **not** be reported through public GitHub Issues.

Please follow the responsible disclosure process described in:

```text id="sbo4tp"
SECURITY.md
```

---

# 🆘 Getting Help

If you need assistance:

1. Read the documentation.
2. Search existing Issues.
3. Search GitHub Discussions.
4. Open a new Discussion if needed.
5. Open an Issue for confirmed bugs or feature requests.

Community members and maintainers will do their best to help.

---

# 🚀 Our Long-Term Vision

ForgeOps is not just another software project.

It is an initiative to create a comprehensive AI-native engineering platform that empowers developers, architects, platform engineers, DevOps teams, SREs, researchers, and organizations to build intelligent systems with confidence.

We believe that:

* Documentation should guide development.
* Architecture should precede implementation.
* Automation should simplify engineering.
* Open standards enable interoperability.
* Collaboration drives innovation.
* Open source strengthens the global technology community.

---

# 🙏 Thank You

Thank you for taking the time to contribute to ForgeOps.

Whether you improve a sentence in the documentation, report a bug, review a Pull Request, design a new architecture, or implement a major feature, your contribution matters.

Together, we are building an extensible, enterprise-grade, AI-native engineering platform for the global open source community.

---

**Happy coding, and welcome to the ForgeOps community! 🚀**
