# ForgeOps Support Guide

> **Welcome to ForgeOps support.**

Thank you for using ForgeOps.

This document explains how to get help, report problems, ask questions, and interact with the ForgeOps community.

ForgeOps is an open source AI-native engineering platform built by and for the global engineering community.

Our goal is to provide clear documentation, effective collaboration channels, and a supportive environment for developers, architects, platform engineers, DevOps teams, SREs, and organizations.

---

# 🌍 Support Philosophy

ForgeOps follows an open source community support model.

We believe that the best support ecosystem is built through:

* High-quality documentation.
* Community collaboration.
* Transparent discussions.
* Shared knowledge.
* Reusable solutions.
* Continuous improvement.

Whenever possible, solutions should become part of the documentation so future users can benefit.

---

# 🆘 Getting Help

Before requesting support, we recommend following these steps:

## 1. Read the Documentation

The first place to look for answers is:

```text
docs/
```

Important documentation areas:

```text
docs/
├── architecture/
├── platform/
├── ai/
├── agents/
├── workflows/
├── integrations/
├── deployment/
├── security/
├── operations/
└── reference/
```

---

## 2. Search Existing Discussions

Before opening a new request:

* Search GitHub Discussions.
* Search existing Issues.
* Review documentation updates.

Your question may already have an answer.

---

## 3. Ask the Community

For questions, ideas, and general discussions use:

```text
GitHub Discussions
```

Recommended topics:

* Architecture questions.
* Implementation guidance.
* Design discussions.
* Best practices.
* Learning discussions.

---

# 📚 Documentation Support

ForgeOps follows a documentation-first approach.

If you find:

* Missing information.
* Incorrect documentation.
* Confusing explanations.
* Missing examples.

Please consider improving the documentation.

Documentation improvements are valuable contributions.

---

# 🐞 Bug Reports

If you believe you found a bug:

Use:

```text
GitHub Issues
```

A good bug report should include:

* Clear description.
* ForgeOps version.
* Environment details.
* Steps to reproduce.
* Expected behavior.
* Actual behavior.
* Logs when relevant.

---

# 💡 Feature Requests

Feature requests should explain:

* The problem being solved.
* Why the feature is valuable.
* Possible approaches.
* Expected impact.

Good feature requests focus on the problem before the solution.

---

# 🔒 Security Issues

Security vulnerabilities must not be reported publicly.

Please follow:

```text
SECURITY.md
```

Security reports require private communication.

---

# 🤝 Community Support

Community members can help by:

* Answering questions.
* Sharing examples.
* Improving documentation.
* Reviewing solutions.
* Helping newcomers.

A strong community reduces friction for everyone.

---

# 🚀 Before Asking for Help

Please provide enough context.

Helpful information:

* Operating system.
* ForgeOps version.
* Deployment method.
* Configuration details.
* Error messages.
* Logs.
* Relevant code examples.

Avoid sharing:

* Passwords.
* API keys.
* Tokens.
* Private credentials.
* Sensitive company information.

---

# 📌 Support Channels

The project uses different channels for different purposes.

| Need               | Channel              |
| ------------------ | -------------------- |
| Questions          | GitHub Discussions   |
| Bugs               | GitHub Issues        |
| Security           | SECURITY.md process  |
| Code Contributions | CONTRIBUTING.md      |
| Documentation      | Pull Requests        |
| Feature Ideas      | Discussions / Issues |

Using the correct channel helps maintain an organized project.

---

# 🌎 Global Community

ForgeOps is designed for a worldwide community.

We encourage:

* Respectful communication.
* Clear technical explanations.
* Knowledge sharing.
* Patience with different experience levels.
* Collaboration across cultures.

Everyone is welcome to participate.
# ForgeOps Support Guide (Part 02)

---

# 🐛 Reporting Bugs

Bug reports are essential for improving ForgeOps.

Before creating a bug report:

1. Search existing Issues.
2. Confirm the problem is reproducible.
3. Check whether the issue exists in the latest version.
4. Collect relevant diagnostic information.

A good bug report helps maintainers understand and resolve the problem faster.

---

# ✅ Bug Report Template

A useful bug report should include:

## Title

Use a clear and descriptive title.

Example:

```text
Agent Runtime fails when executing MCP tools
```

Avoid:

```text
Bug found
Problem
Help
```

---

## Description

Explain:

* What happened.
* What you expected to happen.
* Why it is problematic.

