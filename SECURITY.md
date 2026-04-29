# Security Policy

## About

Orion Map Platform — developed by **Applied Concepts Inc / Stalker Street Dynamics**, maintained under [ProjectOrionACI](https://github.com/ProjectOrionACI).

## Supported Versions

| Version | Supported |
|---------|-----------|
| v1.x (current) | ✅ Active |
| < v1.0 | ❌ Not supported |

## Reporting a Vulnerability

1. Go to the [repository Security tab](https://github.com/ProjectOrionACI/ProjectOrionMapDemo/security)
2. Click **"Report a vulnerability"** to open a private advisory
3. Include: description, reproduction steps, impact assessment, your GitHub handle

We will acknowledge within **48 hours** and resolve confirmed issues within **7 days**.

## Security Measures

- Google Maps API key restricted to `ProjectOrionACI.github.io/*` only
- API usage monitored via Google Cloud Console
- Keys rotated on production deployment
- No backend, no database, no user data collected or stored

## Scope

Primary security surface is the Google Maps API key. Reports about the Maps API itself should go to [Google's bug hunter program](https://bughunters.google.com).
