
# TrustVault Threat Model

## Protected Assets

- User accounts and passwords
- Uploaded documents
- Document permissions
- Audit logs

## Threats and Mitigations

| Threat | Mitigation |
|---|---|
| Unauthorized document access | Server-side permission checks |
| Password theft | Password hashing |
| Unsafe filenames | Secure filename handling |
| Oversized uploads | 10 MB upload limit |
| SQL injection | Parameterized SQL queries |
| Unauthorized sharing | Permission checks before sharing |

## Known Limitations

- CSRF protection needs to be added.
- Audit log access needs role-based restrictions.
- Production deployment requires secure secret management.
- Uploaded files need persistent storage in production.
