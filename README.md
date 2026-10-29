<h1 align="center">Privilege</h1>
<p align="center"><b>Eat Well. Stay Well.</b></p>
<p align="center">
  A security-first fitness and nutrition app that merges your workouts, your sports, and your meals into one plan.
</p>

<p align="center">
 <img width="1083" height="1452" alt="2df7f6c8-d280-4c27-a25f-14af1ca325ec" src="https://github.com/user-attachments/assets/45047282-4115-40d5-8653-234b6a225e56" />


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
- [Developers](#developers)
- [Contact](#contact)

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
  <img width="765" height="1024" alt="WhatsApp Image 2026-10-21 at 4 56 22 PM" src="https://github.com/user-attachments/assets/a6fe1dfe-1a5a-482e-a3bd-b700e35cd5e9" />

</p>

The concept layout covers: login, plan organiser, splits & sports merge, AI chat box, recipe recommendations, calorie tracking, sports & exercise tutorials, cheat meals organiser, and subscription plans.

> The layout above is a design concept. Final screens and copy may differ.

## Availability

Privilege is planned for both Google Play and the App Store. The image above is a concept of the store listings.

## Stakeholders

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
- **API gateway** with rate limiting and authentication.
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

## Developers

| Name | ID |
|---|---|
| Ibrahim Mohamed Haggag | 26104141 |
| Hossam Mohamed Ismail | 26104503 |
| Abdalla Hithem Alam | 26103049 |
| Ammar Osama Mohammad | 26103884 |

## Contact

Recommendations or issues? Reach us at **supportprivilegefitness@gmail.com**.

---

<p align="center"><i>Privilege: Eat Well. Stay Well.</i></p>
