# 00 — What "Biohacking" Actually Means

"Biohacking" is a marketing-grade umbrella term. It has no single referent. It gets applied to a molecular biologist editing bacteria in a garage, a Silicon Valley executive drinking butter coffee, a person with a magnet in their fingertip, and a security researcher exploiting an insulin pump — activities that share almost nothing except a rhetorical posture of "individuals taking biology into their own hands."

Treat the word as a pointer that must be dereferenced. Below are the distinct scenes it points to. They differ on the axes that matter: **substrate** (whose body/organism), **tooling** (wet lab vs. wearable vs. code), **evidence culture** (peer review vs. n=1 vs. engineering test), **risk owner** (self, third parties, patients), and **commercial gravity** (how much of the scene is a sales funnel).

## The six-plus scenes

### 1. DIY bio / citizen science → `01`
Community wet labs, at-home molecular biology, open-source lab equipment, amateur genetic engineering. Substrate: microbes, plants, cell-free systems, occasionally the practitioner. Culture: descends from hacker/maker ethos applied to molecular biology; strong open-source and biosafety-norms streak. Evidence culture: closest to actual science; overlaps with academia and iGEM. Commercial gravity: low-to-moderate (some kit vendors).

### 2. Grinders / implantables → `02`
People who put hardware under their skin: RFID/NFC chips, magnets, subdermal LEDs, sensors. Substrate: the practitioner's own body, permanently. Culture: body-modification scene meets electronics hobbyism; DIY, anti-medical-gatekeeping, high pain tolerance for both senses of the word. Evidence culture: engineering + lived experiment, minimal formal study. Commercial gravity: low, a few specialist vendors.

### 3. Sensory augmentation → `03`
Extending existing senses or adding new ones: color-to-sound for the colorblind, magnetic-field sensing, infrared/ultrasound perception, haptic sensory substitution. Substrate: the nervous system, via implants or wearables. Culture: overlaps grinders (DIY end) and academic neuroscience/HCI (research end) and art (cyborg-art end). Commercial gravity: low-to-moderate (a few devices).

### 4. Medical device security → `04`
Security research on implanted and connected medical devices — pacemakers, insulin pumps, infusion pumps, ICDs. Substrate: patients (third parties), not the researcher. Culture: infosec — vuln research, coordinated disclosure, regulation. This is the corner where "hacking" is literal and the stakes are someone else's life. Evidence culture: rigorous, adversarial, engineering. Commercial gravity: low; adjacent to a medical-device industry and regulators.

### 5. Neurotech / BCI → `05`
Brain-computer interfaces, EEG, neurostimulation (tDCS/tACS), both invasive (implanted electrodes) and non-invasive (headsets). Substrate: the brain — self (consumer EEG, DIY tDCS) or patients (implanted clinical BCI). Culture: splits sharply between well-funded private clinical ventures and open-source/DIY communities. Evidence culture: bimodal — serious clinical trials on one end, dorm-room electrode montages on the other. Commercial gravity: high on the consumer end.

### 6. Quantified self / wellness → `06`
Self-tracking and optimization: wearables, sleep tracking, continuous glucose monitors on non-diabetics, HRV, "n=1 experiments." Substrate: self, non-invasively. Culture: originated as a genuine measurement/curiosity movement; has been largely absorbed by the wellness-optimization market. Evidence culture: n=1, self-report, occasional rigor. **Commercial gravity: very high.** This is where "biohacking" most often means "things sold to you."

### 6b. Longevity / nootropics → `07`
Life extension and cognitive enhancement. Splits hard into two: (a) legitimate aging biology (senescence, mTOR, cellular reprogramming) done in labs, and (b) a supplement/protocol/influencer market that borrows (a)'s vocabulary. Substrate: self. **Commercial gravity: very high** on the (b) side. Broken out from QS because the science-vs-marketing gap is the whole story.

### Cross-cutting: ethics & policy → `08`
Not a scene but a layer over all of them — bioethics, regulation, transhumanism, consent, equity of access. Transhumanism in particular is the ideological substrate that ties implantables, sensory augmentation, neurotech, and longevity into a single "human enhancement" narrative, even though the practitioners often don't overlap.

## Overlap map

Where the scenes genuinely touch:

- **Grinders ↔ Sensory augmentation** — heaviest overlap. The DIY end of sensory augmentation (implanted magnets to "feel" magnetic fields, implanted compasses) *is* grinder practice. Diverges at the research/academic end (Eagleman-style wearables, clinical sensory substitution).
- **Grinders ↔ Medical device security** — shared "implanted electronics" substrate and shared skepticism of medical gatekeeping, but opposite risk models: grinders accept risk on their own bodies; med-device security defends third-party patients. Culturally adjacent (overlapping communities), technically distinct.
- **Neurotech ↔ Sensory augmentation** — both interface with the nervous system; BCIs that restore/augment perception sit in both.
- **Neurotech ↔ Medical device security** — implanted BCIs are medical devices with attack surface; the security discipline extends to them.
- **DIY bio ↔ Longevity** — DIY-bio practitioners occasionally self-experiment with longevity interventions (gene therapy self-trials), bridging the community-science scene and the life-extension scene. This is the most controversial bridge (see Zayner, `01`/`07`).
- **QS ↔ Longevity** — shared self-tracking tooling and shared consumer market; the "measure everything to live longer/better" pitch spans both.
- **Transhumanism (`08`) ↔ everything** — the connective ideology, strongest link to implantables, neurotech, and longevity.

## Where they *don't* overlap

- **DIY bio vs. QS/wellness** — near-orthogonal. Editing a plasmid in a community lab has essentially nothing in common with tracking your sleep, despite both being "biohacking." Different substrate, tooling, culture, evidence standard. Collapsing them is the single most common category error.
- **Medical device security vs. wellness** — opposite in almost every dimension: third-party risk vs. self; adversarial engineering vs. self-optimization; near-zero commerce vs. near-total commerce. They share the word and nothing else.
- **DIY bio vs. grinders** — both DIY, but wet (molecular) vs. dry (electronics under skin). Different skills, different labs, different failure modes.

## Practical read

If you're evaluating "is biohacking worth engaging with," the honest answer is that you're really evaluating six different questions. The scenes with the highest signal for a security-minded engineer are **medical device security** (`04`, literally your field), **DIY bio** (`01`, real science, real community), and **grinders/implantables** (`02`, genuine engineering subculture). The scenes with the lowest signal-to-noise are the **wellness** (`06`) and **nootropics-marketing** (`07`) ends, where the term is mostly a sales layer. Neurotech (`05`) is bimodal — evaluate the specific project, not the category.

## Adjacent scenes
- Everything downstream: `01`–`08`
- Index of who's who: `09`
- What to read to go deeper: `10`
