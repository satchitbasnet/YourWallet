# YourWallet

YourWallet is a modern fintech platform for instant, borderless person-to-person and business-to-business payments. The concept
blends traditional banking rails with blockchain interoperability, enabling users to seamlessly move value between fiat accounts,
debit cards, and crypto wallets while enjoying strong security and compliance controls.

## Key Pillars

- **Frictionless onboarding** – Sign up with email and ID verification, no credit checks or waiting periods.
- **Instant transfers** – Send and receive payments between consumers or businesses using ACH, cards, crypto deposits, or peer-to-peer transfers.
- **Open cash-in and cash-out** – Load and off-ramp funds via bank accounts, debit/credit cards, or supported crypto networks.
- **Multiple payment methods** – Empower users with a Visa-branded card, virtual wallet balances, and crypto withdrawals.
- **Security-first** – Advanced encryption, risk monitoring, fraud detection, and regulatory compliance to safeguard funds and data.

## Documentation

| Document | Description |
| --- | --- |
| [Product Overview](docs/product_overview.md) | Target personas, feature set, user flows, and unique selling points. |
| [Technical Architecture](docs/technical_architecture.md) | Platform components, data flows, integrations, and deployment blueprint. |
| [Security & Compliance](docs/security_compliance.md) | Controls for KYC/AML, fraud prevention, data protection, and auditing. |
| [Visa Card Program Roadmap](docs/card_program.md) | Steps to launch a YourWallet-branded Visa card program. |

## Android application

The `android/` directory now contains the first iteration of the YourWallet mobile client:

- Kotlin-based Android app module configured for SDK 34
- Material 3 theming with a branded adaptive launcher icon
- Simple MVVM-friendly welcome screen that introduces the product vision

### Prerequisites

- Android Studio Giraffe (or newer) with the Android SDK 34 platform
- JDK 17+

### Running the app

1. Open Android Studio and select **Open an Existing Project**.
2. Choose the `android/` folder in this repository.
3. Let Gradle sync the project (internet access required for dependencies).
4. Use **Run > Run 'app'** to install the debug build on an emulator or connected device.

## Getting Started

1. Review the product and technical documentation in the `docs/` folder.
2. Explore the Android client implementation in `android/app` to understand navigation, UI composition, and future extension points.
3. Define milestones for MVP delivery: onboarding, wallet ledger, payments, compliance operations, and card issuance.

## Roadmap Snapshot

- **MVP (0-6 months)**: Digital wallet core, user onboarding, ACH/card/crypto funding, instant P2P transfers, bank and crypto off-ramps.
- **Growth (6-12 months)**: Business accounts, invoicing, developer APIs, risk scoring, enhanced analytics.
- **Scale (12+ months)**: Multi-currency support, expanded geographic compliance, DeFi integrations, embedded finance partnerships.

## License

This repository currently contains planning documentation only. Implementation details and licensing will be defined as the project progresses.
