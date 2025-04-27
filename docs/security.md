# Security Strategy

## Authentication
- **Login Options:**
  - Email/Password (w/ JWT issued)
  - Google OAuth2 (via Spring Security)

- **JWT Contents:**
  - `sub` = userId
  - `roles` = ROLE_USER / ROLE_ADMIN
  - `exp` = token expiration

## Authorization
- Role-based access control (RBAC)
- Routes protected via Spring Security annotations

## CORS, Headers, Other Protections
- `Strict-Transport-Security`, `Content-Security-Policy`
- Cross-origin configured for frontend domain

## Future Hardening
- Rate limiting (Bucket4j or API Gateway)
- CAPTCHA on login