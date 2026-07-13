# My SC-300: Microsoft Identity & Access Administrator Notes

Welcome! This repository is my personal, no-nonsense study guide for the **SC-300 exam**. Instead of overwhelming corporate jargon, I’ve broken down Microsoft Entra ID concepts into practical, detailed notes that read like they were written by a peer, not a textbook.

Whether you are studying for the exam or just trying to configure Entra ID without pulling your hair out, I hope this helps!

---

## What's Inside?

*   **[01. Initial Configuration](./01-initial-configuration/)**
    *   Setting up tenants, custom company branding, and primary domains.  
    *   Understanding Global vs. User vs. Billing Administrator roles.
    *   Delegating control using Administrative Units (OUs for the cloud).
*   **[02. Identity Management](./02-identity-management/)**
    *   Managing Cloud vs. Synced vs. Guest user types. 
    *   Dynamic Groups (automating access based on department or title).
    *   Device registration breakdowns (Entra Registered vs. Entra Joined vs. Hybrid).
*   **[03. External Identities](./03-external-identities/)**
    *   B2B collaboration and the guest user redemption flow.
    *   Setting up Google and Facebook as external Social Identity Providers.
    *   Cross-tenant access controls and B2B Direct Connect for Teams.
*   **[04. Hybrid Identity](./04-hybrid-identity/)**
    *   Deep dive into Microsoft Entra Connect.
    *   Choosing your authentication: Password Hash Sync (PHS) vs. Pass-Through Authentication (PTA) vs. Federation.
    *   Setting up Seamless Single Sign-On (SSO).

---

## 💡 Quick Tips for Navigating These Notes

>  **The Principle of Least Privilege:** If there is one recurring theme in this exam, it’s this—never give a user more access than they absolutely need. If a user only needs to reset passwords, give them the *Helpdesk Administrator* role, not *Global Administrator*.

>  **PHS is King for Backup:** Even if an organization insists on using Pass-Through Authentication (PTA) or Federation for compliance, Microsoft still recommends syncing password hashes as a disaster recovery backup. If the on-premises servers go dark, PHS can keep your cloud users working.

---

## 🛠️ Prerequisites Before You Lab
To get the most out of these notes, I highly recommend signing up for a **Free Azure Trial Account** and activating a trial of **Microsoft Entra ID Premium P2**. Features like Privileged Identity Management (PIM), Dynamic Groups, and Company Branding require premium licensing to test!
