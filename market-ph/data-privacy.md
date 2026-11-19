# Data privacy: Philippines (RA 10173)

> Last reviewed: 2026-11 · Applies to: any product that collects personal data from people in the Philippines

**Not legal advice.** This page summarizes the Data Privacy Act of 2012 (Republic Act No. 10173) and guidance from the National Privacy Commission (NPC) for planning purposes only. Check current NPC issuances at [privacy.gov.ph](https://privacy.gov.ph), and get professional advice for anything high-risk.

## TL;DR (the rules)

- **Collect less.** Only collect personal data you have a clear, stated purpose for.
- **Inventory it.** Every project lists what personal data it stores, why, where, and for how long. Keep this in `docs/privacy.md` in the project repo.
- **Get consent, or have another lawful basis.** Consent must be freely given, specific, and informed. No pre-ticked boxes.
- **Publish a privacy notice** in plain language before or at collection: what you collect, why, who it's shared with, how long it's kept, how to contact you, and users' rights.
- **Respect data subject rights**: users can be informed, access, correct, object, have data erased or blocked, port their data, and complain. Build **export my data** and **delete my account** into the product early.
- **Sensitive personal information** (e.g. health, government IDs, and other categories defined in the law) needs stricter handling. Avoid collecting it unless it's essential.
- **Security measures**: encryption in transit and at rest, access control, and logging ([security](../engineering/security.md)).
- **Third parties** (analytics, hosting, payment providers) are processors. Know which ones receive what data, and list them in the privacy notice.
- **Breaches**: a breach of personal data that may cause serious harm generally has to be reported to the NPC and to the affected users within **72 hours** of discovery under NPC rules. Keep a written incident plan.
- **Registration and DPO**: depending on size and processing, an organization may need to designate a Data Protection Officer and register with the NPC. Check the thresholds as the studio grows.

## Kickoff questions

- [ ] What personal data does this collect? Is each item necessary?
- [ ] What's the lawful basis for each?
- [ ] Where is it stored (which region or provider), and who can access it?
- [ ] How long is it kept, and how is it deleted?
- [ ] Can users export and delete their data?
- [ ] Is the privacy notice written and linked in the app or site?
