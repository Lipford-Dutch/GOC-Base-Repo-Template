# Security Baseline

## Required Controls

- Branch protection on `main`
- Pull request review before merge
- Dependabot alerts and security updates
- Dependency Review on pull requests
- CodeQL or equivalent static analysis
- Secret scanning and push protection
- Least-privilege workflow permissions
- Environment-scoped secrets

## Secret Rules

Never commit:

- tokens
- passwords
- private keys
- certificates
- license keys
- customer data
- production configuration values

## Review Questions

- Does this change expand access?
- Does this change introduce a new secret?
- Does this change process sensitive data?
- Does this change alter release or deployment controls?
- Is rollback documented?

## Exceptions

Use `templates/security-exception.md` for time-bound exceptions.
