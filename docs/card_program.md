# Visa Card Program Roadmap

## Program Objectives

- Extend YourWallet balances to a globally accepted Visa debit card.
- Provide instant access to wallet funds for consumer and business customers.
- Enable real-time funding, spend controls, and reward experiences within the app.

## Stakeholders

| Role | Responsibilities |
| --- | --- |
| Product | Define card features, roadmap, and user experience. |
| Compliance | Ensure card program meets regulatory and network obligations. |
| Finance/Treasury | Manage settlement accounts, funding flows, and reconciliation. |
| Engineering | Build issuer processor integrations, card APIs, and in-app management. |
| Customer Support | Handle disputes, chargebacks, and user education. |
| Partner Manager | Liaise with sponsor bank, issuer processor, Visa, and vendors. |

## Launch Phases

1. **Discovery (0-2 months)**
   - Evaluate issuer processors (Marqeta, Galileo, Stripe Issuing, Unit).
   - Select sponsor bank and establish BIN sponsorship.
   - Define card product (debit vs prepaid), fee structure, rewards, and limits.

2. **Implementation (2-6 months)**
   - Sign commercial agreements with processor and Visa.
   - Complete program design packet (PDP) and Visa risk assessment.
   - Integrate processor APIs for card issuance, tokenization, controls, and webhook events.
   - Build funding logic (just-in-time funding, prefunding model, or hybrid).
   - Implement dispute management workflows and regulatory disclosures.

3. **Certification & Testing (5-7 months)**
   - Run Visa/Mastercard certification tests (VTS, EMV if physical cards).
   - Complete processor certification (end-to-end transaction testing, settlement validation).
   - Conduct pilot program with employees and selected users.

4. **Launch & Scale (7+ months)**
   - Roll out virtual cards with instant issuance and mobile wallet provisioning.
   - Ship physical cards with custom design, fulfillment, and activation tracking.
   - Launch rewards program tied to wallet usage and partner offers.
   - Monitor KPIs (activation rate, spend volume, interchange revenue, disputes).

## Key Technical Components

- **Card Issuance API**: Create, activate, suspend, and terminate cards; manage cardholder profiles.
- **Tokenization**: Integrate with Visa Token Service (VTS) for Apple Pay/Google Pay.
- **Transaction Webhooks**: Real-time authorization and clearing events for ledger updates.
- **Funding Model**: Just-in-time funding from wallet balance to processor authorization hold.
- **Controls & Alerts**: Spend limits, merchant category code (MCC) filters, geofencing, push notifications.
- **Dispute Handling**: User flows for dispute initiation, evidence upload, and case tracking.
- **Reporting & Reconciliation**: Daily settlement reports, fee summaries, and general ledger postings.

## Compliance & Legal Checklist

- Cardholder agreement, privacy policy, and electronic consent flows.
- Reg E and Reg Z disclosures (depending on product type).
- UDAAP review to ensure transparent fees and marketing.
- PCI DSS scope analysis; leverage processor for PAN handling.
- OFAC screening for cardholders and transaction monitoring for card spend.

## Operational Requirements

- 24/7 cardholder support with escalation paths for lost/stolen cards and disputes.
- Inventory management for physical cards (card stock, personalization, shipping).
- Chargeback management with strict response timelines and documentation.
- Fraud monitoring rules tuned for card-not-present and card-present transactions.
- Settlement funding: maintain required prefund levels, reconcile daily with processor.

## Future Enhancements

- Credit builder card or secured card offering.
- Co-branded card partnerships with merchants or marketplaces.
- Dynamic CVV and numberless cards for enhanced security.
- Embedded finance APIs allowing partners to issue cards backed by YourWallet.

