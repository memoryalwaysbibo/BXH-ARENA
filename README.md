# BXH ARENA Production

Production repository safety bootstrap.

## Environment
- Firebase project: `bxh-arena`
- Beta project `bxh-arena-beta` must never be a deployment target from this repository.
- Production domain will be connected only after migration validation.

## Migration safety
- Beta and Legacy repositories are read-only migration sources.
- Do not copy Beta `CNAME` or Beta deployment workflows unchanged.
- Do not grant Beta tester/test-admin privileges to Production users.
- Authentication and Firestore player data require UID/email-aware merge; never bulk-overwrite Production.
- Preserve eligible Pioneer title/qualification data separately.
- Firebase deployment remains disabled until Production credentials and targets are reviewed.
