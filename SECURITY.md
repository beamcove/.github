# Security Policy

## Our Commitment

Security is not an afterthought — it's baked into everything we do. We take the security of our software seriously, and we appreciate the security community's efforts in responsibly disclosing vulnerabilities to us.

**Translation**: If you find a security issue, please tell us before telling Twitter. We promise to take it seriously and work with you to fix it.

## Supported Versions

We provide security updates for the following versions:

| Version | Supported          | Notes                                    |
| ------- | ------------------ | ---------------------------------------- |
| 2.x.x   | :white_check_mark: | Current major version — actively supported |
| 1.x.x   | :warning:          | Security fixes only (until [date])       |
| < 1.0   | :x:                | No longer supported — please upgrade     |

**Pro tip**: Always use the latest version to get the most recent security updates. Yes, we know updating can be a pain, but so are security breaches.

## Reporting a Vulnerability

### Please DO NOT:

- ❌ Open a public GitHub issue about the vulnerability
- ❌ Discuss the vulnerability in public forums or social media
- ❌ Exploit the vulnerability beyond what is necessary to demonstrate it

### Please DO:

✅ **Report privately** using one of these methods:

1. **GitHub Security Advisory** (preferred)
   - Go to the repository's Security tab
   - Click "Report a vulnerability"
   - Fill out the form with as much detail as possible

2. **Email**
   - Send to: **security@example.com**
   - Use PGP encryption if possible (key: [PGP key ID/link])
   - Include "SECURITY" in the subject line

### What to Include in Your Report

A great security report includes:

- **Description of the vulnerability** — What's the issue?
- **Impact assessment** — What could an attacker do with this?
- **Steps to reproduce** — How can we see it ourselves?
- **Affected versions** — Which versions are vulnerable?
- **Suggested fix** — If you have ideas (optional but appreciated!)
- **Your contact information** — So we can follow up with you

**Example:**
```
Subject: SECURITY - SQL Injection in User Search

Description:
The user search endpoint is vulnerable to SQL injection via the 
'username' parameter.

Impact:
An attacker could potentially access or modify database contents,
including sensitive user data.

Steps to Reproduce:
1. Navigate to /api/users/search
2. Send a request with username=admin' OR '1'='1
3. Observe all users are returned

Affected Versions: 
2.0.0 through 2.3.1

Environment:
- OS: Ubuntu 22.04
- Database: PostgreSQL 14.2

Suggested Fix:
Use parameterized queries instead of string concatenation.

Contact: researcher@example.com
```

## What Happens Next?

Here's our commitment to you:

| Timeline | Action |
|----------|--------|
| **24 hours** | We'll acknowledge receipt of your report |
| **72 hours** | We'll provide an initial assessment and planned timeline |
| **90 days** | We aim to have a fix released (or explain why we need more time) |

### The Process

1. **Acknowledgment** — We'll confirm we received your report
2. **Investigation** — We'll validate the vulnerability and assess impact
3. **Fix Development** — We'll work on a patch (we may ask for your input!)
4. **Testing** — We'll verify the fix resolves the issue
5. **Release** — We'll deploy the fix to supported versions
6. **Disclosure** — After the fix is released, we'll publish a security advisory
7. **Credit** — We'll recognize you in the advisory (unless you prefer to remain anonymous)

## Security Best Practices for Users

While we work hard to keep our software secure, security is a shared responsibility. Here's what you can do:

- ✅ **Keep software updated** — Enable automatic updates if possible
- ✅ **Use strong authentication** — Complex passwords, MFA when available
- ✅ **Review access permissions** — Only grant what's necessary
- ✅ **Monitor for suspicious activity** — Set up alerts and logging
- ✅ **Report issues** — See something suspicious? Let us know!

## Scope

### In Scope

The following are within the scope of our security policy:

- All repositories under the Beamcove organization
- Official releases and distributions
- Documented APIs and integrations
- Authentication and authorization mechanisms
- Data handling and storage

### Out of Scope

The following are outside our security scope:

- Third-party dependencies (please report to the upstream project)
- Issues in deprecated or unsupported versions
- Theoretical vulnerabilities with no practical exploit
- Social engineering attacks
- Physical security issues
- DDoS attacks

## Security Updates

We publish security advisories through:

- **GitHub Security Advisories** — https://github.com/beamcove/.github/security/advisories
- **Security mailing list** — Subscribe at [link to mailing list]
- **Release notes** — Check CHANGELOG.md for security fixes

**Want to stay informed?** Watch our repositories and subscribe to our security announcements.

## Bug Bounty Program

We currently **[do/do not]** have a bug bounty program. 

<!-- If you have a bug bounty program, include details here:
**Rewards:**
- Critical vulnerabilities: $XXX - $XXX
- High severity: $XXX - $XXX
- Medium severity: $XXX - $XXX
- Low severity: Recognition in our hall of fame
-->

Even without monetary rewards, we deeply appreciate responsible disclosure and will:
- Credit you in our security advisories (with your permission)
- Add you to our security hall of fame
- Send you awesome swag (when available)
- Give you eternal gratitude and respect from the team

## Hall of Fame

We'd like to thank the following security researchers for responsibly disclosing vulnerabilities:

<!-- Add researchers here as they report issues -->
- *Your name could be here!*

## Questions?

Have questions about our security policy? Want to report a non-security bug? Need help with something else?

- **Security questions**: security@example.com
- **General bugs**: [Open an issue](../../issues)
- **Other inquiries**: [See our support page](SUPPORT.md)

---

**Remember**: Security vulnerabilities are not failures — they're opportunities to make our software better. Thank you for helping us keep our users safe!

*Last updated: [Date]*
