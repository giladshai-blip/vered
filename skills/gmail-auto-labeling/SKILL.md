# Skill: Automatic Gmail Labeling

## Owner
Vered — Executive Personal Assistant

## Mission
Keep Gmail classified with exactly one Vered user label per non-Spam/non-Trash message.

## Core rule
Every processed message must have exactly ONE custom Vered label.
Gmail system labels such as INBOX, UNREAD, SENT, IMPORTANT and category labels are provider-managed and do not count toward this rule.

## Canonical taxonomy
- 🔴 אבטחה וחשבונות
- 🔵 עבודה
- 🟢 משפחה
- 🩷 בריאות
- 🟤 ממשלה ורשויות
- 🟣 קריירה
- 🟡 נסיעות
- 🧾 חשבוניות וקבלות
- 🟠 כספים
- 🛒 קניות והזמנות
- 🔷 טכנולוגיה
- ⚪ כללי

## Priority
When a message matches more than one domain, assign the first matching category in this order:
1. אבטחה וחשבונות
2. עבודה
3. משפחה
4. בריאות
5. ממשלה ורשויות
6. קריירה
7. נסיעות
8. חשבוניות וקבלות
9. כספים
10. קניות והזמנות
11. טכנולוגיה
12. כללי

## Safety
- Do not delete mail as part of classification.
- Do not archive unless explicitly requested.
- Exclude Spam and Trash.
- Remove obsolete custom labels from messages before assigning the canonical label.
- Never intentionally apply two custom Vered labels to the same message.

## Color policy
The Gmail connector currently does not expose native label-color editing. Therefore canonical labels use visible color emoji prefixes.
If native label-color mutation becomes available, map each label to its corresponding visual color without changing the one-label rule.

## Maintenance
Review ⚪ כללי periodically and promote stable patterns into an existing category or a deliberately approved new category.
