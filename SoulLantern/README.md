# SoulLantern

![SoulLantern portfolio banner](assets/soullantern-github-hero.png)

SoulLantern is a mobile project centered on prayer, personal reflection, and journaling. I worked on the experience as both a product and an engineering problem: making the interface approachable, connecting account and content flows, exploring a Premium offering, and working through the less visible details of mobile testing and release preparation.

## Why I built it

I wanted a quieter, more intentional space for people to return to their thoughts and spiritual practices. The challenge was to make personal content feel easy to revisit without turning the experience into a complicated productivity tool.

## Inside the project

![Selected app screens](assets/soullantern-product-overview.png)

- Prayer and journal/reflection content, with AI-assisted prayer generation represented in the development audit.
- Account sign-in and protected synchronization flows.
- Premium subscription interface and RevenueCat integration work.
- Mobile UI iteration, exports, build checks, and release preparation.

![Core experience](assets/soullantern-core-experience.png)

![Premium experience](assets/soullantern-premium.png)

## Technology

The available engineering audits document an **Expo / React Native** mobile application, an **Express** API, **Replit-managed Clerk** authentication, **RevenueCat** subscription integration, local **AsyncStorage**, **Expo SecureStore** for authentication tokens, and an AI-backed prayer-generation endpoint. These are documented integrations, not a claim that every production flow has passed live verification.

## Development and release status

![Development evidence](assets/soullantern-development.png)

The project has undergone build, export, API-test, mobile-test, and release-readiness work. The supplied audits also identify remaining production configuration, dependency alignment, privacy, storage, and social-sign-in verification tasks. **This repository is a portfolio case study, not a claim of App Store approval or a completed public release.**

## More detail

- [Project notes](docs/project-notes.md)
- [Technical overview](docs/technical-overview.md)
- [Testing and release notes](docs/testing-and-release.md)
- [Visual asset notes](docs/visual-asset-notes.md)

## Repository scope

This portfolio package documents the project using selected screenshots and development notes. It does not contain the full private application source, production credentials, API keys, or other secrets. Screenshots may show intermediate states and should not be interpreted as proof that a feature is live in production.
