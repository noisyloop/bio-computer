# 04 — Medical Device Security

## What it is

This is the corner where "hacking" is literal and the stakes are highest, because the risk owner is a third party — a patient — not the researcher. Medical device security is the vulnerability research, exploitation, and coordinated-disclosure discipline applied to implanted and connected medical devices: cardiac pacemakers and implantable cardioverter-defibrillators (ICDs), insulin pumps, infusion pumps, patient monitors, and the increasingly networked hospital device fleet. It is a subfield of infosec, not of wellness, and it is arguably the highest-signal "biohacking" scene for a security engineer because it *is* security engineering.

The field was catalyzed by two lines of work. Academically, the 2008 Halperin et al. paper demonstrating radio attacks on an implantable defibrillator (a Medtronic ICD) established that these devices had exploitable wireless attack surface. Publicly, **Barnaby Jack**'s demonstrations (~2011–2013) — wirelessly compromising insulin pumps and later pacemakers, including the ability to deliver a lethal shock or dump insulin — made the threat visceral and forced the industry and regulators to engage. The through-line since has been a maturing coordinated-disclosure ecosystem: researchers finding flaws, a rocky early history of vendor denial and legal threat, and gradual movement toward structured vulnerability handling, ISAOs, and regulator involvement.

The regulatory layer is now central. The **FDA** has issued premarket and postmarket cybersecurity guidance and, via the 2022/2023 statutory changes (the "cyber devices" authority added to the FD&C Act, section 524B), can now require security documentation (including an SBOM and a plan to monitor/patch) as a condition of clearance. This makes medical device security one of the few biohacking-adjacent scenes with hard regulatory teeth and a real compliance industry around it. The tension the field manages: connectivity and remote monitoring genuinely improve care, and every added interface is attack surface on a life-sustaining device that may be implanted for a decade and cannot be easily patched.

## Key figures

- **Barnaby Jack** — (deceased, 2013) the field's most famous figure; demonstrated wireless insulin-pump and pacemaker attacks that could be lethal; his work (and death, days before a planned talk) is the field's origin myth and its ethics touchstone. [primary historical]
- **Jay Radcliffe** — security researcher and Type 1 diabetic who publicly demonstrated attacks on his own insulin pump (~2011); notable for researching a device he personally depended on, which sharpened the ethics conversation. Active in the space. [verify current role]
- **Marie Moe** — security researcher with an implanted pacemaker; "hacking my heartbeat" research examining the security and reliability of her own life-sustaining implant; strong voice for patient perspective + transparency. [verify current role]
- **Billy Rios** — prolific medical-device (and ICS) vulnerability researcher; extensive work on infusion pumps and hospital devices; co-founder of security firms in the space; pushed FDA/industry engagement. [verify current affiliation]
- **Jonathan Butts** — researcher (WhiteScope, with Rios); co-authored pacemaker/implant vulnerability research and a notable Medtronic disclosure; part of the coordinated-disclosure fights that shaped norms. [verify current affiliation]
- **Kevin Fu** — academic (co-author of the 2008 ICD paper; UMich/Northeastern); later served as the FDA's first Acting Director of Medical Device Cybersecurity; the key academic-to-regulator bridge. [verify current role]
- **Beau Woods / Josh Corman** — "I Am The Cavalry" movement; advocacy connecting security research to public safety (medical, auto, etc.); drove the Hippocratic Oath for Connected Medical Devices and disclosure-norms advocacy. [verify current roles]
- **Suzanne Schwartz** — FDA official long associated with the agency's medical-device cybersecurity program; the regulator-side face. [verify current role]

## Key organizations / projects

- **U.S. FDA — medical device cybersecurity program** — premarket & postmarket guidance; section 524B "cyber devices" authority. Start point: FDA's medical device cybersecurity pages. https://www.fda.gov (search "medical device cybersecurity") [primary, regulatory]
- **I Am The Cavalry** — grassroots safety-research advocacy group (medical, automotive, ICS). https://iamthecavalry.org [primary, advocacy]
- **Health-ISAC (H-ISAC)** — health-sector information sharing & analysis center; the coordination body for threat/vuln sharing in healthcare. https://h-isac.org
- **MDIC (Medical Device Innovation Consortium)** — public-private consortium with medical-device cybersecurity workstreams. [verify]
- **CISA / ICS-CERT advisories** — publish medical device vulnerability advisories (many devices are handled as ICS). https://www.cisa.gov [primary, advisories]
- **Archimedes Center for Medical Device Security** (Kevin Fu-associated) — academic center + training. [verify current status]
- **MITRE** — authored medical-device cybersecurity playbooks/regional incident-prep guidance for the FDA. [verify]

