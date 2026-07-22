# Pull Request Template

Thank you for contributing to **ForgeOps** 🚀

Before submitting your Pull Request, please make sure your changes follow the contribution guidelines.

Related documentation:

* `CONTRIBUTING.md`
* `CODE_OF_CONDUCT.md`
* `SECURITY.md`

---

# 📌 Pull Request Summary

## Description

<!--
Describe what this Pull Request changes.

Explain:
- What was implemented?
- Why was it needed?
- What problem does it solve?
-->

---

# 🔗 Related Issue

<!--
Link the related GitHub Issue.

Example:

Closes #123
-->

Issue:

---

# 🎯 Type of Change

Select the relevant option:

* [ ] New feature
* [ ] Bug fix
* [ ] Documentation update
* [ ] Refactoring
* [ ] Performance improvement
* [ ] Security improvement
* [ ] Build/CI improvement
* [ ] Test improvement
* [ ] Breaking change

---

# 🏗 Architecture Impact

Does this change affect the architecture?

* [ ] No architecture impact
* [ ] Minor architecture change
* [ ] Requires ADR
* [ ] Introduces new module/service
* [ ] Changes existing interfaces

If applicable, reference:

```
docs/adr/
```

---

# 📂 Affected Components

Select all that apply:

* [ ] Platform Core
* [ ] AI Platform
* [ ] Agent Runtime
* [ ] Workflow Engine
* [ ] MCP Platform
* [ ] Integrations
* [ ] SDK
* [ ] API
* [ ] Infrastructure
* [ ] Documentation
* [ ] Security
* [ ] Testing

---

# 🧪 Testing

Describe the tests performed.

## Automated Tests

* [ ] Unit tests
* [ ] Integration tests
* [ ] End-to-end tests
* [ ] Performance tests

Commands executed:

```bash
mvn clean verify
```

or:

```bash
pytest
```

---

# 📖 Documentation

Documentation impact:

* [ ] Documentation updated
* [ ] New documentation created
* [ ] No documentation required

Related documentation:

```
docs/
```

---

# 🔒 Security Review

Security considerations:

* [ ] No security impact
* [ ] Security reviewed
* [ ] New permissions introduced
* [ ] New secrets/configuration introduced
* [ ] Authentication/authorization affected

---

# 📸 Screenshots / Examples

If applicable, provide:

* Screenshots
* API examples
* Architecture diagrams
* Logs
* Demonstrations

---

# ⚠ Breaking Changes

Does this change break compatibility?

* [ ] No
* [ ] Yes

If yes, describe:

```text
```

---

# 🚀 Deployment Considerations

Does this change require deployment actions?

* [ ] No
* [ ] Database migration
* [ ] Configuration update
* [ ] Infrastructure change
* [ ] Environment variable changes

Details:

```text
```

---

# ✅ Pull Request Checklist

Before requesting review:

## Code Quality

* [ ] Code follows project standards
* [ ] No unnecessary changes included
* [ ] No debug code remains
* [ ] Code is readable and maintainable

---

## Testing

* [ ] Tests added or updated
* [ ] All tests pass locally
* [ ] No regression introduced

---

## Documentation

* [ ] Documentation updated
* [ ] Architecture changes documented
* [ ] ADR created when necessary

---

## Security

* [ ] No secrets committed
* [ ] Dependencies reviewed
* [ ] Security considerations evaluated

---

## Git

* [ ] Commit messages follow Conventional Commits
* [ ] Branch follows naming conventions
* [ ] Pull Request is focused on one objective

---

# 👀 Reviewer Notes

Additional information for reviewers:

```text
```

---

# 🙏 Final Checklist

By submitting this Pull Request, I confirm that:

* I have read the contribution guidelines.
* I have followed project standards.
* I have tested my changes.
* I have updated documentation where necessary.
* I understand that maintainers may request changes before merging.

Thank you for contributing to ForgeOps 🚀

