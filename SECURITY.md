# Security Policy

## Supported Versions

We actively support the following versions of the Astro app and its deployment configurations. Ensure you are using a supported version to receive the latest security updates.

| Version       | Supported          |
|---------------|--------------------|
| v1.x.x        | ✅ Yes             |
| Older versions| ❌ No              |

---

## Reporting a Vulnerability

If you discover a security vulnerability, please follow these steps to report it responsibly:

1. **Do Not Publicly Disclose**: Avoid posting details of the vulnerability in public forums or repositories.
2. **Contact Us**: Email a detailed description of the issue to: `security@brainsait.io`.
3. **Provide Context**:
   - Steps to reproduce the issue.
   - Affected versions or configurations.
   - Environment details and logs, if applicable.

**Response Time**: We will acknowledge reports within **48 hours** and prioritize fixing the vulnerability based on its severity.

---

## Security Best Practices for Contributors

### General Guidelines
- **Use SSH Authentication**: Interact with the repository using SSH keys, not HTTPS credentials.
- **Follow Principle of Least Privilege**: Limit access to repository secrets and Cloudflare credentials.
- **Avoid Sensitive Data Exposure**: Never commit API keys, tokens, or other sensitive data to the repository.
- **Regular Dependency Updates**: Use tools like `npm audit` to regularly check for vulnerabilities in dependencies.

### Deployment Security
- **Environment Variables**: Use `.env` files to store sensitive credentials (e.g., Cloudflare API tokens).
- **Restrict API Keys**: Use API tokens with minimal permissions required for deployment.
- **Enable HTTPS**: Ensure all communication between your app and Cloudflare uses HTTPS.
- **Monitor Logs**: Regularly review Cloudflare and application logs to detect unusual activities.

---

## Dependency and CI/CD Security

- **Scan Dependencies**: Use `npm audit` and similar tools to detect vulnerabilities in dependencies.
- **Secure CI/CD Pipelines**: Ensure deployment pipelines are configured to prevent unauthorized access.
- **Code Reviews**: Require code reviews for all pull requests to maintain codebase integrity.

---

## Recommended Tools

To enhance security, we recommend:

- **Dependabot**: Automatically update dependencies to fix vulnerabilities.
- **npm audit**: Identify and resolve vulnerabilities in project dependencies.
- **CodeQL**: Analyze code for potential security issues.

---

## Response Policy

When a vulnerability is reported:

1. We will investigate and reproduce the reported issue.
2. If confirmed, we will prioritize a fix and communicate a timeline to the reporter.
3. After resolution, we will:
   - Notify the reporter.
   - Publish a security advisory, if applicable.
   - Backport the fix to supported versions.

---

## Contact

If you have any questions about this security policy or need assistance, contact us at: `security@brainsait.io`.
