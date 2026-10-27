# Project notes

## Product thinking
SoulLantern began with a simple question: how can a mobile experience make prayer, reflection, and journaling easier to return to? The design direction favors calm presentation, readable text, and a small number of clear actions.

## Experience decisions
The supplied UI captures show a light, restrained interface and a separate Premium area. The project has involved iterating on account flows, personal content, subscription presentation, and navigation. These screens document design states, not necessarily a single finalized build.

## Feature evolution
Engineering records describe prayer-generation behavior, local journal/prayer content, synchronization, exports, and account management. Subscription work includes RevenueCat and entitlement configuration. The available evidence supports describing these as implemented or integrated work, while live production behavior still requires verification.

## Monetization decisions
A Premium experience was developed, with subscription-related screens and RevenueCat configuration. Production purchases, entitlement behavior, and environment separation were flagged for further verification. No revenue or subscriber metrics are claimed.

## Iteration and lessons
- Real-device and release testing exposed issues that screenshots alone could not resolve, especially authentication callbacks and production environment wiring.
- A passing export or build does not by itself prove release readiness.
- Sensitive personal and spiritual content needs careful local storage, privacy disclosure, and access-control decisions.
- Subscription interfaces need to agree with real purchase configuration and entitlements.

These notes are based on available screenshots and audits; they are not a chronological changelog.