---

## Environment

Include:

```text
ForgeOps Version:

Operating System:

Java Version:

Python Version:

Docker Version:

Kubernetes Version:

Deployment Method:
```

---

## Steps to Reproduce

Provide exact steps.

Example:

```text
1. Start ForgeOps platform
2. Configure MCP connector
3. Execute workflow
4. Observe failure
```

---

## Logs

Include relevant logs.

Remove sensitive information before sharing.

Never include:

* Passwords.
* Tokens.
* API keys.
* Private credentials.

---

# 💡 Feature Requests

Feature requests help shape the future of ForgeOps.

Before requesting a feature:

* Check the roadmap.
* Search existing discussions.
* Explain the problem first.

---

# Good Feature Requests Include

## Problem

Describe the problem.

Example:

```text
Developers need a way to monitor agent execution history.
```

---

## Motivation

Explain why it matters.

Example:

```text
Without visibility, troubleshooting autonomous workflows becomes difficult.
```

---

## Proposed Solution

Describe possible approaches.

Example:

```text
Provide an execution timeline dashboard with agent events.
```

---

## Alternatives Considered

Explain other options.

This helps maintainers understand the decision process.

---

# 🧠 AI Feature Requests

AI-related requests should include additional context.

Consider describing:

* Expected model behavior.
* Required capabilities.
* Context requirements.
* Memory requirements.
* Tool usage.
* Evaluation criteria.
* Safety considerations.

Examples:

* New AI provider support.
* Agent capability improvements.
* Prompt strategies.
* RAG improvements.
* Evaluation methods.

---

# 🏗 Architecture Discussions

Major architectural discussions should not begin directly with implementation.

Recommended process:

```text
Idea

↓

Discussion

↓

Architecture Proposal

↓

ADR

↓

Implementation
```

Architectural documentation belongs in:

```text
docs/architecture/

docs/adr/
```

---

# 🔄 Support and Development Workflow

ForgeOps follows this workflow:

```text
User Question

↓

Community Discussion

↓

Documentation Improvement

↓

Issue (if needed)

↓

Implementation

↓

Release
```

The goal is to transform repeated questions into permanent knowledge.

---

# 📦 Installation Support

When requesting installation help, provide:

## Deployment Type

Example:

```text
Local Development

Docker Compose

Kubernetes

Cloud Deployment

Bare Metal
```

---

## Infrastructure Information

Include:

* CPU resources.
* Memory.
* Storage.
* Network configuration.
* Cloud provider (if applicable).

---

## Configuration

Include relevant configuration:

* Environment variables.
* Application settings.
* Deployment manifests.

Remove sensitive values before sharing.

---

# ☁ Cloud and Kubernetes Support

For Kubernetes-related issues, include:

* Kubernetes version.
* Cluster type.
* Namespace.
* Helm chart version.
* Deployment status.
* Pod logs.
* Events.

Useful commands:

```bash
kubectl get pods

kubectl describe pod <name>

kubectl logs <name>
```

---

# 🔌 Integration Support

When requesting help with integrations, provide:

* Integration name.
* Connector version.
* Authentication method.
* Configuration approach.
* Error messages.
* Expected behavior.

Examples:

* GitHub integration.
* Kubernetes connector.
* Terraform integration.
* Cloud provider integration.
* MCP server integration.

---

# 📖 Documentation Issues

Documentation problems should be treated as first-class issues.

Examples:

* Missing information.
* Incorrect examples.
* Broken links.
* Outdated architecture diagrams.
* Confusing explanations.

Documentation improvements are welcome through Pull Requests.

---

# 🤝 Helping Others

Community members are encouraged to help.

Helpful contributions include:

* Answering questions.
* Sharing solutions.
* Creating examples.
* Improving documentation.
* Explaining concepts.

Teaching others strengthens the entire ecosystem.

---

# ⏳ Expected Response Time

ForgeOps is maintained by contributors.

Response times depend on:

* Issue complexity.
* Maintainer availability.
* Community participation.
* Severity.

Critical security issues follow the process described in:

```text
SECURITY.md
```

---

# 🌱 Community First

The goal of support is not only solving individual problems.

The goal is building a knowledge ecosystem where every solved problem helps future users.

# ForgeOps Support Guide (Part 03)

---

# ❓ Frequently Asked Questions (FAQ)

This section contains common questions about ForgeOps.

