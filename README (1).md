<p align="center">
  <img src="assets/logo.jpg" alt="Privilege logo" width="320">
</p>

<h1 align="center">Privilege</h1>
<p align="center"><b>Eat Well. Stay Well.</b></p>
<p align="center">
  A security-first fitness and nutrition app that merges your workouts, your sports, and your meals into one plan.
</p>

<p align="center">
  <img alt="Platform" src="https://img.shields.io/badge/platform-iOS%20%7C%20Android-informational">
  <img alt="Status" src="https://img.shields.io/badge/status-in%20development-orange">
  <img alt="Encryption" src="https://img.shields.io/badge/encryption-AES--256%20%7C%20TLS%201.3-success">
</p>

<p align="center">
  <img src="assets/device-mockup.png" alt="Privilege on a tablet" width="520">
</p>

---

## Table of Contents

- [About](#about)
- [Why Privilege?](#why-privilege)
- [Key Features](#key-features)
- [App Screens](#app-screens)
- [Availability](#availability)
- [Stakeholders](#stakeholders)
- [Plans & Rewards](#plans--rewards)
- [Security](#security)
- [Tech Stack](#tech-stack)
- [Testing & Validation](#testing--validation)
- [Compliance](#compliance)
- [Research Background](#research-background)
- [Contact](#contact)
- [License](#license)

## About

Privilege is a mobile fitness application for iOS and Android. Every user gets **free diet plans**, and can upgrade to **Premium** for personalized nutrition guidance, advanced workout tracking, and exclusive fitness challenges.

It was built as a university project, with security treated as a core feature rather than an afterthought, because fitness apps collect some of the most sensitive data there is: health metrics, activity history, and GPS location.

## Why Privilege?

Leading apps such as MyFitnessPal, Strava, and Nike Training Club differ mostly in look and branding. Underneath, they offer the same core features: tracking, basic analytics, and generic plans. Privilege targets that gap with features that go beyond tracking.

Research also points to a local need. Mobile health adoption in Egypt is only **27.4%**, held back by poor usability, static algorithms, and a lack of culturally adapted personalization.

## Key Features

| | Feature | What it does |
|---|---|---|
| 🤖 | **AI Chat Bot** | Intelligent assistant that helps build, merge, and adjust your plans |
| 🎮 | **Gamification** | Community challenges, streaks, and rewards to keep you consistent |
| 🥗 | **Nutrition** | Free diet plans, recipe recommendations, calorie tracking, and a **cheat meal organizer** for dietary flexibility |
| 🔀 | **Sports Merge** | Combine gym splits with other sports (e.g. Push Day + Basketball) in a single schedule |
| 📈 | **Progression** | Classified user levels (Beginner → Intermediate → Pro) that structure your fitness journey |
| ⌚ | **Wearable Integration** | Real-time tracking from connected devices |
| 🎥 | **Tutorials** | Exercise and sport tutorials (gym, basketball, swimming, and more) |
| 📅 | **Plan Organiser** | Weekly calendar and daily scheduling with quick-add |

## App Screens

<p align="center">
  <img src="assets/app-layout.jpg" alt="Privilege interactive app layout" width="700">
</p>

The concept layout covers: login, plan organiser, splits & sports merge, AI chat box, recipe recommendations, calorie tracking, sports & exercise tutorials, cheat meals organiser, and subscription plans.

> The layout above is a design concept. Final screens and copy may differ.

## Availability

<p align="center">
  <img src="assets/store-listing.jpg" alt="Privilege store listings concept" width="700">
</p>

Privilege is planned for both Google Play and the App Store. The image above is a concept of the store listings.

## Stakeholders

<p align="center">
  <img src="assets/stakeholders.jpg" alt="Privilege app stakeholders" width="700">
</p>

End users, fitness coaches and nutritionists, partners and sponsors (gyms and food providers), the app developers and tech team, and administrators and management.

## Plans & Rewards

**Tiers**

- **Free:** basic access and free diet plans
- **Premium:** personalized nutrition, advanced workout tracking, exclusive challenges

**Earn discounts by staying disciplined**

| Milestone | Reward |
|---|---|
| 90-day streak | 25% off 1 month of Premium |
| Intermediate level | 35% off 1 month of Premium |
| 180-day streak | 50% off 1 month of Premium |
| Pro level | 100% off 1 month of Premium |

## Security

Traditional fitness apps keep long-lived authentication states and store sensitive biometric data in persistent local storage or insecure remote environments. If a phone or wearable is compromised, an attacker can extract full workout history, GPS telemetry, and physiological data.

Privilege is designed to reduce that exposure:

- **180-second decaying token framework.** Session permissions are mirrored non-persistently in volatile memory and zero-masked on expiration.
- **AES-256** encryption for data at rest.
- **TLS 1.3** for all communications.
- **Role-based access control (RBAC).**
- **API gateway** with rate limiting and authentication.
- **PostgreSQL** with encryption at rest.
- **Multi-factor authentication** for admin access to servers.
- **Regular vulnerability scanning and patching.**
- **Hardware security enclave certificates** signed before deployment.

**Threats addressed**

- Data-scraping injections
- Broken Object-Level Authorization (BOLA)
- Real-time Bluetooth Low Energy (BLE) ambient signal sniffing

## Tech Stack

| Layer | Technology |
|---|---|
| Mobile | Flutter / React Native (iOS & Android) |
| Database | PostgreSQL (encrypted at rest) |
| API | API gateway with rate limiting & authentication (GraphQL) |
| Hosting | Cloud-based, with redundancy and failover |
| Security | AES-256, TLS 1.3, RBAC |

## Testing & Validation

- **Penetration testing:** simulated attacks on the app and backend
- **Load testing:** stability under peak usage
- **Automated SAST/DAST scanning:** deep static and dynamic verification
- **GraphQL mutation fuzzing:** 25-million request high-density loop
- **Volatile memory forensic audits:** verify the zero-state mask
- **Internal QA and controlled beta testing**

## Compliance

Pre-launch validation targets:

- GDPR
- ISO 27001
- Local data protection regulations

The release schedule is a hard gate: a failed milestone blocks the release build. The production deadline was **19 October 2026**.

## Research Background

- Tong, H.L., et al. (August 18, 2022). *PLOS Digital Health.* Fitness tracking apps improve accountability and self-monitoring; active users are nearly twice as likely to meet recommended aerobic activity guidelines.
- Arafa, A., et al. (December 9, 2022). *Journal of Personalized Medicine.* Mobile health adoption in Egypt is only 27.4%, with usability, static algorithms, and lack of cultural personalization as major barriers.

## Contact

Recommendations or issues? Reach us at **supportprivilegefitness@gmail.com**.

## License

No license has been chosen yet. Add a `LICENSE` file (for example MIT) before making the repository public.

---

<p align="center"><i>Privilege: Eat Well. Stay Well.</i></p>
