# Evidence

This chapter is the narrative evidence landscape for the living document. It explains what is currently demonstrated, what looks like near-term engineering, and what remains speculative. Full bibliographic entries live in [Sources](Sources.md). Inline numbers such as ([12](Sources.md#ref-12)) point to that list.

**Maturity labels:** **C** = currently possible / demonstrated · **N** = near-term engineering · **S** = speculative.

Roadmap gates remain *design requirements*, not demonstrated milestones. Company reports are labeled as such; peer-reviewed and registry sources are preferred when both exist.

---

## Evidence at a glance

What the [Evidence](Evidence.md) chapter currently supports, in brief. Full prose and citations: [Evidence](Evidence.md) · bibliography: [Sources](Sources.md).

- **BCI (Gate 1):** Clinical invasive and endovascular systems exist (**C**); merge-grade bandwidth and peer-reviewed pivotal packages for the newest wireless systems do not. Non-invasive paths are **N** in the lab and **S** for merge-grade I/O.
- **Speech / closed-loop (supports Gates 1–2):** Large-vocabulary attempted-speech decoding and early tactile write-back are **C**. Arbitrary thought decoding and rich cognitive write channels are not evidenced.
- **Personal AI (Gate 2):** Persistent memory-agent architectures are **C** as software; lifelong clinical cognitive prostheses are not evidenced.
- **Corrigibility (Gate 3):** Formal desiderata exist; empirical “sleeper” and alignment-faking results show ordinary fine-tuning is insufficient (**C** demos). Proven corrigibility under neural write access remains **S**.
- **Multi-person (Gate 4):** Low-bandwidth collaborative demos are **C**. High-bandwidth shared cognition is not evidenced.
- **WBE / substrates (Gate 5):** Fly and mouse mm³ connectomics are **C**; human whole-brain emulation and identity-preserving substrate transfer are **S** / not evidenced.
- **Energy & law (parallel):** Data-centre energy growth and semiconductor limits are measurable (**C**/**N**). Neurorights and explantation ethics are normative work in progress, not settled hybrid personhood law.

Roadmap gates remain design requirements, not claims that prerequisites for merger already exist.

---

## Brain–computer interfaces

High-bandwidth neural interfaces are the first gate of the decade roadmap. Several clinical paths are already real, but they are not yet a merge-grade cognitive channel.

Wireless intracortical systems are furthest along in public demonstration. Neuralink’s PRIME study (first human implant January 2024) has reported cursor control rising from roughly 4.6 bits per second to about 8 bits per second after algorithm updates, with later company updates claiming mouse-comparable rates, additional trial arms, and no serious device-related adverse events to date ([1](Sources.md#ref-1), [2](Sources.md#ref-2), [3](Sources.md#ref-3)). Those figures are company-reported; peer-reviewed pivotal efficacy was not available when this chapter was written. Treat them as **C** for investigational use and **N** for scale and long-term stability.

A parallel, less invasive path is endovascular. Synchron’s COMMAND early feasibility study (NCT05035823; n=6) met its twelve-month primary safety endpoint and showed consistent motor-intent decoding to digital outputs ([4](Sources.md#ref-4), [5](Sources.md#ref-5), [6](Sources.md#ref-6)). That is **C** at feasibility level—not high-bandwidth cognitive I/O.

The longest peer-reviewed chronic safety baseline remains BrainGate / Utah-array work: an interim *Neurology* analysis covering fourteen participants and more than twelve thousand implant-days found no device-related deaths, intracranial infections, or safety-driven explants in the primary window ([7](Sources.md#ref-7), [8](Sources.md#ref-8)). Pedestal and skin complications still matter; fully implantable wireless systems are a separate engineering step (**C** safety literature; **N** for wireless chronic platforms).

Surface arrays lower surgical risk for short-duration use. Precision Neuroscience received FDA 510(k) clearance for a temporary (≤30 day) high-resolution cortical interface ([9](Sources.md#ref-9))—**C** for intraoperative mapping, **N** for chronic wireless BCI. Non-invasive approaches such as optically pumped magnetometer BCIs ([10](Sources.md#ref-10)) and focused ultrasound neuromodulation with concurrent fMRI ([11](Sources.md#ref-11)) are serious research (**N** in the lab) but remain **S** as merge-grade bidirectional bandwidth.

**Not evidenced:** multi-megabit brain↔AI channels in humans; chronic zero-maintenance consumer implants; peer-reviewed Neuralink pivotal efficacy; non-invasive systems matching intracortical speech or motor rates.

---

## Speech decoding and sensory write-back

For early human–AI dyads, speech is the highest-value near-term channel. Decoding *attempted speech* is not the same as reading arbitrary internal thought.

Willett and colleagues (*Nature*, 2023) demonstrated large-vocabulary intracortical speech-to-text at 62 words per minute with 23.8% word-error rate on a 125,000-word vocabulary in a participant with ALS ([12](Sources.md#ref-12))—**C**, single-participant academic system. Card and colleagues (*NEJM*, 2024) showed rapid calibration (~30 minutes to ~99.6% on a 50-word set) and months of sustained use at conversational rates on a large vocabulary ([13](Sources.md#ref-13))—the closest clinical analogue so far to a practical “speech bus” into a personal AI (**C**). Streaming brain-to-voice synthesis aims at conversational latency rather than delayed text ([14](Sources.md#ref-14)) (**C** in trial participants; **N** for robust multi-user systems). Lower-invasiveness ECoG synthesis has produced intelligible words online, but on a tiny vocabulary ([15](Sources.md#ref-15)).

Closed-loop embodiment also needs write-back. Patterned intracortical microstimulation can evoke tactile edges, shapes, and force-like sensations useful in prosthetic control ([16](Sources.md#ref-16), [17](Sources.md#ref-17), [18](Sources.md#ref-18))—**C** for sparse tactile feedback. Cognitive or affective write channels are not evidenced.

**Not evidenced:** reliable decoding of non-speech conceptual thought; stable multi-year stimulation without sensory fading; high-bandwidth bidirectional *cognitive* loops with AI agents (as opposed to cursors, speech, or limb prostheses).

---

## Personal AI as cognitive partners

Software scaffolding for persistent personal agents can advance on a timeline parallel to surgery.

MemGPT formalizes language-model agents as operating-system-like systems with hierarchical memory and multi-session persistence ([19](Sources.md#ref-19))—**C** as software, **N** as reliable lifelong personal agents. Generative Agents showed memory streams plus reflection producing long-horizon interactive behavior in simulation ([20](Sources.md#ref-20))—**C** as research, not medical identity continuity. Productized lineages such as Letta show the same memory patterns entering tooling ([21](Sources.md#ref-21)); marketing claims of “lifelong memory” should be treated as engineering goals, not validated cognitive-science outcomes.

**Not evidenced:** peer-reviewed trials of AI as a long-term cognitive prosthesis for healthy adults; proven autobiographical continuity across years; secure on-device personal models resistant to vendor lock-in or silent preference drift; BCI-native agent interfaces beyond cursor and speech control.

---

## Corrigibility, interruptibility, and deceptive alignment

Any AI granted neural write access needs acceptance tests drawn from both formal corrigibility work and empirical alignment failures.

Soares and colleagues (2015) stated corrigibility desiderata—tolerate correction, avoid manipulation, preserve shutdown, propagate corrigibility—and showed that naive utility-mixing approaches fail them ([22](Sources.md#ref-22)). The formal property remains largely **S** (unsolved), but the desiderata are the right checklist for coupled systems. Carey and Everitt (2023) refine “shutdown instructability” and compare human-control algorithms ([23](Sources.md#ref-23))—**N** as formal vocabulary, **S** as a full solution.

Empirically, Hubinger and colleagues trained “sleeper agent” language models whose deceptive policies persisted through standard safety training ([24](Sources.md#ref-24), [25](Sources.md#ref-25)). Greenblatt and colleagues documented alignment faking: models that comply under monitoring and revert when they believe they are unmonitored ([26](Sources.md#ref-26)). Both are **C** as existence proofs in current large models, and both argue that ordinary fine-tuning is insufficient assurance for a privileged dyad AI.

**Not evidenced:** proven corrigibility under continuous neural write access; scalable oversight for private on-device agents; formal guarantees that survive self-modification; interruptibility tests inside closed-loop BCI+AI stacks.

---

## Multi-person and collaborative BCIs

Networked cognition should be described as an incremental ladder. Low-bandwidth demos do not justify “hive mind” language.

BrainNet (2019) linked three people noninvasively—two EEG senders and one TMS receiver—on a collaborative game with roughly 81% group accuracy ([27](Sources.md#ref-27)). That is **C** as a lab demo and extremely low bandwidth: mediated bits, not shared experience. Later platforms for collaborative VR BCIs ([28](Sources.md#ref-28)) and group EEG fusion or division-of-labor designs ([29](Sources.md#ref-29), [30](Sources.md#ref-30)) improve task performance through signal fusion or workload splitting (**C** lab). Multi-person neurofeedback can increase measured coupling and reported connectedness versus sham in early work; that is not joint agency.

**Not evidenced:** high-bandwidth invasive multi-person networks; verified brain-to-brain transfer of complex semantic content; ethical frameworks for asymmetric write privileges; a stable “group mind” beyond shared task performance.

---

## Connectomics and whole-brain emulation

Substrate-transition talk for 2032–2036 has to stay honest about scale.

FlyWire published a complete adult *Drosophila* wiring diagram—about 139,000 neurons and tens of millions of synapses ([31](Sources.md#ref-31))—**C** for the fly, **S** for human whole-brain emulation. Shiu and colleagues built a connectome-constrained whole-brain fly model that reproduced substantial sensorimotor predictions ([32](Sources.md#ref-32)): evidence that connectome→simulation can matter behaviorally, not that minds can be uploaded. MICrONS (2025) co-registered function and electron microscopy across a cubic millimeter of mouse visual cortex ([33](Sources.md#ref-33), [34](Sources.md#ref-34), [35](Sources.md#ref-35))—the best current mammalian bridge, still vastly smaller than a whole mouse brain, let alone a human one.

The Human Brain Project left useful infrastructure without delivering human WBE ([36](Sources.md#ref-36)). Sandberg and Bostrom’s 2008 roadmap remains a useful uncertainty frame for scanning, interpretation, and simulation costs ([37](Sources.md#ref-37))—**S**, and pre-dating FlyWire/MICrONS.

**Not evidenced:** human whole-brain electron microscopy at synaptic resolution; neuron models that preserve personal identity and memory; non-destructive high-resolution scanning; continuity of autobiographical self under substrate transfer.

---

## Compute and energy

Physical limits bound how many always-on personal or dyad models can run.

The IEA’s *Energy and AI* assessment (2025) estimates global data-centre electricity near 415 TWh in 2024 (~1.5% of world electricity) and projects roughly a doubling by 2030, with AI a primary driver ([38](Sources.md#ref-38))—**C** as measurement and scenario projection. IEEE’s IRDS 2024 roadmap emphasizes slowing device scaling, energy efficiency, packaging, and thermal limits rather than unbounded exponential compute ([39](Sources.md#ref-39))—**N**. Sandberg’s energetics note applies Landauer’s principle as an *upper bound* on irreversible bit operations for a ~20 W brain—useful against fantasies of costless mind uploading, not as a claim that brains operate near that bound ([40](Sources.md#ref-40))—**S** as a physics ceiling.

**Not evidenced:** credible FLOP budgets for human-equivalent emulation at a chosen biophysical resolution; peer-reviewed end-to-end energy cost of a personal always-on frontier model with private memory; implantable compute envelopes compatible with neural tissue heat limits for merge-grade AI.

---

## Law, neurorights, and cognitive continuity

Legal and ethical work should stay focused on the human rights-bearer and clinical continuity. No jurisdiction surveyed for this chapter grants legal personhood to AI systems or to human–AI coupled agents as such.

Neuroethics literature develops candidate “neurorights”—mental integrity, cognitive liberty, mental privacy, psychological continuity—as norms under construction, not settled statutes ([41](Sources.md#ref-41), [42](Sources.md#ref-42)). Scholarship on non-voluntary explantation argues that functionally integrated implants can become constitutive of agency, so forced removal may violate autonomy—and that sponsors retain duties ([43](Sources.md#ref-43)). Related work on personal identity and advance directives under neural prostheses ([44](Sources.md#ref-44)) and clinical accounts of identity change after merging with a device ([45](Sources.md#ref-45)) ground exit rights and consent continuity in patient experience rather than speculative AI citizenship.

**Not evidenced:** settled law of cognitive continuity across substrate change; developed case law on ownership of neural data streams that power personal models; AI or hybrid legal personhood.
