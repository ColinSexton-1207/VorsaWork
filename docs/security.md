# Security Strategy

## Authentication
- **Login Options:**
&nbsp;&nbsp;&nbsp;- Email/Password (w/ JWT issued)
&nbsp;&nbsp;&nbsp;- Google OAuth2 (via Spring Security)

- **JWT Contents:**
&nbsp;&nbsp;&nbsp;- `sub` = userId
&nbsp;&nbsp;&nbsp;- `roles` = ROLE_USER / ROLE_ADMIN
&nbsp;&nbsp;&nbsp;- `exp` = token expiration

## Authorization
- Role-based access control (RBAC)
- Routes protected via Spring Security annotations

## CORS, Headers, Other Protections
- `Strict-Transport-Security`, `Content-Security-Policy`
- Cross-origin configured for frontend domain

## Future Hardening
- Rate limiting (Bucket4j or API Gateway)
- CAPTCHA on login