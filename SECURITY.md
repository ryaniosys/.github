# Security Policy

## Reporting a Vulnerability

**Please do NOT create a public GitHub issue for security vulnerabilities.**

### How to Report

1. **GitHub Private Reporting** (preferred)  
   Use [GitHub's private vulnerability reporting](https://github.com/ryaniosys/.github/security/advisories/new)

2. **Email**  
   Contact: security@iosys.swiss

### What to Include

- Description of the vulnerability
- Steps to reproduce
- Potential impact
- Any suggested fixes (optional)

### Response Timeline

- **Acknowledgment**: Within 48 hours
- **Initial assessment**: Within 5 business days
- **Resolution target**: Depends on severity

### Severity Levels

| Level | Description | Target Resolution |
|-------|-------------|-------------------|
| Critical | Active exploitation, data breach risk | 24-48 hours |
| High | Significant security impact | 7 days |
| Medium | Limited impact, requires specific conditions | 30 days |
| Low | Minimal impact | Next release |

## Supported Versions

We provide security updates for the latest release of each active project.

## Security Best Practices

When contributing:
- Never commit secrets, API keys, or credentials
- Use environment variables for sensitive configuration
- Follow the principle of least privilege
- Keep dependencies updated
