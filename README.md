# CyberFlow — Cyberrange Attack Flowchart

**Live demo:** [https://mohitmohanty.github.io/cyberflow/](https://mohitmohanty.github.io/cyberflow/)

---

## Overview

**CyberFlow** is an educational visualization that maps the stages of a realistic attack lifecycle in a cyberrange scenario. The site presents a flowchart that illustrates how an adversary might progress from initial reconnaissance through delivery, exploitation, persistence, and actions on objective — and how defender tooling (shown with **Wazuh** File Integrity Monitoring and prevention controls) fits into the detection/response cycle.

This repository contains the website content and supporting documentation for instructors, red/blue teamers, and security engineers who want a clear, high-level representation of attack stages for training, tabletop exercises, or curriculum material.

---

## Purpose & learning goals

* Communicate the **attack lifecycle** in a single, easy-to-follow flowchart.
* Show the interplay between attack actions and *defensive* monitoring (file integrity checks, alerting, and prevention).
* Support cyberrange scenarios and classroom/train-the-trainer materials without sharing operational, harmful details.
* Encourage responsible, legal hands-on practice in isolated labs only.

---

## High-level flow (conceptual)

> Note: This is a conceptual overview to be used for training and defensive planning. It intentionally omits operational instructions that could enable wrongdoing.

1. **Reconnaissance** — Attacker gathers information about targets (public-facing services, users, and assets).
2. **Weaponization (conceptual)** — Adversary prepares an artifact intended to trick a user (illustrated in the site as a document-like container carrying a malicious executable).
3. **Delivery** — The artifact is delivered to the target (conceptually represented by phishing-style lures / malicious links).
4. **Exploitation & Execution (conceptual)** — The delivered artifact is executed on the target system, allowing the attacker to run code.
5. **Persistence & Post-exploitation** — Attacker attempts to maintain access and move laterally.
6. **Actions on Objective** — Data theft, disruption, or other attacker goals.
7. **Detection & Response (Wazuh shown)** — File Integrity Monitoring (FIM), rule-based detection, alerting, and automated prevention close the loop — illustrating how defenders can observe and respond.
8. **Continuous cycle** — Logging, lessons learned, and tuning of detections feed back into improved defenses.

---

## What this repository contains

* Static website (HTML/CSS/JS) for the CyberFlow visualization.
* Flowchart assets and labels used on the site.
* README (this file) with usage notes and contributor guidance.
* (No attack tooling, scripts, or payloads are included — by design.)

---

## How to use the site

* **Presentations / Teaching:** Use the flowchart pages during lectures or walkthroughs to explain each conceptual stage and where controls should be placed.
* **Red/Blue Exercises:** Use the flowchart as a planning artifact when designing exercise objectives and detection telemetry collection requirements.
* **Detection Mapping:** Map Wazuh alerts, FIM events, and endpoint telemetry to each stage to decide which controls cover which attacker behaviors.

---

## Responsible use & legal notice

This project is explicitly educational and defensive in purpose. It describes attacker *concepts* at a high level to support awareness and detection planning. It **does not** provide step-by-step instructions for creating malware, embedding executables in documents, constructing phishing sites, or carrying out exploits.

**Do not** use these materials to plan, commit, or assist in unlawful or harmful activities. If you wish to perform hands-on testing, do so only in:

* Properly authorized environments (owned lab infrastructure or an organization’s designated test range), and
* Isolated networks with no access to production or the public internet, and
* Under explicit written permission and applicable laws/regulations.

---

## Recommended defensive resources

(For learning detection and monitoring techniques — not for offensive use.)

* Wazuh documentation and FIM best practices (use vendor docs and official guides).
* Endpoint detection & response (EDR) vendor resources and telemetry mapping guides.
* SANS/OWASP/other reputable training resources for defensive posture and secure configurations.

---

## Contributing

Contributions are welcome if they keep the repository focused on education, detection, and defensive guidance.

* Suggested contributions: clearer labels, improved flowchart descriptions, additional defender-mapping examples (e.g., which logs to collect at each stage), accessibility improvements, or translated content.
* Please open pull requests with clear descriptions and avoid adding offensive/operational content.

---

## License

Choose an appropriate open-source license for this repository (e.g., MIT, Apache 2.0). If you want, I can add a license file for you.

---

## Contact / Author

Created and maintained by Mohit Mohanty.
Live site: [https://mohitmohanty.github.io/cyberflow/](https://mohitmohanty.github.io/cyberflow/)


