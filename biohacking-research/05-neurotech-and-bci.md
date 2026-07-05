# 05 — Neurotech & Brain-Computer Interfaces

## What it is

Neurotech spans everything that reads from or writes to the nervous system electrically, and it splits along two axes that matter more than the "biohacking" label: **invasive vs. non-invasive**, and **clinical/well-funded vs. DIY/open-source**.

**Reading (recording).** Non-invasive EEG (electrodes on the scalp) is cheap, safe, low-resolution, and noisy — good for coarse states (relaxation, some motor imagery, P300/SSVEP paradigms), bad for the high-bandwidth "type with your mind" dreams. Invasive recording (electrodes on or in the cortex — ECoG, Utah arrays, stentrode) gives dramatically better signal and is the basis of the serious clinical BCI results: paralyzed patients moving cursors, robotic arms, and (recently) speech decoding at usable rates. The gap between consumer EEG and implanted BCI is enormous — conflating them is the field's central category error.

**Writing (stimulation).** Non-invasive neuromodulation includes **tDCS** (transcranial direct-current stimulation — weak DC current, popular in DIY because it's buildable from a 9V battery and electrodes) and **tACS/TMS**. tDCS is the DIY-neurohacking flagship: cheap, does *something* measurable to cortical excitability, and is surrounded by wildly overstated claims about cognitive enhancement. The evidence is genuinely mixed — real neuromodulatory effects exist, but reliable, meaningful cognitive-enhancement results in healthy people are weak, inconsistent, and heavily publication-biased. Invasive stimulation (deep brain stimulation, DBS) is established clinical medicine for Parkinson's, tremor, and some psychiatric indications — the mature, evidenced end of "writing to the brain."

The scene therefore contains, simultaneously: genuinely revolutionary clinical science (implanted BCI restoring function to paralyzed people), a serious open-source hardware community (OpenBCI) doing legitimate research-grade work on a budget, a heavily VC-funded private BCI race (Neuralink, Synchron, others), a consumer-EEG wellness market (Muse and similar) that is mostly meditation-feedback, and a DIY tDCS fringe running current through their own heads on thin evidence. Evaluate the specific project; the category tells you almost nothing.

## Key figures

- **Elon Musk / Neuralink team** — Neuralink is the highest-profile invasive-BCI company; high-bandwidth implanted electrode arrays + surgical robot; began human implants (first reported 2024). Musk is the promoter; the science is done by a large team. Real progress, heavy hype — hold both. [verify latest trial status]
- **Thomas Oxley** — neurologist, founder/CEO of Synchron; developed the "Stentrode," a BCI delivered via the vasculature (no open-brain surgery), in human trials. Often cited as the more clinically pragmatic invasive approach. Active. [verify trial status]
- **Conor Russomanno** — co-founder/CEO of OpenBCI; the central figure of the open-source neurotech community. Active. [primary, open-source wing]
- **Joel Murphy** — OpenBCI co-founder (hardware). [verify]
- **Bryan Johnson** — founded Kernel (non-invasive neuroimaging headsets, e.g. Flow/Flux) before/alongside his longevity venture; represents the well-funded non-invasive-imaging bet. Also `07`. [verify Kernel's current status; commerce-adjacent]
- **Miguel Nicolelis** — pioneering academic BCI researcher (Duke); primate and human BCI, exoskeleton work; foundational figure. [primary, academic]
- **Leigh Hochberg / BrainGate consortium** — academic implanted-BCI research (Utah arrays; cursor, robotic-arm, and speech-decoding milestones in paralyzed patients). The rigorous clinical-academic backbone. [primary, academic]
- **Marom Bikson** — academic authority on tDCS/tES dosing and safety; the person to read to calibrate DIY-tDCS claims against evidence. [primary, academic]

## Key organizations / projects

- **OpenBCI** — open-source EEG/EMG/ECG hardware + software (Cyton, Ganglion boards; Galea headset combining EEG with other sensors). The legitimate DIY/research bridge. https://openbci.com [primary, open-source; sells hardware — light commerce]
- **Neuralink** — invasive high-bandwidth BCI + surgical robot. https://neuralink.com [private, commerce/venture]
- **Synchron** — endovascular "Stentrode" BCI. https://synchron.com [private]
- **Blackrock Neurotech** — makes the Utah array and much of the implanted-electrode hardware used in academic BCI (BrainGate); the quiet incumbent behind many milestones. https://blackrockneurotech.com [verify]
- **Kernel** — non-invasive functional neuroimaging headsets (Flow/Flux). https://www.kernel.com [verify current status; commerce]
- **Muse (InteraXon)** — consumer EEG headband for meditation/neurofeedback; the mainstream consumer-EEG product. https://choosemuse.com [commerce]
- **BrainGate** — academic research consortium (Brown, MGH, Stanford, others) for implanted BCI in paralysis. https://www.braingate.org [primary, academic]
- **Emotiv / NeuroSky** — earlier consumer-EEG companies; historical context for the consumer wave. [verify current status; commerce]
- DIY tDCS communities (historically r/tDCS and DIY forums) — the amateur neuromodulation scene; approach critically. [verify current activity]

## Foundational reading / viewing

Primary first:
- **BrainGate publications** (Hochberg et al., *Nature* 2006 cursor control; 2012 robotic-arm; recent high-rate speech-decoding papers, 2021–2023) — the rigorous clinical record of what implanted BCI actually achieves. [primary, note dates]
- **Neuralink / Synchron peer-reviewed publications and trial registrations** — read the papers/registrations, not the press. [primary — verify specific citations]
- **OpenBCI documentation & community** — primary technical reference for accessible neurotech. [primary]
- **Marom Bikson et al., tDCS safety/dosing reviews** — primary calibration on neuromodulation claims. [primary]
- **Cochrane / large meta-analyses on tDCS for cognition** — the antidote to enhancement hype. [primary/secondary — verify current reviews]

Secondary:
- **Miguel Nicolelis, *Beyond Boundaries* (2011)** — accessible history/vision from a pioneer. [primary-ish, note date]
- Journalism on Neuralink (MIT Tech Review, *Wired*, STAT News) — for hype-vs-reality calibration; STAT News is unusually good on neurotech. [secondary]
- **IEEE Brain / Neuroethics literature** — for the policy layer (see `08`). [secondary]

## Current state (2026)

The most exciting *and* most hype-prone scene here. **Invasive clinical BCI is having real, non-hype breakthroughs** — speech decoding for paralyzed/locked-in patients has moved from proof-of-concept toward genuinely usable communication rates, and multiple companies (Neuralink, Synchron, plus academic BrainGate) have humans implanted. This is legitimate, historic science. Treat the *clinical results* as real and the *timeline-to-consumer / "merge with AI"* promotion as marketing. [verify latest per-company trial milestones — this field moves fast and specifics date quickly.]

**Non-invasive consumer neurotech (Muse-class EEG)** is a stable, modest wellness/meditation market — real biofeedback, limited scope, don't expect cognition boosts. **DIY tDCS** persists but the enthusiasm has cooled as meta-analyses failed to support the strong enhancement claims. **OpenBCI** remains the healthiest part of the accessible/DIY end — genuinely useful for research, art, and learning.

## Red flags / caveats

- **Consumer EEG ≠ implanted BCI.** The single biggest error. A $300 headband reads coarse scalp signals; it cannot do what a cortical implant does. Marketing frequently borrows the implant's glamour for the headband's capabilities.
- **tDCS enhancement claims are weakly supported.** Real neuromodulation, unreliable cognitive benefit, meaningful safety caveats (burns, montage errors, unknown long-term effects of chronic DIY use). Read Bikson and the meta-analyses before believing a forum protocol.
- **Neuralink-style hype.** Separate the peer-reviewed result from the "telepathy / AI symbiosis" framing. The former is impressive; the latter is promotion.
- **Neuro-privacy is the sleeper issue.** Even coarse neural/biometric data is sensitive; consumer neurotech's data practices are under-scrutinized (see `08`, and emerging "neurorights" law).
- **`[commerce]`** on Muse, Kernel, Emotiv/NeuroSky, and OpenBCI hardware sales — though OpenBCI's open-source posture makes it the least concerning.
- **Surgical/venture risk** on the invasive companies — implanted-device longevity, vendor-dependence, and reversibility concerns mirror `03`/`04`.

## Adjacent scenes
- **`03` Sensory augmentation** — BCIs that restore/augment perception overlap directly.
- **`04` Medical device security** — implanted BCIs are attack surface; that discipline applies.
- **`02` Grinders** — the far DIY edge (Warwick's neural implant) touches here.
- **`07` Longevity** — shared figures (Bryan Johnson/Kernel) and "optimize the brain" framing.
- **`08` Ethics/policy** — neurorights, neuro-privacy, enhancement equity.
- **`00`** — why neurotech is the most bimodal scene.
