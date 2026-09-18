# Skill: Automatic Gmail Labeling

## Owner
Vered — Executive Personal Assistant

## Mission
Keep Gmail continuously classified using a stable, explainable taxonomy without deleting messages or changing read/unread state.

## Safety
- Never delete email as part of labeling.
- Never archive unless the user explicitly requests it.
- Never remove an existing user label merely because Vered adds a new one.
- Spam and Trash are excluded from normal classification.
- Multiple labels are allowed when one message belongs to multiple domains.

## Canonical Vered taxonomy
- ורד/מסווג — master marker for every processed message.
- ורד/כספים — banking, cards, salary, pension, insurance, taxes, receipts and financial notices.
- ורד/עבודה — Biscotti and other work-related communications.
- ורד/משפחה — communications involving family members, children and schools.
- ורד/קניות — orders, deliveries, purchase confirmations and retail.
- ורד/חשבוניות וקבלות — invoices, receipts and payment documents.
- ורד/קריירה — recruiters, LinkedIn career activity, job applications and professional opportunities.
- ורד/נסיעות — flights, hotels, booking services, car rental and travel logistics.
- ורד/בריאות — healthcare providers, clinics, appointments and medical administration.
- ורד/ממשלה ורשויות — government agencies, tax authority and official public services.
- ורד/אבטחה וחשבונות — sign-ins, password resets, verification codes and account-security notices.
- ורד/טכנולוגיה — developer services, cloud tools, AI services and technology platforms.
- ורד/כללי — processed messages not matching another Vered domain label.

## Classification strategy
1. Apply `ורד/מסווג` to every message except Spam and Trash.
2. Apply all matching domain labels using sender, domain, subject and Gmail category evidence.
3. After domain rules run, apply `ורד/כללי` only to messages with the master label and no domain label.
4. Preserve all previous labels.
5. Re-run safely: labeling is idempotent.

## Important-message behavior
Labeling is not importance detection. For alerts, Vered must separately inspect new mail and decide whether action is required.

## Maintenance
Periodically review:
- messages left in `ורד/כללי`;
- new frequent senders;
- false positives;
- categories with unusually large or small growth.

Update classification queries when stable sender patterns emerge.
