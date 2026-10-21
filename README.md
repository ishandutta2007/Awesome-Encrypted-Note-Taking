# Awesome-Encrypted-Note-Taking

## Top Encrypted Note Taking Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on End-to-End Encryption, Local-First Storage & Privacy-First Note Management*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Encrypted Note Taking**. These tools enable individuals and organizations to capture, organize, and sync notes with strong encryption guarantees—ensuring that sensitive information remains private even from the service provider itself.



**Examples** include Evernote, Bear, Standard Notes, Joplin Cloud, Notion, Obsidian Sync, Apple Notes (Advanced Data Protection), Simplenote, Microsoft OneNote, and Google Keep (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom sync backends, and transparent encryption implementations—ideal for privacy advocates, developers, and organizations that prioritize data sovereignty. The open-source encrypted notes landscape is anchored by **Standard Notes** (the leading E2EE note app), with strong contenders in **Joplin**, **Notesnook**, **Memos**, and **Trilium**.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Evernote](https://evernote.com/)**  

  The long-standing note-taking standard with client-side encryption for individual text selections and attachments. Encryption is applied manually to selected content, requiring a passphrase for decryption; encrypted content cannot be edited in real-time without first decrypting . Free plan is severely limited (50 notes, 1 notebook, 1 device).



- **[Bear](https://bear.app/)**  

  macOS/iOS Markdown notes app with Bear Pro unlocking iCloud sync and the ability to encrypt individual notes and lock the app . No end-to-end encryption for sync itself—encryption is per-note and optional.



- **[Standard Notes (Cloud)](https://standardnotes.com/)**  

  Privacy-first note app with end-to-end encryption enabled by default on all plans, including free. Free tier includes unlimited devices, plain-text notes, tags, and offline access; paid plans unlock Markdown, rich text, and other editors . The entire app is open-source, with the cloud tier as the hosted convenience option.



- **[Joplin Cloud](https://joplinapp.org/cloud/)**  

  Hosted sync and sharing service for the open-source Joplin app, with end-to-end encryption available in settings. Notes are encrypted before leaving the device and can only be decrypted with the master password . Free tier available with paid plans for more storage and features.



- **[Obsidian Sync](https://obsidian.md/sync)**  

  Paid sync add-on for Obsidian with end-to-end encryption (default) or standard encryption. E2EE uses AES-256-GCM with scrypt key derivation; Obsidian cannot access encrypted vault data . Local vaults are never encrypted by the app itself.



- **[Apple Notes (Advanced Data Protection)](https://support.apple.com/en-au/102651)**  

  Apple's built-in notes app gains end-to-end encryption for note content when Advanced Data Protection is enabled on the Apple ID. Without ADP, notes are encrypted in transit and at rest but Apple holds the keys .



- **[Simplenote](https://simplenote.com/)**  

  Free, cross-platform notes app owned by Automattic. Client apps are open-source, but the server is proprietary. Supports Markdown, tags, version history, and publishing. No end-to-end encryption—data is encrypted in transit and at rest on Automattic's servers .



- **[Notion](https://www.notion.com/)**  

  Workspace and notes platform with encryption in transit (TLS 1.2+) and at rest (AES-256), but **no end-to-end encryption**. Notion holds the encryption keys, meaning the company can technically access workspace content .



- **[Microsoft OneNote](https://www.microsoft.com/en-us/microsoft-365/onenote)**  

  Microsoft's note-taking app with password protection for individual sections, but not full notebook encryption. Syncs via OneDrive, where data is encrypted at rest by Microsoft—not end-to-end encrypted .



- **[Google Keep](https://keep.google.com/)**  

  Google's lightweight notes app with encryption in transit and at rest on Google's servers. No end-to-end encryption option; Google holds the keys. Best for casual, non-sensitive notes.



## Open-Source GitHub Projects



- **[Standard Notes](https://github.com/standardnotes/app)**  

  The leading open-source E2EE note-taking application. Uses XChaCha-20 encryption, with all client code auditable. Free tier includes unlimited devices, offline access, tags, and passcode/fingerprint lock. Paid tiers unlock advanced editors (Markdown, rich text, code, spreadsheet) and web clipping . The server is also open-source for self-hosting. Best for users who want encryption-by-default with a polished cross-platform experience.



- **[Joplin](https://github.com/laurent22/joplin)**  

  Open-source Markdown note-taking app with optional end-to-end encryption for sync. Notes are stored as plain Markdown files locally; E2EE encrypts them before they leave the device . Sync via Joplin Cloud, Dropbox, OneDrive, or self-hosted Nextcloud/WebDAV. Desktop client can be slow on older hardware, and search performance degrades with very large libraries . Best for Markdown users who want local-first control with optional cloud sync.



- **[Notesnook](https://github.com/streetwriters/notesnook)**  

  Privacy-focused, feature-rich E2EE note app with zero-knowledge architecture. Free plan includes unlimited devices, 50MB monthly storage, 50 notebooks, and 50 tags—more generous than most competitors . Rich-text editor supports checklists, headings, code snippets, colored text, and math formulas. Also offers a self-hostable sync server. Best for users who want Evernote-like features with strong encryption.



- **[Memos](https://github.com/usememos/memos)**  

  Self-hosted, lightweight note-taking app built around a private timeline. Write in Markdown, skip folder hierarchies, and keep all data on your own server. 63k+ stars. MIT licensed . Not E2EE by default—encryption depends on your server setup—but ideal for users who want full infrastructure control.



- **[Trilium](https://github.com/zadam/trilium)**  

  Hierarchical note-taking app with strong organization features, scripting, and self-hosting. While not strictly E2EE out of the box, it can be deployed on encrypted infrastructure for full data control. Popular among users who want a private, self-managed knowledge base .



- **[Logseq](https://github.com/logseq/logseq)**  

  Open-source, local-first outliner with bidirectional links, block references, and daily journals. Free and open-source; sync via Git or third-party services. Not E2EE by default, but local-first architecture means you control the files. Best for outliner-style thinkers and journalers .



- **[Obsidian](https://github.com/obsidianmd/obsidian-releases)**  

  Free for personal use, local-first Markdown editor with a massive plugin ecosystem. Core is closed-source, but the app is listed here because it's a dominant local-first alternative often paired with encrypted sync solutions. Obsidian Sync offers E2EE as an optional paid add-on . Local vaults are plain files—encryption requires third-party tools (e.g., encrypted disk volumes).



### Additional Strong Open-Source Options



- **Simplenote (clients)** — The desktop and mobile clients are open-source, but the server remains proprietary. Not recommended for sensitive data .

- **OpenNotas** — Multi-platform, E2EE note app with simplicity, sync, and offline support .

- **Justnote** — Secure note app with sync and full data control, GPL-2.0 licensed .

- **Frameworks for building custom systems**: Pair **Standard Notes** (self-hosted server) with its open-source clients for full E2EE control. Use **Joplin** with self-hosted Nextcloud for Markdown-based E2EE sync. For timeline-style notes, self-host **Memos** behind a VPN or encrypted reverse proxy.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- "Encrypted" is not synonymous with "end-to-end encrypted." Verify whether the provider holds decryption keys before trusting sensitive data.

- Self-hosted open-source solutions require proper server hardening, backup encryption, and key management practices.



---



**Made for privacy advocates, developers, researchers, and anyone who believes their notes should remain theirs alone.**  

Let's make encrypted note-taking more open, auditable, and accessible.
