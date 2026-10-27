# Technical overview

This overview describes technology **documented in the supplied SoulLantern engineering records**. It does not imply a public production deployment.

| Area | Documented implementation |
|---|---|
| Mobile client | Expo and React Native; Expo Router appears in dependency checks |
| API | Express server and protected API routes |
| Authentication | Replit-managed Clerk, `@clerk/expo`, Clerk middleware |
| Session storage | Expo SecureStore for Clerk tokens |
| Local content | AsyncStorage for prayers, journals, faith preferences, and sync state |
| Subscription integration | RevenueCat SDK keys, subscription/entitlement integration work |
| AI | Server-side AI integration for prayer generation; provider credentials remain server-side |
| Backend data | Database-backed owner-scoped sync/export/deletion routes described in audit |
| Build/release | Expo exports, EAS configuration, Replit deployment planning |

## High-level flow

```text
Expo / React Native app
   |-- Clerk authentication -> SecureStore token cache
   |-- Local journal and prayer data -> AsyncStorage
   |-- Subscription UI -> RevenueCat integration
   `-- Authenticated requests -> Express API
                                   |-- Owner-scoped data/sync operations
                                   `-- Server-side AI prayer generation
```

## Security and production boundaries

The audit reports owner-scoped protected endpoints and separation of server secrets from public mobile configuration. It also identifies work remaining before public release, including production API configuration, local content protection, subscription environment separation, and provider callback verification. A passing test or code audit is not equivalent to live production validation.

## What is intentionally omitted

No private source, credentials, customer records, production endpoints, tokens, or internal environment values are included in this portfolio package.