As the project grows, this FAQ will evolve based on community feedback.

---

# What is ForgeOps?

ForgeOps is an AI-native engineering platform designed to combine:

* Artificial Intelligence.
* Autonomous Agents.
* Platform Engineering.
* DevOps automation.
* SRE practices.
* Cloud-native infrastructure.
* Enterprise integrations.
* Workflow orchestration.

The goal is to provide a unified platform for building, operating, and automating intelligent engineering systems.

---

# Is ForgeOps Open Source?

Yes.

ForgeOps is designed as an open source project with community collaboration as a core principle.

The project welcomes contributions including:

* Code.
* Documentation.
* Testing.
* Architecture proposals.
* Security improvements.
* Community support.

---

# Who can contribute?

Everyone is welcome.

Contributors may include:

* Software developers.
* Architects.
* DevOps engineers.
* Platform engineers.
* SRE professionals.
* AI engineers.
* Security researchers.
* Documentation contributors.
* Students and learners.

---

# Is ForgeOps production ready?

ForgeOps follows an incremental development approach.

Development phases are documented in:

```text id="9y2t0z"
ROADMAP.md
```

Early versions may focus on architecture, experimentation, and foundational capabilities before enterprise production adoption.

---

# How do I start developing ForgeOps?

Start by reading:

```text id="q1e8x7"
README.md

CONTRIBUTING.md

docs/
```

Then:

1. Configure the development environment.
2. Understand the architecture.
3. Review existing issues.
4. Select an area to contribute.
5. Follow the contribution workflow.

---

# Which technologies does ForgeOps use?

ForgeOps is built around modern cloud-native technologies.

Primary technologies include:

## Backend

* Java
* Maven
* Spring Boot

## AI Platform

* Python
* AI frameworks
* LLM providers
* RAG components
* MCP integrations

## Infrastructure

* Docker
* Kubernetes
* Terraform

## Integration

* REST APIs
* OpenAPI
* Event-driven architecture

The technology stack evolves with the needs of the platform.

---

# How do I request a new feature?

Feature requests should be created through GitHub Discussions or Issues depending on maturity.

Before requesting:

1. Search existing proposals.
2. Explain the problem.
3. Describe expected benefits.
4. Consider alternatives.

Major architectural changes should include an ADR.

---

# How do I report a security issue?

Do not create a public Issue.

Follow:

```text id="9w8jca"
SECURITY.md
```

Security reports must be handled privately.

---

# 🏢 Enterprise Support

ForgeOps is designed with enterprise adoption in mind.

Future enterprise capabilities may include:

* Commercial support.
* Enterprise consulting.
* Architecture reviews.
* Deployment assistance.
* Training programs.
* Managed services.
* Priority support agreements.

Community support remains the foundation of the open source project.

---

# 🧑‍💻 Community Support vs Enterprise Support

## Community Support

Available to everyone:

* Documentation.
* GitHub Discussions.
* GitHub Issues.
* Community contributions.

---

## Enterprise Support (Future)

May include:

* Guaranteed response times.
* Professional services.
* Dedicated assistance.
* Security consulting.
* Custom integrations.

Details will be announced as the project matures.

---

# 📋 Support Responsibilities

## Users

Users should:

* Read documentation.
* Provide sufficient information.
* Respect community guidelines.
* Protect sensitive information.

---

## Contributors

Contributors should:

* Follow project standards.
* Improve documentation.
* Write quality code.
* Help other community members.

---

## Maintainers

Maintainers should:

* Maintain project quality.
* Review contributions.
* Guide technical decisions.
* Support community growth.

---

# 📈 Improving Support

ForgeOps continuously improves support processes through:

* Community feedback.
* Documentation improvements.
* Automation.
* Better examples.
* Improved tooling.

Support quality is considered part of the overall developer experience.

---

# 📚 Related Documents

For more information, see:

```text id="o6v4c1"
README.md

CONTRIBUTING.md

CODE_OF_CONDUCT.md

SECURITY.md

ROADMAP.md

docs/
```

---

# 🙏 Thank You

Thank you for being part of the ForgeOps community.

Whether you are:

* Asking your first question.
* Reporting a bug.
* Improving documentation.
* Submitting code.
* Helping another contributor.

Your participation helps build a stronger AI-native engineering ecosystem.

Together, we are building the future of intelligent software engineering.

---

**Welcome to ForgeOps 🚀**