## Foundational reading / viewing

Primary first:
- **Halperin et al., "Pacemakers and Implantable Cardiac Defibrillators: Software Radio Attacks and Zero-Power Defenses" (IEEE S&P, 2008)** — the founding academic paper. [primary, note date]
- **FDA guidance documents**: "Cybersecurity in Medical Devices: Quality System Considerations and Content of Premarket Submissions" (2023) and postmarket management guidance (2016). [primary, regulatory — note dates/versions]
- **Section 524B, FD&C Act** (added by the 2022 Consolidated Appropriations Act / "PATCH Act" provisions) — the statutory cyber-device requirement. [primary, note date]
- **Barnaby Jack's public talks & demonstrations (~2011–2013)** — primary demonstrations (recordings/writeups survive). [primary historical]
- **Marie Moe, "Unpatchable" / talks on her own pacemaker** — primary patient-researcher account. [primary]
- **Jay Radcliffe's insulin-pump research writeups (2011+)** — primary. [primary]

Secondary:
- **I Am The Cavalry, "Hippocratic Oath for Connected Medical Devices"** — a norms document (arguably primary advocacy). [primary/advocacy]
- Journalism on the Medtronic/St. Jude (Abbott) pacemaker disclosure fights (~2016–2018), including the MedSec/Muddy Waters short-selling episode — a genuinely instructive case in disclosure ethics gone sideways. [secondary, note dates]
- MIT Tech Review / *Wired* profiles of Barnaby Jack and the field. [secondary]

## Current state (2026)

Mature, institutionalized, and regulator-driven — the most "grown up" scene in this whole KB. The FDA's 524B authority (in force since 2023) means new connected devices must arrive with a security posture (SBOM, patch/monitoring plans), which has pulled the industry from denial toward baseline hygiene. Coordinated disclosure is now normal rather than adversarial in most cases, though frictions remain. There's a real professional field here — vendors, consultancies, ISACs, academic centers, and a dedicated research literature.

Live threads in 2026: legacy/long-lived implanted devices that can't be patched but are still in bodies for years; the expanding hospital IoT/IoMT attack surface (networked pumps, monitors, imaging); ransomware against hospitals as a patient-safety issue; and SBOM/software-supply-chain requirements maturing. This is the biohacking corner most worth a security engineer's serious attention — the skills transfer directly and the mission is unambiguously defensive.

## Red flags / caveats

- **Disclosure ethics are genuinely hard here.** The St. Jude/Muddy Waters episode (researchers partnering with a short-seller to profit from a vulnerability disclosure) is the cautionary example: even "true" findings can be delivered in ways that harm patients and the field's credibility. Judge disclosures on process, not just correctness.
- **Threat inflation vs. real risk.** Targeted assassination-via-pacemaker makes headlines but is a low-probability, high-effort attack; the higher-expected-value risks are systemic (hospital ransomware, mass device flaws, unpatched fleets). Don't let the dramatic framing crowd out the boring, likelier harms.
- **"Researcher on their own device" ≠ generalizable.** Radcliffe/Moe self-research is ethically clean but n=1; vendor-scale claims need vendor-scale evidence.
- **Regulatory ≠ solved.** 524B applies going forward; the installed base of legacy devices predates it and remains exposed.
- **Access/testing legality** — attacking devices you don't own, or in ways that risk patients, is both illegal and unethical; this field runs on responsible, authorized research.

## Adjacent scenes
- **`02` Grinders** — shares implanted-electronics curiosity and anti-gatekeeping culture; opposite risk owner (self vs. patient).
- **`05` Neurotech** — implanted BCIs are medical devices with attack surface; this discipline extends to them.
- **`06` QS/wellness** — consumer health wearables sit in a lighter-regulation gray zone with their own (privacy-heavy) security issues.
- **`08` Ethics/policy** — disclosure ethics, regulation, patient consent and safety.
- **`00`** — why this scene shares only the word with the wellness corners.
