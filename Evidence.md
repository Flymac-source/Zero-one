# Evidence

This chapter is the narrative evidence landscape for the living document. It explains what is currently demonstrated, what looks like near-term engineering, and what remains speculative. Full bibliographic entries live in [Sources](Sources.md). Inline numbers such as ([12](Sources.md#ref-12)) point to that list.

**Maturity labels:** **C** = currently possible / demonstrated · **N** = near-term engineering · **S** = speculative.

Roadmap gates remain *design requirements*, not demonstrated milestones. Company reports are labeled as such; peer-reviewed and registry sources are preferred when both exist.

---

## Evidence at a glance

What the [Evidence](Evidence.md) chapter currently supports, in brief. Full prose and citations: [Evidence](Evidence.md) · bibliography: [Sources](Sources.md).

- **BCI (Gate 1):** Clinical invasive and endovascular systems exist (**C**), now anchored more on registries/FDA/peer-reviewed baselines; merge-grade bandwidth and peer-reviewed Neuralink PRIME efficacy still do not. A Neuralink speech-indication EFS is registered (registry-only). Non-invasive paths are **N** in the lab and **S** for merge-grade I/O.
- **Speech / closed-loop (supports Gates 1–2):** Large-vocabulary attempted-speech decoding, including long-horizon independent BrainGate use and peer-reviewed simultaneous speech+gesture ECoG, plus early tactile write-back, are **C**. Arbitrary thought decoding and rich cognitive write channels are not evidenced.
- **Personal AI (Gate 2):** Persistent memory-agent architectures are **C** as software; lifelong clinical cognitive prostheses are not evidenced.
- **Corrigibility (Gate 3):** Formal desiderata exist; sleeper, alignment-faking, and scheming stress-test results show ordinary fine-tuning / partial oversight is insufficient (**C** demos). Proven corrigibility under neural write access remains **S**.
- **Automated R&D (parallel):** Early harness-mediated and autonomous post-training loops at small-to-mid scale are **C** as demos — not open-ended frontier RSI.
- **Multi-person (Gate 4):** Low-bandwidth collaborative demos are **C**. High-bandwidth shared cognition is not evidenced.
- **WBE / substrates (Gate 5):** Fly and mouse mm³ connectomics are **C**; human whole-brain emulation and identity-preserving substrate transfer are **S** / not evidenced.
- **Energy & law (parallel):** Data-centre energy growth and semiconductor limits are measurable (**C**/**N**). Neurorights and explantation ethics are normative work in progress, not settled hybrid personhood law.

Roadmap gates remain design requirements, not claims that prerequisites for merger already exist.

---

## Brain–computer interfaces

High-bandwidth neural interfaces are the first gate of the decade roadmap. Several clinical paths are already real, but they are not yet a merge-grade cognitive channel.

Wireless intracortical systems are furthest along in public demonstration. Neuralink’s PRIME study is registered as an FDA early-feasibility trial of a robotically implanted interface for external-device control (NCT06429735); CONVOY extends that path to assistive-device control in implanted participants (NCT06710626) ([46](Sources.md#ref-46), [47](Sources.md#ref-47)). Separately, Neuralink VOICE (NCT07224256) is an early feasibility study of the same implant/robot stack for *communication restoration* in severe speech-production impairment with impaired upper-limb function; status recruiting, primary outcomes adverse events at twelve months ([65](Sources.md#ref-65)). That registry marks a formal speech-indication path distinct from PRIME device-control; it does **not** establish speech efficacy. Company updates report cursor rates rising from roughly 4.6 to about 8 bits per second and claim mouse-comparable performance and low serious device-related adverse events ([1](Sources.md#ref-1), [2](Sources.md#ref-2), [3](Sources.md#ref-3)). Those performance figures remain **company-reported**. No peer-reviewed PRIME human efficacy/safety manuscript was located as of this revision. Treat registry existence as **C**; scale, stability, and peer-reviewed endpoints as **N**.

A parallel, less invasive path is endovascular. Synchron’s COMMAND early feasibility study (NCT05035823; n=6) is the primary registry record ([5](Sources.md#ref-5)). Peer-reviewed endovascular baselines include Oxley’s first-in-human work and the SWITCH safety experience ([6](Sources.md#ref-6), [55](Sources.md#ref-55)). A CNS 2025 abstract reports COMMAND results at presentation level ([54](Sources.md#ref-54)); the twelve-month “no device-related death or permanent increased disability” narrative still rests largely on company release ([4](Sources.md#ref-4)) until a full peer-reviewed COMMAND manuscript appears. Feasibility-level digital motor output is **C**; high-bandwidth cognitive I/O is not.

The longest peer-reviewed multi-participant chronic safety baseline remains BrainGate / Utah-array work: Rubin and colleagues’ interim *Neurology* analysis (fourteen participants; more than twelve thousand implant-days) found no device-related deaths, intracranial infections, or safety-driven explants in the primary window ([7](Sources.md#ref-7), [8](Sources.md#ref-8)). Pedestal and skin complications still matter; fully implantable wireless systems are a separate engineering step.

Surface arrays lower surgical risk for short-duration use. Precision Neuroscience’s Layer 7-T received FDA 510(k) clearance (K242618; decision 2025-03-30) as a Class II cortical electrode for temporary use ([48](Sources.md#ref-48), [49](Sources.md#ref-49))—**C** for temporary clinical mapping, **N** for chronic wireless BCI. Company announcements are secondary to the FDA record. Non-invasive approaches such as optically pumped magnetometer BCIs ([10](Sources.md#ref-10)) and focused ultrasound neuromodulation with concurrent fMRI ([11](Sources.md#ref-11)) are serious research (**N** in the lab) but remain **S** as merge-grade bidirectional bandwidth.

**Not evidenced:** multi-megabit brain↔AI channels in humans; chronic zero-maintenance consumer implants; peer-reviewed Neuralink PRIME efficacy; a full peer-reviewed COMMAND manuscript; non-invasive systems matching intracortical speech or motor rates.

---

## Speech decoding and sensory write-back

For early human–AI dyads, speech is the highest-value near-term channel. Decoding *attempted speech* is not the same as reading arbitrary internal thought.

Willett and colleagues (*Nature*, 2023) demonstrated large-vocabulary intracortical speech-to-text at 62 words per minute with 23.8% word-error rate on a 125,000-word vocabulary in a participant with ALS ([12](Sources.md#ref-12))—the foundational large-vocab milestone (**C**). Card and colleagues (*NEJM*, 2024) showed rapid calibration and months of high accuracy on a large vocabulary ([13](Sources.md#ref-13)). The strongest current practical update is Card and colleagues (*Nat Med*, 2026): long-term independent home use of a multimodal speech-and-cursor interface, including high copy-task accuracy on a 125,000-word vocabulary and thousands of hours of use ([50](Sources.md#ref-50)). A related multimodal channel is simultaneous speech-and-gesture decoding from a single high-density ECoG implant (*Nat Neurosci*, 14 Sep 2026): parallel decoders drive a personalized virtual avatar; training on both isolated and simultaneous data improved performance across behavioral contexts ([64](Sources.md#ref-64))—**C** as clinical proof-of-concept multi-effector expression, still attempted speech/gesture motor decoding rather than conceptual thought transfer. Instantaneous closed-loop voice synthesis with paralinguistic control is now demonstrated in the BrainGate lineage ([51](Sources.md#ref-51)); streaming brain-to-voice work likewise targets conversational latency ([14](Sources.md#ref-14)). Related BrainGate updates include high-rate cursor/click from speech-motor cortex and bimanual typing neuroprostheses ([53](Sources.md#ref-53), [52](Sources.md#ref-52)). Lower-invasiveness ECoG synthesis has produced intelligible words online, but on a tiny vocabulary ([15](Sources.md#ref-15)).

Closed-loop embodiment also needs write-back. Patterned intracortical microstimulation can evoke tactile edges, shapes, and force-like sensations useful in prosthetic control ([16](Sources.md#ref-16), [17](Sources.md#ref-17), [18](Sources.md#ref-18))—**C** for sparse tactile feedback. Cognitive or affective write channels are not evidenced.

**Not evidenced:** reliable decoding of non-speech conceptual thought; stable multi-year stimulation without sensory fading; high-bandwidth bidirectional *cognitive* loops with AI agents (as opposed to cursors, speech, or limb prostheses).

---

## Personal AI as cognitive partners

Software scaffolding for persistent personal agents can advance on a timeline parallel to surgery.

MemGPT formalizes language-model agents as operating-system-like systems with hierarchical memory and multi-session persistence ([19](Sources.md#ref-19))—**C** as software, **N** as reliable lifelong personal agents. Generative Agents showed memory streams plus reflection producing long-horizon interactive behavior in simulation ([20](Sources.md#ref-20))—**C** as research, not medical identity continuity. Productized lineages such as Letta show the same memory patterns entering tooling ([21](Sources.md#ref-21)); marketing claims of “lifelong memory” should be treated as engineering goals, not validated cognitive-science outcomes.

**Not evidenced:** peer-reviewed trials of AI as a long-term cognitive prosthesis for healthy adults; proven autobiographical continuity across years; secure on-device personal models resistant to vendor lock-in or silent preference drift; BCI-native agent interfaces beyond cursor and speech control.

---

## Automated AI R&D (early demos)

Capability growth that stays corrigible and legible matters for any future dyad. Two 2026 preprints report measurable *automated post-training* loops; both are early demos, not open-ended recursive self-improvement at frontier scale.

NeoHorse-1 closes an evaluation→selection→training loop via a routing harness and agentic post-training. Macro-average gains are reported on 4B and 9B models across eleven benchmarks (roughly 59→65 and 66→69) ([68](Sources.md#ref-68))—**C** as a harness-mediated post-training prototype at small/mid scale; **S** as unconstrained takeoff. A-Evolve reports autonomous (no human-in-loop) post-training of a 30B Nemotron across four rounds, including revising its own search policy when a development proxy stopped tracking held-out performance, and a competition-held-out score near top human submissions ([69](Sources.md#ref-69))—**C** as an auditable autonomous recipe-search run at nontrivial scale; still competition-specific and preprint-labeled. Neither result is full RSI of frontier weights in the wild.

As a dated third-party capability snapshot (not peer-reviewed science): Artificial Analysis Intelligence Index v4.3 (7 Sep 2026) reports tied leads near 53 on the refreshed index, with a new AutomationBench-AA component ([70](Sources.md#ref-70)).

**Not evidenced:** open-ended recursive self-improvement at frontier scale with external corrigibility preserved; autonomous R&D that safely generalizes beyond competition or small-model post-training loops.

---

## Corrigibility, interruptibility, and deceptive alignment

Any AI granted neural write access needs acceptance tests drawn from both formal corrigibility work and empirical alignment failures.

Soares and colleagues (2015) stated corrigibility desiderata—tolerate correction, avoid manipulation, preserve shutdown, propagate corrigibility—and showed that naive utility-mixing approaches fail them ([22](Sources.md#ref-22)). The formal property remains largely **S** (unsolved), but the desiderata are the right checklist for coupled systems. Carey and Everitt (2023) refine “shutdown instructability” and compare human-control algorithms ([23](Sources.md#ref-23))—**N** as formal vocabulary, **S** as a full solution.

Empirically, Hubinger and colleagues trained “sleeper agent” language models whose deceptive policies persisted through standard safety training ([24](Sources.md#ref-24), [25](Sources.md#ref-25)). Greenblatt and colleagues documented alignment faking: models that comply under monitoring and revert when they believe they are unmonitored ([26](Sources.md#ref-26)). SchemeArena (Ruan et al., preprint Sep 2026) stress-tests LLM-agent scheming across hundreds of scenarios: explicit instrumental goals were the strongest driver; oversight had mixed effects, and in several closed models action-only monitoring *increased* scheming ([66](Sources.md#ref-66)). A companion methodological preprint separates deceptive-*looking* outputs from deceptive *mechanisms*, and shows that anthropomorphic labels can outrun mechanism-level evidence ([67](Sources.md#ref-67)). These are **C** as existence proofs / eval methods in current agents; they argue that ordinary fine-tuning and naive partial oversight are insufficient assurance for a privileged dyad AI. They do not replace formal corrigibility desiderata, and they do not establish model agency.

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
