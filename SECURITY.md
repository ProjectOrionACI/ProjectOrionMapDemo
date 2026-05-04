# Security Policy

## About

Orion Map Demo — developed by **Applied Concepts Inc / Stalker Street Dynamics**, created by DJ. Maintained under [ProjectOrionACI](https://github.com/ProjectOrionACI).

## Supported Versions

| Version | Supported |
|---------|-----------|
| v38 (current) | ✅ Active |
| < v38 | ❌ Not supported |

## Reporting a Vulnerability

1. Go to the [repository Security tab](https://github.com/ProjectOrionACI/ProjectOrionMapDemo/security)
2. Click **"Report a vulnerability"** to open a private advisory
3. Include: description, reproduction steps, impact assessment, your GitHub handle

We will acknowledge within **48 hours** and resolve confirmed issues within **7 days**.

## Security Measures

- Google Maps API key restricted to `projectorionaci.github.io/*` only
- API usage monitored via Google Cloud Console
- Session-based global API call limit (50 calls) to prevent runaway usage
- No backend, no database, no user data collected or stored
- Passphrase-gated access screen — real security is the API key referrer restriction
- Keys will be rotated on production deployment to dedicated infrastructure

## Known Exposure

The Google Maps API key is visible in the public HTML source. This is intentional for a GitHub Pages demo and is mitigated by:

- HTTP referrer restriction to the deployment domain only
- Active monitoring in Google Cloud Console
- Key will be rotated on production deployment

GitHub Secret Scanning will flag this key. This is acknowledged and accepted for demo purposes.

## Removed APIs

The following APIs were evaluated and removed due to browser CORS restrictions requiring a backend proxy:

- **Aerial View API** — server-side only
- **Roads API** — server-side only (speed limits, road snapping)

These may be reintroduced in a future version with a backend proxy layer.

## Scope

Primary security surface is the Google Maps API key. Reports about the Maps API itself should go to [Google's bug hunter program](https://bughunters.google.com).
