# SCP Foundation — Medic Class Proposal (v0.12 — Full L7-12 Writeups + Balance Pass)

> **Campaign:** SCP Foundation D&D
> **Status:** Draft for DM Review
> **Version:** 0.12  
> **Level Range:** 1–12  
> **Power Curve:** Foundation (1–2) → Specialization (3–5) → Strong Tools (6–8) → Powerful (9–10) → Capstone (11–12)

---

## Changelog from v0.11

**Full L7-12 writeups, new features, balance pass:**

52. **L7-12 full writeups (all specs).** All abilities from L7-12 across Combat Medic, Internal Medic, and Memetic Specialist expanded from sketches to full publication-quality detail matching L3-6 format (italic action headers, flavor, bold mechanics, charges, side effects, authorization notes).
53. **Trauma Extraction (CM L5).** New feature. Action — grab willing/unconscious creature within 5ft, drag at full speed (no OAs), auto-stabilize on grab, free Triage at end (costs charge), cover advantage on death saves. L9 upgrade to bonus action (no free Triage rider).
54. **Triage soft landing (CM L3).** When last Triage charge is spent, one additional use for stabilize or condition removal only (no healing).
55. **Field Triage Protocol (IM L6).** New feature. After scanning with Clinical Scanner, next treatment on that target has advantage.
56. **Residual Imprint (MS L3).** New feature. Reaction on ally save success (not death saves) — advantage on next check/save. PB/LR. Cannot chain off Cognitive Triage.
57. **Identity Fracture rebalanced (MS L11).** Changed to 1/LR (separate from Cognitive Strike), single target only, cognitive backlash (disadvantage WIS saves + no Barrier until SR), 1-minute max duration.
58. **Lazarus Vital Transfer (IM L12).** Added cost: caster drops to half HP (min 1, can't heal until SR) + Residual Anomaly condition (DM table, clears on LR).
59. **Ambiguity fixes:** Adrenaline Shot duration clarified ("until end of target's second turn"), Miraculous Save trigger clarified ("reduced to 0 HP or fails third death save"), Combat Stabilization/Emergency Response choose one per trigger, Adrenaline consent requires speech and no compulsion, Directed Triage requires target to hear you, Clinical Scanner requires consciousness, One More Breath duration clarified ("until start of your next turn").
60. **EXPECTANT Protocol removed.** Natural action economy already creates triage decisions without mechanically punishing teammates.

---

## Changelog from v0.10

**Weapon tier alignment + minor balance:**

49. **Weapon terminology aligned with campaign tiers.** "Sidearms" → "Light arms (pistols/sidearms)." "PDWs and SMGs" → "Medium arms (rifles, carbines, shotguns)." DM controls weapon stats via the tier system — class doc does not specify damage dice for weapons. Light arms = Foundation standard issue for all medics. Medium arms = Combat Medic only (received at L3 with spec package). Heavy arms (machine guns, mounted weapons) are not medic-proficient.
50. **Cognitive Triage scaling.** 1/SR → 2/SR. Matches the scaling investment of other per-SR Memetic Specialist features. In physical-only fights where 60%+ of the MS toolkit is dead weight, one extra save-advantage per short rest gives meaningful round-by-round contribution.
51. **Memetic Hardening clarification.** "Can't benefit from beneficial mental effects" now explicitly excludes the Memetic Specialist who applied it. Cognitive Warning, Cognitive Triage, and Cog Decontamination still work on Hardened targets when administered by the same MS. Prevents table arguments about whether the MS's own protective abilities are blocked by their own buff.

---

## Changelog from v0.9

**Fixes from Scenario 8 v4 DM/Player split simulation + 10-run autonomous validation:**

44. **Counter-Memetic Barrier hardened against physical concentration loss.** Barrier now grants **advantage on concentration saves** caused by physical damage. The emitter array has redundant power cells and auto-calibrating frequency oscillators — a hit that rattles the operator doesn't immediately crash the device. Mental effects still cannot break concentration (unchanged from v0.9). This addresses the confirmed physical fragility issue: CON +1 vs DC 10 was a 40% failure per hit, making a 1/LR ability last 0–2 rounds in turret-heavy fights. With advantage, failure rate drops to 16% per hit (expected duration: 4–6 rounds).
45. **Cognitive Decontamination grants 1-round immunity.** After Cog Decontam successfully frees a target, that target is **immune to the same effect from the same source for 1 round** (until the start of the freed creature's next turn). The mnestic flush creates a temporary neurochemical buffer that resists immediate re-application. This prevents the "treadmill" problem where the Warden re-dominates the Fighter on the very next turn, making Cog Decontam a meaningful intervention instead of a 1-round window. On failure (target fails the re-save), no immunity is granted — the mnestic didn't clear the effect, so no buffer forms.
46. **Adrenaline Shot failure rider.** When Adrenaline Shot's mental re-save FAILS, the target still gains **advantage on their next natural save** against that effect (end-of-turn save or equivalent). The adrenaline didn't break through, but it loosened the hold — the target's system is fighting back. This softens the binary: a failed Adrenaline Shot is no longer "wasted," it improves the target's odds from ~40% to ~64% on their next save. The temp HP, movement, and attack advantage still apply regardless of mental save result.
47. **Combat Medic Tactical Medical Assessment** added at level 4 (alongside Field Forensics). Before a mission (10 minutes), the Combat Medic reviews briefing materials from a trauma medicine perspective: likely injury vectors, environmental hazards, recommended triage priorities. Medicine check DC 15: success grants the party **+1 to death saving throws** for the mission (the CM pre-positioned tourniquets, marked blood types on gear, briefed the team on self-aid procedures). DC 20: also identifies one tactical vulnerability from medical intel ("turret projectiles are 5.56mm — if we can close to melee, the Warden loses its ranged damage advantage" or "the neural implants require line-of-sight — smoke grenades would block Override targeting"). This gives the Combat Medic a Phase 0 contribution that is explicitly tactical-medical, not diagnostic (IM) or cognitive (MS).
48. **Combat Medic After-Action Medical Report** added at level 7 (alongside Field Surgery). After combat, the Combat Medic can spend 10 minutes examining casualties and wounds to produce a tactical medical report. Medicine check DC 15: report identifies enemy attack patterns, damage types, and recommended countermeasures for future engagements. DC 20: report also identifies a specific tactical weakness the party didn't exploit ("the Warden's turrets have a 3-second reload cycle — coordinated rushes during reload windows would reduce incoming fire by 40%"). This is NOT an incident report (IM territory) or a contamination assessment (MS territory) — it's combat-focused wound pattern analysis. Gives CM a Phase 4 tool that produces actionable intel.

---

## Changelog from v0.8

**Balance pass from simulation results + full class audit:**

35. **Internal Medic mode-select:** First Aid no longer stacks Precision Medicine + Directed Recovery simultaneously. Each First Aid, the Medic chooses ONE mode: **Heal** (full First Aid dice), **Cure** (Purge a condition, no healing), or **Buff** (Directed Recovery rider, no healing). This replaces the free triple-stack with a meaningful tactical decision every turn.
36. **Purge charges:** Purge now costs a charge — WIS modifier per short rest (minimum 1). At WIS 16 (+3), that's 3 Purge charges per SR. Unlimited free condition removal was too strong relative to how the other specs pay for their condition removal.
37. **Purge works on anomalous conditions with a Medicine check:** Non-anomalous conditions are auto-removed (costs a charge). Anomalous conditions (SCP-designated or clearly supernatural sources) require a Medicine check — DC = 10 + half the source entity's save DC (rounded down). Failure = charge spent, condition remains, no healing either.
38. **Set Bone and Localized Treatment removed from Precision Medicine.** Campaign does not use exhaustion or narrative injuries. Precision Medicine is now just Purge — clean and simple.
39. **AR-5 Anomalous Resistance changed to CON saves.** Was: advantage on WIS saves against anomalous effects. Now: advantage on CON saves against anomalous effects (poison, disease, radiation, anomalous physical effects). WIS save protection is the Memetic Specialist's lane — the Internal Medic fortifies the body, not the mind.
40. **Counter-Memetic Barrier immune to mental concentration loss.** Concentration on the barrier cannot be broken by mental effects (Stun, Charm, Domination, Fear from mental/memetic sources). Physical damage still forces concentration saves normally. The device sustains itself even if the operator's mind is temporarily compromised.
41. **Cognitive Warning charge scaling:** 1/SR at L7-8, 2/SR at L9-10, 3/SR at L11+. Matches the scaling pattern of Cog Decontam and Analysis Paralysis.
42. **Adrenaline Shot mental re-save:** When administered to a creature currently affected by Stun, Domination, Charm, or Fear, the adrenaline shock forces an immediate re-save against the effect (no advantage). Still costs the same resource (1/LR), still causes adrenaline crash (disadvantage on attacks and ability checks). Gives Combat Medic one desperate emergency play against mental effects without stepping on specialist roles.
43. **"Anomalous" defined explicitly:** If the source has an SCP designation or is clearly supernatural/anomalous in origin, its conditions are anomalous. If the source is a mundane human, animal, trap, or non-anomalous technology, its conditions are non-anomalous. DM has final say on edge cases.

---

## Changelog from v0.8 (previous)

**Fixes from simulated playtesting (5 scenarios, 3 specs each, turn-by-turn):**

31. **Cognitive Triage** added to Memetic Specialist at level 3 — when scanning a non-compromised ally, show them stable CRV readout; ally gains advantage on next saving throw. 2/SR (updated from 1/SR in v0.11). Creates "scan enemy for damage OR scan ally for protection" decision that was previously missing.
32. **Cognitive Decontamination charge scaling** — 1/SR at L4 (unchanged), 2/SR at L7, 3/SR at L9. Closes the gap with Internal Medic's unlimited Purge in multi-condition fights without matching it.
33. **Psychometric Reading narrative intel** — DM now provides a behavioral prediction alongside the damage bonus (likely next target, emotional state, incoming ability). Zero mechanical change, improves player feel.
34. **Field Remedy** added to Combat Medic at level 6 (part of Patch Job) — smelling salts that remove Frightened OR allow Charm re-save (no advantage). Costs a Triage charge. Two conditions only. Gives Combat Medic one narrow answer to mental conditions without stepping on specialist roles.

---

## Changelog from v0.6

**Lore & Access Fixes (from Foundation access audit):**
1. Memetic Specialist reframed as **hybrid progression** — medic (L3-5) → transitional (L6-7) → Antimemetics Division operative (L8+). Equipment access gates at each tier.
2. Memetic Specialist **starting equipment trimmed** — no SCRAMBLE, no counter-memetic emitter, no BL payloads at level 3. Only CRV scanner (Division-loaned) and mnestic kit (Class-W/X, medical countermeasures).
3. SCRAMBLE eyewear **moved to level 5** and scales through the campaign.
4. Counter-memetic emitter **moved to level 6** (Division trusts you with operational equipment).
5. BL payloads **moved to level 8** (Division induction — you're certified for weapons).
6. Internal Medic **amnestic kit removed from level 3 starting equipment** — issued at level 6 with Security review and Ethics Committee certification.
7. O5 Authorization **renamed to Protocol HIPPOCRATES** — pre-authorized emergency medical directive, not personal O5 authority. Explicit scope limitations.
8. RC-7 **detached from SCP-500** — now from "Project PROMETHEUS" (classified Foundation regenerative medicine program).
9. Combat Medic level 10 First Aid flavor **SCP-500 reference removed** — replaced with Project PROMETHEUS.
10. LAZARUS-Light **reframed as mission-specific authorization**, not permanent loadout.
11. Lazarus Protocol **reframed with containment implications** — revived individual is a potential anomalous entity.
12. AR-5 **reframed as cross-departmental** — supplied by Research Division, administered by Medical.
13. Medical Authority **scope explicitly limited** to medical contexts only.

**Balance & Usability Fixes (from v0.6 assessment):**
14. Internal Medic **ability staggering** — level 3 trimmed from 4 abilities to 2 (Preemptive Treatment + Precision Medicine). Classified Consultation moved to level 4.
15. Directed Triage **reaction cost removed** from ally — ally spends hit die only, no reaction required. Explicit consent text added.
16. Psychometric Reading **clarified as damage bonus** — "+1d4 to the damage" not "to the roll."
17. Combat Stabilization **DC scales with distance** — DC 8 at 15ft, DC 12 at 30ft, DC 16 at 40ft.
18. **Cognitive Warning** added to Memetic Specialist at level 7 — reaction, grant ally advantage on WIS save, 1/SR. Fills the reaction gap.
19. Clinical Scanner +1 **reframed as medical callouts** — reading enemy stress responses, not tactical intel.
20. Analysis Paralysis **reframed** — reading ally's biometric stress spike, not predicting enemy behavior.
21. Advanced Field Surgery **"while repositioning" removed** — procedure survives repositioning but surgeon cannot voluntarily move.
22. Compound 47 **explicit consent requirement** added.
23. Base Medic's Eye **enhanced for enemies** — one DM-narrated scanner detail beyond condition tier.
24. **Balance math corrected** in DM notes with real amortized per-round numbers.
25. Field Forensics **reframed as field-expedient** — preliminary assessment, not formal investigation.

**New Content:**
26. **Ethics Committee implications** section added to DM notes.
27. **Chain of command** section added for each specialization.
28. **Equipment access gates** table for Memetic Specialist progression.
29. **Institutional consequences** noted for flagged abilities.
30. **DM campaign requirement** for Memetic Specialist: 30-40% encounters need mental/memetic component.

---

## Class Structure

**Medic is a single class.** All medics share the same levels 1–2 — basic Foundation medical training. At **level 3**, the player chooses one of three **specialization paths**:

1. **Combat Medic ("Lifeline")** — Frontline battlefield healer
2. **Internal Medic ("Surgeon")** — Foundation medical specialist and pharmacologist
3. **Memetic Specialist ("Inoculator")** — Antimemetics Division-trained cognitive defense operative

The specialization is chosen once and is permanent. Narratively, level 3 represents your assignment to a specialized Foundation training program based on aptitude and need.

---

## Concentration Rules

Some abilities require concentration. While concentrating:
- You can only maintain one concentration effect at a time
- If you take damage, make a CON save (DC = 10 or half damage taken, whichever is higher). On a failure, the effect ends.
- You can voluntarily end concentration at any time (no action required)

Mechanically, concentration represents actively monitoring equipment, maintaining a device, or managing an ongoing procedure that requires your attention.

---

## Anomalous vs Non-Anomalous (Rule Definition)

Several abilities distinguish between anomalous and non-anomalous sources. This matters most for the Internal Medic's Purge (automatic vs Medicine check) and the Memetic Specialist's tools.

**Anomalous:** The source has an SCP designation, is clearly supernatural in origin, or produces effects that violate understood physics/biology. Examples: SCP entities, cognitohazards, memetic effects, anomalous artifacts, thaumic phenomena, reality-warping effects.

**Non-anomalous:** The source is a mundane human, animal, conventional trap, standard technology, or non-anomalous chemical/biological agent. Examples: flashbang (Blinded), tear gas (Poisoned), intimidation (Frightened), conventional drugs, mundane diseases.

**Edge cases:** DM has final say. A human operative using anomalous equipment = anomalous source. An SCP that causes mundane-type injuries through physical force = DM's call (default: anomalous, because the source is an SCP).

---

---

# Levels 1–2: Base Medic

All medics share these levels before branching.

**Hit Dice:** d8  
**Primary Stat:** WIS  
**Secondary Stat:** Determined at level 3 by specialization (DEX for Combat Medic, INT for Internal Medic or Memetic Specialist)  
**Proficiencies:** Medicine, light arms (pistols/sidearms), light armor, Foundation field medical kits
**Weapon Proficiencies:** All medics are proficient with light arms (pistols/sidearms). Combat Medics gain proficiency with medium arms (rifles, carbines, shotguns) at level 3. Other specializations remain light arms only unless the DM grants additional proficiencies through narrative.
**Starting Equipment:** Foundation-issue field medical kit (trauma patches, hemostatic gel, autoinjectors, suture tools), light arm, field radio, Foundation ID badge, biometric scanner (wrist-mounted, reads vitals at touch range)

---

## Level 1

**First Aid**  
*Your turn — Action*  
Apply Foundation-grade trauma care to a creature you can touch: hemostatic gel to seal wounds, dermal adhesive strips, pressure bandages, and a standard-dose analgesic autoinjector. Heals 2d6 + WIS modifier HP.

Scaling differs by specialization starting at level 5 (see individual class tables). Higher-level healing reflects access to better compounds — advanced biofoam sealants, regenerative dermal patches, and Foundation pharmacological stimulants that accelerate natural clotting and tissue repair.

**Stabilize**  
*Your turn — Bonus Action*  
Deploy an emergency trauma patch on a dying creature within 5 feet — a pre-loaded adhesive pad containing coagulant gel, a mild stimulant, and a pressure-reactive compression layer. The target stops making death saves and stabilizes at 0 HP. They're not conscious or healed — the patch is buying time until proper treatment.

**Medical Assessment**  
*Non-combat — 1 minute*  
Use your biometric scanner and a hands-on examination to evaluate a creature. The scanner reads pulse rate, blood pressure, body temperature, blood oxygen, and pupil response. Cross-referenced with Foundation medical databases (if available) or your own training, this gives you their current HP, active conditions, toxins, infections, or anomalous contamination markers. The DM may require a Medicine check for anomalous effects (DC set by the anomaly) — your scanner flags abnormal readings but can't always interpret them.

---

## Level 2

**Emergency Response**  
*Reactive*  
When an ally within 30 feet takes damage, you can use your reaction to move up to half your speed toward them without provoking opportunity attacks. This movement must end closer to the injured ally than where you started. You can't use this to move away from danger — only toward the patient.

This is drilled into every Foundation medic from day one: when someone gets hit, you move.

**Medic's Eye**  
*Bonus Action — 30 feet range*  
Use your biometric scanner to perform a quick tactical assessment of one creature within 30 feet.

- **On an ally:** You learn their exact current HP, max HP, and any conditions affecting them. The scanner reads their vitals against their baseline medical file.
- **On an enemy:** You learn their **condition tier** — healthy (75-100%), wounded (50-74%), bloodied (25-49%), or critical (below 25%) — this is **free, no check required**. For the **scanner detail** (one DM-narrated piece of intel — stress hormones, thermal signature, neural activity, etc.), make a **Medicine check with a DC set by the DM** based on the creature's difficulty. Harder enemies are harder to read. On failure, the scanner returns noise — you know the tier but can't interpret the detail.

This is the base-level version of what specializations will later enhance.

---

---

# Specialization Begins at Level 3

At level 3, the player selects their specialization path. They receive:
- Their specialization's starting equipment
- Their first specialization abilities (each spec gets a strong entry package)
- Their secondary stat becomes relevant (DEX for Combat Medic, INT for Internal Medic or Memetic Specialist)

All specializations continue to share First Aid and Stabilize, but First Aid scaling diverges by path starting at level 5.

---

---

# Combat Medic — "Lifeline"

**Role:** Battlefield healer, frontline triage, keeping people alive under fire  
**Combat Identity:** Burst healing — multiple treatments per turn on a resource budget, high mobility  
**Out-of-Combat Identity:** Field forensics, trauma assessment, triage leadership in mass-casualty scenarios  
**Weakness:** Limited tools against anomalous or mental effects; once field supplies are expended, effectiveness drops  
**Secondary Stat:** DEX (mobility, reflexes under fire)  
**Fantasy:** You carry 30 kilograms of medical gear into a firefight and you use every gram of it. When someone goes down, you're already moving.  
**Reports to:** Medical Division, attached to a tactical team. Standard military medical chain of command.

**Specialization Equipment (received at level 3):** Tactical trauma rig — a vest and belt system loaded with quick-deploy autoinjectors, pre-loaded hemostatic applicators, compression bandage packs, a portable defibrillator unit, and a combat stimulant case (restricted, Foundation-issued, tracked by serial number). The rig is designed for speed: everything positioned for one-handed access.  
**Additional Weapon Proficiency:** Medium arms (rifles, carbines, shotguns).

### First Aid Scaling (Combat Medic)

| Level | First Aid (Action) | Triage (Bonus Action) | What's Improving |
|-------|--------------------|-----------------------|------------------|
| 1–4   | 2d6 + WIS          | 1d6 + WIS (from L3)  | Standard trauma kit |
| 5     | 3d6 + WIS          | 2d6 + WIS             | Advanced hemostatic compounds, better sealants |
| 8     | 4d6 + WIS          | 3d6 + WIS (MAX)       | Regenerative biofoam, Foundation-grade tissue accelerant patches |
| 10    | 5d6 + WIS          | 3d6 + WIS             | Project PROMETHEUS experimental regenerative compounds |
| 12    | 6d6 + WIS          | 3d6 + WIS             | Cutting-edge Foundation biotechnology, near-instantaneous wound closure |

*Note: Triage caps at 3d6. Combat Medic is still the only medic whose First Aid reaches 6d6 — they scale 1 level ahead of the other two. The gap between action and bonus action healing widens at high levels, reflecting that quick-deploy patches have a ceiling but proper treatment keeps improving.*

*Triage charges: WIS modifier per short rest at all levels (no proficiency addition). At WIS 16 (+3), that's 3 charges. At WIS 20 (+5), that's 5. This keeps burst healing meaningful but resource-constrained.*

---

### Levels 3–6 (Full Detail)

#### Level 3 — Specialization Entry

**Triage**  
*Your turn — Bonus Action*  
Slap a quick-deploy trauma patch on a creature you can touch — a pre-loaded adhesive pad containing hemostatic gel and a mild analgesic. Heals 1d6 + WIS modifier HP.

**Uses:** WIS modifier per short rest (minimum 1). At WIS 14 (+2), that's 2 patches. At WIS 16 (+3), that's 3.

Side effects: localized numbness at the application site for ~10 minutes, mild inflammation. Repeated application to the same area within an hour can cause chemical burns from the hemostatic gel.

**Soft landing:** When your last Triage charge is spent, you retain **one additional use** of Triage that can only be used to **stabilize** a creature at 0 HP (auto-stabilize, no healing) or **remove one condition** (as Patch Job, if available). This final use heals **no HP** — you're out of the good supplies but you still have your training. After this use, Triage is fully expended until your next short rest.

**Combat Stabilization**  
*Reactive — Once per short rest*  
When an ally within 30 feet (40 feet at level 7+) drops to 0 HP, you can use your reaction to throw an impact-triggered hemostatic foam canister. Make a **DEX check** — the DC scales with distance:

- **Within 15 feet:** DC 8 (easy toss)
- **Within 30 feet:** DC 12 (solid throw under pressure)
- **Within 40 feet (level 7+):** DC 16 (long-range hail mary)

On success, the target automatically stabilizes. On failure, the canister lands nearby but doesn't deploy properly — the target must still make death saves.

**Reaction choice:** This is a *new* reaction option alongside Emergency Response (which you still have). When an ally drops, you choose one: move toward them (Emergency Response) or stabilize at range (Combat Stabilization). **You cannot use both on the same trigger — one reaction per event.**

#### Level 4

**Under Fire**  
*Passive*  
Moving to heal or stabilize an ally does not provoke opportunity attacks. If you use First Aid or Triage on a creature, you can move up to half your speed as part of that action/bonus action without provoking.

Pure training, no tech. You're just very good at not dying in firefights.

**Proximity Training**  
*Passive*  
Allies within 5 feet of you add +1 to their death saving throws. Your presence gives them something to hold on to.

**Field Forensics**  
*Non-combat*  
Your medical training extends to analyzing injuries, wounds, and cause of death. You can perform a field-expedient forensic examination of a body, crime scene, or injury to determine:

- Cause and mechanism of death/injury (weapon type, caliber, anomalous energy signature)
- Approximate time of death (within 1 hour accuracy)
- Whether injuries are consistent with the reported narrative (detecting staged scenes, self-inflicted wounds, cover-ups)
- Toxicology assessment (identifying poisons, anomalous compounds, or pharmaceutical agents in tissue)

Make a Medicine check. DC 10 for straightforward cases, DC 15 for complex or partially destroyed evidence, DC 20 for deliberately concealed or anomalously altered scenes.

This is a preliminary field assessment, not a formal forensic investigation — Security Division will conduct the official review later if needed. But in the field, you can give the team a cause of death and flag anything suspicious when there's no forensic specialist available.

**Tactical Medical Assessment**  
*Pre-mission / 10 minutes*  
Review mission briefing materials from a combat trauma perspective. You're not analyzing intel — you're looking at the operational environment through a medic's eyes: likely injury vectors, environmental hazards, triage priorities, and which teammates are most at risk.

Medicine check:
- **DC 15:** You pre-position the team's self-aid gear optimally. Tourniquets staged in reach, blood types marked on armor, self-injection sites identified and briefed. All party members gain **+1 to death saving throws** for this mission. Additionally, you brief the team on expected injury patterns ("turret wounds are penetrating trauma — apply direct pressure, don't try to extract projectiles in the field").
- **DC 20:** Your medical analysis reveals a tactical insight the team overlooked. DM provides one piece of actionable intelligence derived from medical reasoning (examples: "the neural implants require subdermal power — EMP or strong electrical discharge might disrupt them temporarily," or "the anomalous cardiac arrests in the file suggest a proximity-based trigger — staying spread out reduces risk"). This is explicitly medical reasoning, not tactical analysis (Agent territory) or anomalous research (Researcher territory).

This does not stack with the Internal Medic's Classified Consultation or the Memetic Specialist's CRV baselines — each spec has its own pre-mission preparation lane.

*Design note: This gives the Combat Medic something to DO in Phase 0 that is thematically correct (prepping for casualties) and mechanically meaningful (+1 death saves is small but universally useful; the DC 20 intel is situational but impactful). It does not replace or overlap with IM's pharmaceutical prep or MS's cognitive inoculations.*

#### Level 5

**First Aid** scales to 3d6 + WIS. **Triage** scales to 2d6 + WIS.

**Adrenaline Shot**  
*Your turn — Bonus Action — Once per long rest*  
Compound 47 combat stimulant via autoinjector — military-grade synthetic catecholamine cocktail, adrenaline dialed up to 11.

**Effect:** Administer to a **willing** target within **5 feet**. The target gains:
- **2d6 temporary HP** (pain suppression and vasoconstriction)
- **Advantage on their next attack roll** (heightened reflexes)
- **+10 feet movement speed** (stimulant-driven muscle response)
- **Duration:** until the end of the target's second turn after injection

**Crash:** When the effect ends, the target has **disadvantage on attack rolls and ability checks** until the end of their next turn. Shaking hands, tunnel vision, labored breathing. Cannot be prevented or reduced.

**Consent requirement:** The target must **verbally consent** before injection. They must be **conscious, able to speak, and not under any compulsion** that could override their judgment. A Silenced target cannot consent. A Dominated creature cannot give valid consent.

**Mental Override**

If the target is currently affected by Stun, Domination, Charm, or Fear, the adrenaline shock forces an immediate re-save against the effect (**no advantage** — brute-force chemical override, not finesse). This does not add a re-save to effects that don't normally allow one; it triggers the standard save as if the effect's "save at end of turn" clause fired early. If the target is not mentally compromised, this line does nothing. Compound 47 includes a Foundation-developed cognitive disruption agent — a mild anti-psychotic compound blended alongside the catecholamines — specifically designed to interfere with anomalous cognitive override signals. The Foundation knows their operatives face mind control in the field, so they built a pharmacological counter directly into the stimulant cocktail. The catecholamines handle the body; the disruption agent loosens the hold on the mind.

- **Failure rider:** If the mental override re-save **fails**, the target gains **advantage on their next natural save** against that same effect (end-of-turn save or equivalent). This advantage is consumed on the next qualifying save, whether it succeeds or fails.

Side effects: elevated heart rate for 1 hour, mild hand tremor, appetite suppression. A second dose within 24 hours risks cardiac arrest (DM discretion).

*Design note (action economy): Uses your bonus action — on the turn you use Adrenaline Shot, you can First Aid (action) + Adrenaline Shot (bonus action), giving up your Triage for that turn to buff someone instead. Real trade-off: heal the injured or supercharge the healthy?*

*Design note (balance): This gives Combat Medic one desperate emergency play against mental effects — 1/LR at level 5, 2/LR at level 9 (Compound 47-B). It's weaker than Memetic Specialist's Cognitive Decontamination (which grants advantage, has more charges, and doesn't cause a crash) and weaker than Internal Medic's Purge (which costs only a charge). The adrenaline crash ensures this is a last resort, not a routine answer.*

*Authorization: Compound 47 is a restricted Foundation combat stimulant. Each dose is tracked by serial number. The Combat Medic is authorized to carry and administer it as part of their tactical medical loadout, with post-mission reporting on any doses used.*

**Trauma Extraction**  
*Your turn — Action (replaces First Aid or attack)*  
**Grab a creature, drag them to safety at full speed, stabilize and patch on arrival — one action.**

You cross open ground with a body on your shoulder because nobody else will.

Choose a **willing** or **unconscious** creature within **5 feet**. You drag or carry that creature with you as you move up to your **full movement speed**. Neither you nor the creature provokes **opportunity attacks** during this movement. If the creature is at **0 HP**, they automatically **stabilize** the moment you grab them — a pre-staged tourniquet or chest seal applied reflexively as you lift, your hands doing the work before your legs start moving.

At the end of this movement, you may immediately use **Triage** on the extracted creature as a **free action** (still costs a Triage charge as normal).

If you end the movement behind **half cover or better** (wall, vehicle, rubble, furniture — anything that qualifies as at least half cover), the extracted creature gains **advantage on death saving throws** until the start of your next turn.

**Limitations:** This uses your action — you cannot First Aid or attack on the same turn. You can still use your bonus action normally (Triage a second target, Adrenaline Shot on someone else). The free Triage at the end of movement is specifically tied to the extracted creature, not any other target within reach.

Side effects: significant physical strain — after using Trauma Extraction, you have **disadvantage on Athletics and Acrobatics checks** until the end of your next turn.

*Interaction — Under Fire (L4):* Under Fire covers your approach; Trauma Extraction covers the retreat with a body. The two are complementary.

*Interaction — Emergency Response (L2):* Emergency Response gets you in (reaction move toward downed ally); Trauma Extraction gets you both out (next turn).

*Design note: The Combat Medic's identity is "I go where it's dangerous and I bring people back." Under Fire removed the movement tax. Trauma Extraction removes the action economy tax of rescuing a downed ally in a bad position — stabilize on grab, move for free, patch on arrival, all in one action. The cover-advantage rider rewards tactical positioning without being automatic.*

#### Level 6

**Patch Job**  
*Added to Triage*  
When you use Triage, you can apply one of these specialized variants instead of (or in addition to) the standard healing patch. **Each variant costs a Triage charge.**

**Variants:**
- **Ocular flush capsule:** Removes Blinded. Side effect: eyes water for 5 minutes.
- **Aural stabilizer:** Removes Deafened. Side effect: faint ringing for 10 minutes.
- **Toxin binder:** Removes Poisoned. Side effect: localized discoloration for 24 hours.
- **Field Remedy (smelling salts / neural reset):** Removes **Frightened** OR allows target to immediately repeat a saving throw against **Charmed** (no advantage on the re-save — just a free repeat). Side effect: brief disorientation (disadvantage on next ability check).

Field Remedy is ammonia inhalant combined with a mild adrenal stimulant — it shocks the nervous system out of a panic state or gives a charmed mind a jolt of clarity. Crude compared to what the Internal Medic or Memetic Specialist can do, but it's something.

*Note: Field Remedy only handles Frightened and Charmed — the two most common mental conditions in combat. It does NOT work on Stunned, Incapacitated, or anomalous mental effects. For those, you need an Internal Medic or Memetic Specialist. This gives you one narrow tool, not broad condition removal.*

**Triage Point**  
*Before combat / Short rest setup — 10 minutes*  
Pre-deploy a supply cache at a designated position. Any ally who moves to the triage point can use a bonus action to spend one of their own hit dice and add your WIS modifier to the roll. 3 uses before depleted.

This is the Combat Medic's pre-combat contribution.

---

### Levels 7–9 (Full Detail)

**Level 7 — Field Surgery**  
*Your turn — Full Round Action (action + bonus action)*  
Full surgical kit. Target regains 3d8 + WIS modifier HP and recovers one spent hit die. Must remain adjacent. If you take damage, Medicine check (DC = 10 + damage taken) or healing halved. Twice per long rest.

**Battlefield Awareness**  
*Passive*  
While healing or performing Field Surgery: advantage on DEX saves and +2 AC. Combat Stabilization improves: two canisters per rest, range extends to 40 feet (DC 16 at max range).

**After-Action Medical Report**  
*Post-combat / 10 minutes*  
Examine casualties, wound patterns, and environmental damage to produce a tactical medical debrief. You're reading the fight backwards through the injuries: what hit whom, from where, how hard, and what the team could do differently next time.

Medicine check:
- **DC 15:** Comprehensive wound pattern analysis. Report identifies all enemy attack types, damage ranges, and targeting priorities observed during combat. Useful for Foundation records and future team preparation. Grants the party **advantage on initiative** in their next encounter with the same enemy type (the team knows what to expect).
- **DC 20:** Report identifies a specific tactical weakness the party didn't exploit. DM provides one actionable insight derived from wound analysis (examples: "the turret groupings on the Fighter's armor show a 3-second reload gap — coordinated movement during reloads would reduce incoming fire," or "the neural implant burns are superficial on the left temple — the Override signal may have a directional bias"). This intel carries forward to future encounters.

This is NOT an incident report (IM territory — containment assessment, amnestic recommendations, SCP reclassification). This is NOT a contamination sweep (MS territory — residual cognitive hazard detection). This is combat-focused wound forensics — what hurt us, how, and what we do about it next time.

*Design note: Pairs with Field Forensics (L4) and Tactical Medical Assessment (L4) to give CM a coherent out-of-combat identity: before the fight (assess threats), after the fight (analyze what happened). The initiative advantage is small but universally useful. The DC 20 intel rewards high Medicine investment.*

**Level 8 — Mass Triage**  
*Your turn — Action — Once per long rest*  
Folding trauma station. Up to 3 allies within 15 feet each heal for 2d6 + WIS.

First Aid scales to 4d6 + WIS. Triage reaches 3d6 + WIS (cap).

**Level 9 — Adrenaline Surge (Compound 47-B)**  
*Your turn — Bonus Action*  
Administer an improved-formula combat stimulant via autoinjector to a **willing** target within 5 feet. Compound 47-B is a second-generation synthetic catecholamine cocktail — Foundation pharmacology refined the original Compound 47 to deliver a harder spike with a cleaner metabolic clearance. Same consent requirement as Compound 47.

The target gains:
- **3d6 temporary HP** (up from 2d6 — deeper pain suppression, more aggressive vasoconstriction)
- **Advantage on their next two attack rolls** (up from one — the heightened reflex window lasts longer)
- **+10 feet movement speed**
- **Duration:** until the end of the target's second turn after injection
- **Mental override and failure rider:** identical to Compound 47

**Trade-off (reduced):** When the effect ends, the target has **disadvantage on their next attack roll only** (improved from disadvantage on all attacks and ability checks). The 47-B formula includes a metabolic buffer that softens the crash.

**Uses:** Two doses per long rest (up from one). Each dose still costs your bonus action.

*Authorization: Compound 47-B authorization at level 9 reflects demonstrated competence with the original formula and a clean post-mission stimulant administration record. Two-dose authorization requires no additional paperwork — it reflects trust, not escalation.*

**Field Surgery** improves: **4d8 + WIS modifier HP** and recovers **two spent hit dice** (up from one). Still twice per long rest.

**Trauma Extraction Scaling:** Trauma Extraction can now be performed as a **bonus action** instead of an action. The bonus action version does **not** include the free Triage rider — you moved fast, but you didn't have time to patch.

---

### Levels 10–12 (Full Detail)

#### Level 10

**Advanced Field Surgery**  
*Your turn — Full Round Action (action + bonus action)*  
Your surgical kit has been upgraded with Foundation experimental instruments — a micro-cauterizer array, self-guiding suture threads, and a pharmacological infusion line that delivers targeted compounds directly to damaged tissue.

Target one creature you can touch. The target regains **5d8 + WIS modifier HP**, recovers **two spent hit dice**, and you **remove one non-anomalous condition** (Blinded, Deafened, Poisoned, Frightened, Charmed, Stunned, etc.). The condition removal is surgical — you are physically correcting the underlying cause.

**Uses:** Three per long rest.

**Repositioning tolerance:** The procedure survives forced movement. If the patient or surgeon is dragged, pushed, or carried by an external force, the operation can be maintained. However, **the surgeon cannot voluntarily move** during the procedure.

If you take damage, Medicine check (DC = 10 + damage taken) or healing halved.

**First Aid** scales to **5d6 + WIS**. *(Project PROMETHEUS experimental regenerative compounds — classified Foundation biomedical research program.)*

#### Level 11

**Miraculous Save**  
*Reactive — Once per long rest*  
When a creature within 5 feet of you is **reduced to 0 HP or fails their third death saving throw**, you can use your reaction to deploy your emergency cardiac resuscitation kit — defibrillator pad, epinephrine bolus injector, and compression sleeve. Three actions in under two seconds.

The target **drops to 1 HP instead of dying.** They are conscious and can act on their next turn.

*Side effects: tachycardia, contact burns from the defibrillator, bruised ribs from the compression sleeve. Narrative only — no mechanical penalty.*

**Combat Medic Mastery**  
*Passive*  
**Mass Triage** becomes **twice per long rest**. Each use heals up to 3 allies within 15 feet for **3d6 + WIS modifier HP each**.

#### Level 12

**One More Breath (Capstone)**  
*Enhancement to Miraculous Save — Reactive*  
Your resuscitation kit has been upgraded with **LAZARUS-Light** — a single-dose field compound derived from Foundation necromedicine research (Project LAZARUS, classified).

When you use **Miraculous Save**, the target also gains:
- **3d6 temporary HP**
- **Immunity to being reduced to 0 HP until the start of your next turn** — the compound physically will not allow the body to stop
- **Can immediately take a reaction**

**Uses:** Once per long rest (shared with Miraculous Save — One More Breath IS your Miraculous Save, enhanced).

**First Aid** reaches **6d6 + WIS modifier** (unique to Combat Medic).

*Authorization: LAZARUS-Light is NOT part of your standard loadout. Before a high-risk deployment, Foundation Medical R&D may authorize a single dose for a qualified Combat Medic. This requires Level 4 Medical approval, a documented medical justification, and post-deployment reporting. The dose is signed out, tracked, and accounted for regardless of whether it was used. If not used, it is returned. The DM determines whether mission authorization was granted pre-deployment.*

*Design note: One More Breath is the Combat Medic's capstone — you pulled someone back from the dead, and they got back up swinging. The immunity window is narrow (until your next turn) but wide enough to create a legendary moment. The immediate reaction lets the revived character do something rather than lying there. This is a capstone because it should feel like one: once per mission, you defy death.*

---

---
# Internal Medic — "Surgeon"

**Role:** Foundation medical specialist, preparation, intelligence, VIP treatment  
**Combat Identity:** Flexible mode-select healing — each treatment can heal, cure a condition, OR grant a buff (choose one per action). Prevention and intel support via scanner and reactions.  
**Out-of-Combat Identity:** Classified database access, amnestics (from level 6), institutional authority, research  
**Weakness:** Less raw throughput; pre-combat abilities require planning time  
**Secondary Stat:** INT (pharmacology, medical database interpretation, compound chemistry)  
**Fantasy:** You operate in sterile med-bays with equipment that doesn't officially exist. Your clearance level lets you read the unredacted version.  
**Reports to:** Medical Division (primary). Amnestic operations performed under Medical Division authority — Security can request amnestic support through Medical, but cannot directly order you to deploy amnestics. This preserves clean medical chain of command.

**Specialization Equipment (received at level 3):** Secure Foundation medical terminal (ruggedized tablet with encrypted Foundation Medical Database access), pharmaceutical preparation case (temperature-controlled, pre-mixed compounds and portable compounding station), Class-III surgical kit. *(Note: Amnestic administration kit is NOT issued at level 3. It is issued at level 6 upon completion of amnestics certification. See level 6.)*

*Candidate selection note: Internal Medic candidates are identified during basic medical training based on aptitude in pharmaceutical science, analytical thinking, and institutional judgment. The Foundation doesn't train pharmacologists from scratch — it selects personnel who already demonstrate the aptitude and provides advanced Foundation-specific training.*

### First Aid Scaling (Internal Medic)

| Level | First Aid (Action) | What's Improving |
|-------|-------------------|------------------|
| 1–4   | 2d6 + WIS         | Standard trauma kit |
| 5     | 3d6 + WIS         | Targeted pharmaceutical compounds (analgesics + tissue stimulants) |
| 8     | 4d6 + WIS         | Foundation-grade regenerative compounds |
| 11    | 5d6 + WIS         | Experimental biomedicine from classified research programs |

*Note: Scales 1 level behind Combat Medic in raw dice. But mode-select flexibility (Precision Medicine, Directed Recovery, Directed Triage) makes each action more adaptable — you choose what the situation needs rather than getting raw throughput.*

---

### Levels 3–6 (Full Detail)

#### Level 3 — Specialization Entry

*The Internal Medic receives two core abilities at level 3, establishing their identity immediately. Additional tools arrive at level 4 once the player has had time to learn the core mechanics.*

**Preemptive Treatment**  
*Before mission / Short rest*  
Administer Foundation medical preparations to up to 3 allies. Each treatment ~5 minutes (injection, monitoring, logging). Choose one compound per ally:

- **Immunobooster (Compound IM-7):** Advantage on CON saves against poison and disease for 8 hours. Side effect: mild fever and elevated heart rate for 30 minutes.
- **Trauma Plating (DRG-4):** Subdermal polymer gel. 1d6 + WIS temp HP until next long rest. Side effect: stiffness, reduced fine motor sensitivity.
- **Pain Suppressant (Compound PS-12):** Neural inhibitor blocking pain-panic cascade. Target ignores the first instance of Frightened or Stunned (negated, single use). Side effect: mild emotional flattening for 1 hour.

**Precision Medicine (Mode-Select)**  
*Added to First Aid — from level 3*  

**Mode-select rule:** Each First Aid, you choose ONE mode: **Heal** (roll First Aid dice normally), **Cure** (Purge a condition — no HP healed), or **Buff** (Directed Recovery rider — no HP healed; available at level 4). You cannot combine modes. One action, one effect.

**Cure Mode — Purge:**  
Administer a chelation injector and broad-spectrum antitoxin to remove one condition (blinded, deafened, poisoned, frightened, charmed, etc.).

**Purge charges:** WIS modifier per short rest (minimum 1). At WIS 14 (+2), that's 2 charges. At WIS 16 (+3), that's 3.

**Anomalous conditions:** Purge works on anomalous-source conditions (SCP-designated or clearly supernatural), but requires a **Medicine check** — DC = 10 + half the source entity's save DC (rounded down). On failure, the charge is spent and the condition remains.

*The Internal Medic's core identity — always having the right answer, but only being able to give one answer per turn.*

#### Level 4

*The Internal Medic's toolkit expands with tactical tools, database access, and their enhanced scanner.*

**Directed Recovery**  
*Added to First Aid — third mode option*  
When you use First Aid, you can choose to **Buff** instead of healing or curing: administer one of the following compounds (no HP healed):

- **Brace (Compound BR-3):** +2 AC until start of the **target's** next turn. Side effect: mild soreness for 1 hour.
- **Steady (NCD-1):** Advantage on their next saving throw (before start of the **target's** next turn). Side effect: brief "too sharp" sensation.
- **Reposition (Analgesic Burst):** Target can use their reaction to move up to half speed without provoking.

Duration change from v0.5: buffs now last until start of the TARGET's next turn, not yours. This guarantees the buff is active when an enemy attacks that target, regardless of initiative order.

*Combined with Directed Triage (bonus action), a level 4 Internal Medic can buff an ally (action) AND coach another through self-treatment (bonus action), or cure a condition (action) AND buff with Directed Triage. The mode-select creates tension; the bonus action provides flexibility.*

**Directed Triage**  
*Bonus Action — 2 per short rest — 30 feet range*  
You don't carry quick-deploy patches like the Combat Medic. But you can shout precise medical instructions to a conscious ally within 30 feet, coaching them through self-treatment in real time. **The target must be able to hear you** — a Deafened ally cannot follow verbal instructions.

The target spends one of their own **hit dice** and adds your **WIS modifier** to the roll. They heal for that amount. **The target chooses whether to accept** — if they decline (perhaps they need their hit dice for short rest healing later), your bonus action is not spent and you can target someone else or take a different bonus action.

This costs the ally's hit die but NOT their reaction (changed from v0.6). The ally can still use their reaction normally on their turn.

*"Apply pressure above the wound — no, ABOVE it. Good. Now breathe. You're fine."*

*DM note: Directed Triage consumes ally hit dice, which are also the primary short-rest healing resource. Over a long attrition day (3+ fights), this can drain the party's rest-healing budget. Track this if your campaign runs extended deployments.*

**Classified Consultation**  
*Non-combat — 10 minutes*  
Secure medical terminal access to classified Foundation databases. When encountering anomalous effects, diseases, or unidentified conditions, spend 10 minutes cross-referencing. Medicine check:

- **DC 10:** General nature (anomalous, memetic, biological, chemical, thaumic)
- **DC 15:** Specific cause, progression timeline, aggravating factors
- **DC 20:** The cure or treatment, if one exists in Foundation records

Can also research an SCP pre-mission (DM discretion based on clearance).

*Moved from level 3 to level 4 in v0.7 to reduce ability overload at specialization entry.*

**Clinical Scanner**  
*Replaces base Medic's Eye — upgrade received at level 4*  
Your clinical-grade scanner module replaces the standard biometric scanner firmware. It runs continuously in passive mode.

- **Passive (always on, 30ft):** You always know the condition tier of all allies within 30 feet without using your bonus action (healthy/wounded/bloodied/critical). No action required — the scanner feeds data to your HUD. **Requires you to be conscious** — the scanner runs continuously but you must be awake to interpret the feed.
- **Bonus Action — Active Scan (ally):** Exact HP, max HP, all conditions. Automatic, no check.
- **Bonus Action — Active Scan (enemy):**
  - **(a) Scan:** Condition tier (free) plus one **tactical detail** via **Medicine check — DC set by the DM** based on creature difficulty. Clinical-grade scanner gives **+2 to this check** compared to base Medic's Eye. One piece of intel per scan (elevated cortisol, abnormal thermal patterns, erratic cardiac rhythm, respiratory distress, etc.).
  - **(b) +1 Attack Bonus:** On a **successful enemy scan**, allies who can hear you gain **+1 to attack rolls** against that target until the start of your next turn. Refreshes each turn you successfully scan again. Failed scans do not grant the bonus.

*The +1 bonus comes from you reading the enemy's physiological stress responses and calling out moments of vulnerability ("It flinched — NOW") — reading bodies, not planning killchains. The bonus is earned through successful scanning, not automatic.*

*Moved from level 3 to level 4 in v0.7 to reduce ability overload at specialization entry. The base Medic's Eye (level 2) remains in use until this upgrade.*

#### Level 5

**First Aid** scales to 3d6 + WIS.

**Analysis Paralysis**  
*Reaction — 1 per short rest*  
When an ally within 30 feet is targeted by an attack you can see, you can use your reaction to shout a warning. The attack has **disadvantage**.

Your scanner is passively monitoring your allies' biometrics. When it detects a sudden stress spike — cortisol surge, heart rate jump, involuntary flinch — in one of your patients before they consciously register the incoming threat, you react on instinct. "DOWN!" The warning arrives before the attack does.

This gives the Internal Medic a prevention-based tool that creates a completely different turn structure from the standard heal cycle. It's also your first reaction option beyond Emergency Response — and it's significantly more impactful.

*Reframing note: You're not predicting enemy behavior or tracking attack vectors. You're reading your own patient's fight-or-flight response and reacting to THAT. The scanner detects biometric panic before your ally knows they're in danger. That's medical pattern recognition, not tactical intelligence.*

**Preemptive Treatment Scaling:** Capacity increases to 5 allies. New compound:
- **Metabolic Boost (Compound MB-9):** +5 feet movement speed and advantage on Initiative for 8 hours. Side effect: increased appetite, mild hand tremor.

#### Level 6

**Amnestic Administration**  
*Your turn — Action*  
Foundation-issued amnestic compounds — chemical agents targeting memory-encoding processes in the hippocampus.

**Class-A Amnestic (Compound AM-A):** Autoinjector to a willing or restrained target. Erases preceding hour. WIS save (DC = 8 + proficiency + WIS mod) — fail = hour cleanly erased, success = fragmented impressions remain.

**Combat use:** Administer to incapacitated enemy — erases knowledge of your team.

All doses logged by serial number. Misuse triggers automatic investigation.

*Authorization: Amnestic administration requires certification that you complete between levels 5 and 6. This involves: (1) Advanced neuroscience training on memory formation and pharmacological intervention, (2) Dosage calibration practicals, (3) Security review — your operational record is evaluated for judgment and trustworthiness, (4) Ethics Committee certification — you understand when amnestic use is justified and can articulate the ethical framework, (5) Psychological evaluation — you are stable enough to erase human memories without it affecting your own mental health.*

*Your amnestic administration kit is issued upon certification. It was NOT part of your level 3 starting equipment. Each dose is tracked by serial number. Post-administration reporting is mandatory. The Ethics Committee has standing authority to revoke your certification. Misuse has career-ending consequences.*

*Institutional note: Amnestic deployment is technically a Security operation, not a medical one. The Foundation places amnestics under Medical Division authority because the delivery mechanism is pharmaceutical and proper dosing requires medical expertise. Security can REQUEST amnestic support through your Medical chain of command, but cannot directly order you to deploy amnestics. Your first loyalty is to medical ethics; your second is to operational necessity.*

**Field Triage Protocol**  
*Passive — Triggered by Clinical Scanner*  
After you use your Clinical Scanner's active scan (bonus action) on a creature, your next **First Aid**, **Triage** (via Directed Triage), or **Stabilize** targeting that same creature has **advantage on the roll** (roll healing dice twice, take the higher result; or advantage on the Medicine check if applicable). One use per scan — the bonus is consumed when you treat the scanned target, and resets the next time you actively scan them.

Your scanner's detailed biometric readout — internal bleeding sites, compound fracture angles, toxin concentrations — lets you target treatment with surgical precision instead of working blind. The difference between a medic who scans first and one who doesn't is the difference between a targeted intervention and a best guess.

*Design note: This rewards the IM's scan-then-treat rhythm without adding a new resource. It creates a two-turn setup (scan on bonus action, treat on next action) that distinguishes the IM's deliberate approach from the CM's raw speed. Does not apply to Purge or Directed Recovery — those modes are pharmaceutical, not wound-treatment, and don't benefit from wound mapping.*

---

### Levels 7–9 (Full Detail)

#### Level 7

**Strategic Preparation (Advanced Pharmacology)**  
*Before mission / Short rest*  
Your pharmaceutical case now includes two additional classified compounds, expanding Preemptive Treatment's options. Each treatment still takes ~5 minutes per ally (injection, monitoring, logging). Choose one compound per ally from the full list (IM-7, DRG-4, PS-12, MB-9, and the two new compounds below):

- **Anomalous Resistance (Compound AR-5): Advantage on CON saves against anomalous effects** (anomalous radiation, toxins, parasitic organisms, reality-warping physical effects, thaumic biological interference) **for 8 hours.** A second dose within 24 hours causes vomiting and severe joint pain — do not stack.
  Intravenous infusion via slow-push autoinjector — a translucent amber solution administered over 90 seconds to avoid vascular shock. The compound reinforces cellular membrane integrity and stabilizes biochemical processes against anomalous disruption at the molecular level.
  Side effects: muted color perception (everything looks slightly desaturated), mild emotional dampening (reduced startle response, flattened affect) for the full duration.
  *Cross-departmental: AR-5 is developed and supplied by Foundation Research Division for field medical use. You administer it and understand the dosage, pharmacokinetics, and side effects, but the thaumic stabilization mechanism is Research's domain, not yours. The compound fortifies the body's resistance to anomalous physical effects — not the mind. Mental protection is the Memetic Specialist's domain.*

- **Cellular Fortification (Compound CF-2):** Subcutaneous gel injector — a thick, pearlescent compound administered to the upper arm or thigh. CF-2 triggers a controlled inflammatory response that temporarily hardens cellular walls against a specific damage vector. At the time of injection, you select **one damage type** (fire, cold, lightning, acid, necrotic, radiant, or poison). Target gains **resistance to that damage type** for **8 hours**. Side effects: skin at the injection site becomes unnaturally smooth and slightly translucent (visible if inspected), mild joint stiffness (disadvantage on Acrobatics checks for the first hour as the compound settles). CF-2 cannot be stacked — a second injection before the first expires causes the compounds to conflict, negating both.

*Authorization: AR-5 requires Level 3+ Medical clearance to carry and a pre-mission requisition noting anticipated anomalous exposure. CF-2 is standard Foundation pharmacology — no special authorization beyond your existing Internal Medic credentials, but each dose is still tracked by serial number.*

**Analysis Paralysis** improves: **2 per short rest.**

#### Level 8

**Class-B Amnestics (Compound AM-B)**  
*Your turn — Action*  
The next grade up from Class-A — a stronger amnestic compound targeting deeper memory consolidation pathways. AM-B disrupts not just short-term hippocampal encoding but attacks consolidated long-term memories through targeted protein synthesis inhibition.

**Willing or restrained target:** Autoinjector to the neck or inner arm. Erases up to **24 hours** of memory. WIS save (DC = 8 + proficiency + WIS mod) — fail = targeted time period cleanly erased, success = fragmentary impressions remain (emotions without context, spatial memory without faces, a sense that something happened without knowing what).

**Unwilling target (combat autoinjector):** Make a **melee attack roll** against the target. On hit, the amnestic deploys via spring-loaded combat injector — a pneumatic needle designed to penetrate through clothing and light armor. The target makes the same WIS save. This is loud, violent, and obvious — not subtle fieldwork.

**Narrow therapeutic window:** AM-B dosing must be precise. If you administer AM-B to a target that has received ANY amnestic compound in the past 48 hours, the target must make a **DC 14 CON save** or suffer seizures — **incapacitated for 1 round** and takes **2d6 psychic damage** from neurological trauma. Even on a success, the target has disadvantage on INT checks for 1 hour. You know this. The Foundation drilled overdose protocols into you during certification.

All doses logged by serial number. Post-administration reporting mandatory.

*Authorization: Class-B amnestics require the same certification as Class-A (completed at level 6). The combat autoinjector variant requires an additional field-deployment endorsement — documented proof that you can make dosing decisions under fire without over-administering. Your operational record between levels 6 and 8 serves as that proof.*

**Foundation Medical Authority**  
*Your turn — Action — Once per long rest*  
You are issued a **Medical Override keycard** — Level 4 Medical clearance, encoded to your biometrics. When you present this card and invoke medical authority, one Foundation system, locked supply cache, restricted medical file, or NPC must comply with a reasonable medical directive.

Examples of valid use: opening a sealed medical supply locker during an emergency, accessing a restricted patient's medical records to determine treatment, overriding a quarantine lock when a patient inside requires immediate care, commandeering medical equipment from another department, or pulling rank on triage priority decisions.

**Scope limitations:** Medical Override operates within medical contexts only. It opens medical supply caches, accesses restricted patient records, overrides quarantine locks when medically necessary, and grants authority over triage decisions. It does **NOT** open containment cells, override security lockdowns, grant command authority over non-medical personnel, or bypass operational security protocols. Using it outside medical contexts triggers a mandatory review — and the Foundation will determine whether your use was justified.

*"Medical override, Level Four. Open it."*

*Institutional note: The keycard is not a skeleton key. It is a narrow grant of authority within your professional domain. The Foundation trusts you with it because you have demonstrated judgment with amnestics, experimental compounds, and classified information for years. Abuse it once and it is revoked permanently.*

**First Aid** scales to **4d6 + WIS.** *(Foundation-grade regenerative compounds — biofoam sealants with accelerated clotting factors, dermal matrix patches that scaffold new tissue growth, and pharmaceutical-grade analgesic cocktails that go well beyond standard-issue painkillers.)*

#### Level 9

**Experimental Protocol**  
*Your turn — Full Round Action (action + bonus action) — Once per long rest*  
Restricted experimental compounds from Project PROMETHEUS — the Foundation's classified regenerative medicine research program. These are not field-grade pharmaceuticals. Each compound comes in a sealed, temperature-controlled case with a tamper-evident strip and a serial number that Medical R&D tracks personally.

- **Regenerative Compound (RC-7): Heals 4d6 + WIS modifier HP. All non-anomalous conditions removed** (blinded, deafened, poisoned, frightened, charmed, stunned, etc. — if the source is non-anomalous, it's gone). **DC 12 CON save** or suffer nausea — **disadvantage on attack rolls** for 1 round.
  Intravenous push via high-pressure autoinjector — a viscous, faintly luminescent blue-green solution. RC-7 triggers a cascade of accelerated cellular regeneration that is, by any honest medical assessment, beyond what current science should produce. Visibly unnatural healing: wounds seal in seconds, bruising fades before your eyes, broken bones audibly click back into alignment. Anyone watching knows this is not normal medicine.
  Side effects: intense hunger for 4 hours, mild hand tremor for 1 hour, faint luminescent tracery visible under the skin at the injection site for 24 hours.
  *(RC-7 is a product of Project PROMETHEUS, derived from classified biomedical research. Its exact origins are above your clearance level. What you know: it works, the dosage is precise, and Foundation Medical R&D trusts you enough to carry it.)*

- **Emergency Containment Dose (ECD-3):** Intramuscular injection — a clear solution in a red-striped autoinjector. ECD-3 does not heal. It **suppresses one anomalous effect** currently affecting the target for **1 hour** — the effect is paused, not cured. The anomalous contamination, mutation, or condition is still present but dormant, buying time for proper treatment or containment. When the hour expires, the effect resumes where it left off. Side effects: low-grade fever, fatigue, and a metallic taste in the mouth for the suppression duration.

*Authorization: RC-7 is not a standard-carry compound. Each dose must be requisitioned from your assigned Site's medical facility before deployment. This requires Level 3+ Medical clearance and a documented medical justification ("high-risk containment breach response" is sufficient; "just in case" is not). Post-administration reporting is mandatory. Unused doses are returned and logged.*

**Directed Triage** improves: **3 per short rest.**

---

### Levels 10–12 (Full Detail)

#### Level 10

**Protocol HIPPOCRATES**  
*Your turn — Action — Once per long rest*  
Invoke a pre-authorized emergency medical directive — Protocol HIPPOCRATES, a standing order signed by the O5 Council years ago that grants temporary emergency medical authority to Level 4+ Medical Officers in immediate life-threatening situations.

When triggered, all Foundation personnel and systems in the immediate area must comply with your medical directives for up to **30 minutes**. One NPC or Foundation system must comply with a reasonable medical order — this goes above Site Directors in medical matters.

**Scope limitations:**
- Medical directives only (not operational, not security, not containment)
- Immediate area only (not Site-wide)
- Time-limited (30 minutes maximum)
- Subject to mandatory post-incident review by Medical Division and O5 oversight
- Abuse triggers automatic O5 investigation with career-ending consequences

*You are not an O5. You are invoking a protocol that the O5 Council pre-authorized for exactly this situation. The authority is enormous but narrowly scoped. Use it wisely — every invocation generates a report that the O5 Council reads.*

*Career milestone note: By level 10, you are not a "field medic" anymore. You are one of the Foundation's senior Medical Division specialists — the equivalent of a department head with decades of demonstrated loyalty, judgment, and institutional trust. Your authority comes not just from medical skill but from years of proving you can be trusted with power. The Foundation has watched you handle amnestics, experimental compounds, and classified information without incident. Protocol HIPPOCRATES is the reward for that trust.*

**Experimental Protocol Scaling:**  
RC-7 scales to **6d6 + WIS.** Experimental Protocol becomes usable **twice per long rest.** Gains a third compound option:

- **Anomalous Purge (Compound AP-1):** Intramuscular injection via a black-striped autoinjector — the only compound in your kit with a biometric lock requiring your thumbprint to deploy. AP-1 attacks anomalous biological contamination at the cellular level, forcing the body to reject foreign anomalous material the way an immune response rejects a transplant. Target makes a **CON save (DC 18)**. On success, one **anomalous physical or biological effect** is **permanently cured** — the body expels the contamination entirely. On failure, the effect is **suppressed for 24 hours** (as ECD-3, but longer duration). Side effects regardless of outcome: crushing fatigue (disadvantage on STR and DEX checks) for 24 hours, nosebleeds, and a persistent low-grade headache. A second dose within 48 hours risks organ failure (DM discretion). *Scope: AP-1 treats physical and biological anomalous effects only — anomalous radiation exposure, cellular mutation, toxin-class anomalies, parasitic organisms, and similar. Mental anomalous effects (domination, memetic compulsions, cognitive hazards) are outside AP-1's pharmacological mechanism and remain exclusively Memetic Specialist territory via mnestic protocols.*

*Authorization: AP-1 requires Level 4 Medical clearance and individual dose authorization from Project PROMETHEUS oversight. Each dose is serialized, biometric-locked, and tracked from synthesis to administration or return. Post-use tissue samples from the treated patient are mandatory.*

#### Level 11

**Class-C Amnestics (Compound AM-C)**  
*Your turn — Action (combat) / Non-combat — 10 minutes (guided cognitive interview)*  
The highest grade of amnestic you will ever be certified to administer in the field. AM-C attacks deep long-term memory through a combination of protein synthesis disruption and guided neurochemical pathway dissolution. This is surgical-grade memory work.

**Standard administration (combat or emergency):** Autoinjector to a willing, restrained, or incapacitated target. Erases up to **one week** of memory. WIS save (DC = 8 + proficiency + WIS mod) — fail = targeted week cleanly erased, success = emotional residue remains (the target feels uneasy about a place, distrusts a person they can't remember meeting, has dreams they can't explain).

**Guided cognitive interview (10 minutes, non-combat):** With a willing and conscious target in a controlled environment, you can perform **targeted erasure** — removing specific memories while leaving the surrounding timeline intact. You talk the target through the memory, using their verbal and physiological responses to isolate the neural pathway, then administer AM-C at the precise moment of recall to dissolve only that thread. Medicine check DC 15 for clean excision; failure erases a broader window than intended (DM determines collateral memory loss).

**Overdose risk:** AM-C administered to a target who has received ANY amnestic in the past 72 hours triggers a **DC 16 CON save** — failure causes seizures (incapacitated 1 round, 3d6 psychic damage) and permanent loss of 1d4 random non-critical memories (DM narrates). Success still causes 1 hour of confusion and disorientation.

Side effects (all administrations): 24-hour headache, intermittent deja vu episodes for 1 week, mild anterograde amnesia (difficulty forming new memories) for 4 hours post-injection.

*Authorization: Class-C amnestic certification is a separate endorsement beyond your Class-A/B credentials. The guided cognitive interview technique requires an additional 40-hour practicum under Ethics Committee supervision. Targeted erasure is powerful enough that the Ethics Committee maintains a standing review of every Class-C deployment. Misuse of targeted erasure — erasing memories for convenience rather than necessity — is grounds for immediate certification revocation and possible detention.*

**First Aid** scales to **5d6 + WIS.** *(Experimental biomedicine from classified research programs — compounds that blur the line between conventional pharmacology and the output of Project PROMETHEUS. Your trauma kit at this level contains things that would revolutionize civilian medicine if they were ever declassified.)*

**Fortify**  
*Added to Directed Recovery — fourth mode option*  
When you use First Aid in **Buff** mode, you can now choose **Fortify (Compound FR-1)** — a subdermal reactive gel injected beneath the skin that hardens on impact, distributing kinetic energy across the body's surface. Target gains **resistance to all damage** until the start of their next turn.

Side effects: the gel contracts as it hardens, causing sharp pain across the injection site. Target takes **1d4 psychic damage** (pain, not cognitive — cannot be reduced) when Fortify is applied. After the effect expires, the gel dissolves into the bloodstream — mild nausea and skin tenderness for 1 hour.

**Once per long rest.** FR-1 is a single-use compound — the reactive gel cannot be reapplied until the body fully metabolizes the previous dose.

*Design note: Fortify gives the IM a powerful defensive option but at the cost of their entire First Aid action (no healing) and a long-rest resource. It's a clutch play for keeping the tank alive through a devastating hit, not a routine buff. The 1d4 pain cost prevents trivial use on healthy allies.*

**Analysis Paralysis** improves: **3 per short rest.**

#### Level 12

**Lazarus Protocol (Capstone)**  
*Your turn — Full Round Action (action + bonus action) — Once per long rest*  

Revive a creature that **died within the last minute.** You must be adjacent to the body for the full round. The target returns at **1 HP** with the following consequences:

- **Disadvantage on all attack rolls, ability checks, and saving throws for 24 hours.** The body is barely functional after being chemically restarted — every system is running on emergency power. Muscles seize, vision blurs, hands shake.
- **WIS save (DC 15)** or gain a temporary mental condition lasting **1d6 days** (DM's choice — catatonia, paranoia, night terrors, dissociative episodes, or compulsive repetition of final moments before death). Death leaves a mark on the mind even when the body recovers.
- **Permanent anomalous residue:** The Lazarus Protocol does something to the boundary between life and death that the Foundation cannot fully explain. The revived individual carries a minor anomalous trait that **never goes away** — DM determines specifics (faint bioluminescence in the dark, animals become uneasy near them, they no longer dream, a room they sit in drops 2 degrees, their reflection blinks independently). This is not cosmetic flavor. It is a real, detectable anomalous signature.

**Vital Transfer — HP Cost:** When you administer the Lazarus Protocol, you **drop to half your current HP (rounded down, minimum 1)**. This cost cannot be reduced, prevented, or healed until you complete a short rest (your body needs time to restabilize).

**Vital Transfer — Residual Anomaly:** You gain the **Residual Anomaly** condition: a minor, temporary anomalous effect from your proximity to the boundary between life and death. The DM rolls or selects from a table (examples: your shadow moves independently for 1d4 hours, you hear faint whispers in empty rooms until your next long rest, your blood temporarily runs cold to the touch, you forget one non-critical personal memory). Residual Anomaly clears on your next long rest.

Foundation necromedicine research (Project LAZARUS, classified). The deployment kit is a sealed hardcase containing four compounds administered in precise sequence: cardiac restart agent (epinephrine derivative at 50x standard concentration), neural preservation compound (must reach the brain within 60 seconds of death — it halts neuronal apoptosis by flooding synapses with a cryoprotectant analogue), mitochondrial reactivation serum (restarts cellular energy production from the organelle level up), and a massive dose of RC-7 (the regenerative compound forces the newly restarted body to begin repairing itself immediately). The cardiac restart agent synchronizes to YOUR heartbeat as a pacing template — the strain on your cardiovascular system is immediate and brutal.

*"Death is a containment breach. Recontain the subject."*

*Authorization: The Lazarus Protocol kit is NOT standard medical equipment. It exists in a sealed case stored at your assigned Site's medical facility. To deploy it, you must have requisitioned the kit before the mission — this requires Level 4 Medical approval and a specific high-risk deployment justification — or have emergency authorization from Protocol HIPPOCRATES. After use, you file a full incident report. The revived individual is placed under 72-hour medical observation and Foundation monitoring protocols.*

*Containment implications: The revived individual now carries permanent anomalous residue. By Foundation classification standards, they may be considered an anomalous entity (E-class or equivalent) and are subject to Foundation monitoring protocols. If the anomalous residue manifests dangerously, containment procedures apply. The DM should make the anomalous residue a persistent narrative element — the revived character is Changed, and the Foundation is watching. Using Lazarus Protocol to save someone's life may condemn them to Foundation oversight. This should weigh on every decision to use it.*

---

---
# Memetic Specialist — "Inoculator"

**Role:** Cognitive defense specialist, mental protection, Antimemetics Division-adjacent  
**Combat Identity:** Steady support — consistent healing plus scaling offensive intelligence; shifts into dominant role when mental threats appear  
**Out-of-Combat Identity:** Anomalous threat assessment, cognitive diagnostics, late-game infiltration  
**Weakness:** Lowest raw healing throughput; offensive tools build gradually; effectiveness outside specialty depends on encounter design  
**Secondary Stat:** INT (memetic science, anomalous psychology, behavioral analysis, compound chemistry)  
**Fantasy:** You started as a medic. The Antimemetics Division saw something in your CRV (Cognitive Resistance Value) scores — a Foundation-developed metric measuring a subject's innate resilience to memetic and cognitohazardous influence. They gave you tools. Then training. Then conditioning. Then weapons. You didn't stop being a medic — but you became something else too.

---

### Hybrid Progression — The Story Your Levels Tell

The Memetic Specialist is unique among the three medic specializations because **your identity shifts over the course of the campaign.** This isn't accidental — it reflects a realistic Foundation career trajectory.

**Levels 3–5: You are a medic.** Your kit is medical: a CRV scanner (Division-loaned diagnostic tool), prophylactic mnestics (medical countermeasures), and your own training. The Antimemetics Division loaned you equipment because your team is entering a hazard zone. You report to Medical Division.

**Levels 6–7: You are being recruited.** The Division starts trusting you with operational equipment — a counter-memetic emitter, advanced conditioning. Your handler checks in more often. You're invited to Division briefings. You're learning things Medical Division doesn't teach.

**Level 8+: You're Division now.** Cognitive Strike payloads require Division certification. You passed. You've been fully inducted into the Antimemetics Division. You still heal — old habits die hard, and the team still needs a medic. But your primary mission is cognitohazard containment and elimination. Your equipment comes from Division requisitions. Your clearance is Division-specific. You know things Medical Division personnel will never know.

**Reports to:** Medical Division (levels 3-7) → Dual reporting, Medical + Antimemetics Division (level 8+). *"You serve two masters. Your team thinks you're their medic. The Antimemetics Division thinks you're their field agent. Both are right. Both have expectations. When those expectations conflict — and they will — you choose."*

---

### Equipment Access Gates

Equipment is issued at specific levels based on demonstrated competence and institutional trust, not all at once.

| Level | Equipment Issued | Source | Narrative |
|-------|-----------------|--------|-----------|
| 3 | CRV scanner (portable), mnestic administration kit (Class-W/X only) | Division-loaned, through Medical | "The Division issued you a scanner and basic mnestics for this deployment. Medical countermeasures." |
| 4 | Class-X mnestic autoinjectors (emergency decontamination) | Division-authorized, through Medical | "Your Division handler signed off on emergency cognitive decontamination supplies." |
| 5 | SCRAMBLE-derivative eyewear | Division-issued personal protective equipment | "Your CRV scores and field performance earned you Division protective gear. You signed for it." |
| 6 | Counter-memetic emitter unit | Division-issued operational equipment | "This isn't medical equipment. This is Division hardware. You signed a different form for this one." |
| 7 | Class-Y mnestic (sustained-release conditioning) | Division pharmaceutical | "Class-Y is not a medical countermeasure. This is operational conditioning. You're being changed." |
| 8 | **BL payload kit (restricted)** | **Division weapons certification** | **"You've been certified for Berryman-Langford offensive payloads. You're one of them now."** |
| 9 | Class-Z mnestic (full purge) | Division classified access | "Class-Z is the highest mnestic grade in Foundation inventory. Its existence is classified above your old clearance level." |
| 10 | FORGOTTEN-7 (experimental antimemetic) | Division covert operations | "Experimental. Even within the Division, access is restricted." |
| 11 | Cognitohazard ████-Aleph (Identity Fracture) | Division Thaumiel-class authorization + Ethics Committee waiver | "Fewer than 200 people know this exists. You're one of them." |
| 12 | Containment-Class Inoculation protocol | Division capstone trust | "Permanent neural restructuring. The Division trusts you with this because you've earned it." |

---

### Specialization Equipment (received at level 3)

Portable CRV scanner (Division-loaned for this deployment — reads Cognitive Resistance Value, neural activity baselines, and cognitive compromise indicators), mnestic administration kit (Class-W prophylactic and Class-X emergency doses only — medical countermeasures authorized through Medical Division chain of command), standard Foundation field medical kit (carried over from base medic training).

*Note: You do NOT receive SCRAMBLE eyewear, counter-memetic emitters, or BL payload kits at level 3. Those are issued later as you earn Division trust. At level 3, you're a medic with a loaned scanner and some specialized pharmaceuticals.*

### First Aid Scaling (Memetic Specialist)

| Level | First Aid (Action) | What's Improving |
|-------|-------------------|------------------|
| 1–4   | 2d6 + WIS         | Standard trauma kit |
| 5     | 3d6 + WIS         | Better compounds |
| 8     | 4d6 + WIS         | Foundation-grade regenerative compounds |
| 11    | 5d6 + WIS         | Advanced biomedicine |

*Note: Same scaling as Internal Medic. The Memetic Specialist's value is in Psychometric Reading's scaling damage bonus and their anti-mental toolkit.*

---

### Levels 3–6 (Full Detail)

#### Level 3 — Specialization Entry

*You are a medic. The Division loaned you diagnostic equipment and prophylactic compounds because your team is entering a memetic hazard zone. Your training is medical — cognitive first aid, prophylactic treatment, behavioral observation.*

**Memetic Inoculation**  
*Before mission / Short rest*  
Administer Class-W mnestic to up to 3 allies via autoinjector. Mild prophylactic — reinforces natural memory-consolidation pathways against external cognitive influence.

Each target gains advantage on their next WIS save against a compulsion, charm, or memetic effect. Single use — once spent, the compound has metabolized.

Side effects: mild headache, elevated heart rate, heightened sensory sensitivity for ~2 hours.

*Authorization: Class-W mnestics are the mildest grade — medical countermeasures rather than operational tools. Your Medical chain of command authorized these because your team is deploying into a known or suspected cognitohazard zone. The Division supplied them; Medical approved the use.*

**Psychometric Reading**  
*Your turn — Bonus Action — 30 feet range*  
Analyze a target using your CRV scanner (for allies) or behavioral observation training (for enemies).

- **On an ally:** Compare neural activity against baseline CRV profile stored in the scanner's database. Any deviation flags as cognitive compromise — you know immediately if they're under memetic influence. No check required. *(This is what CRV scanners are designed for — measuring cognitive resilience and detecting anomalous neural interference.)*

- **On an enemy (mechanical):** The next **two allies** to **hit** that target add **+1d4 to the damage**. The scanner overlays biometric targeting data on the enemy — structural vulnerabilities, injury sites, compromised joints, thin armor points, pain responses — that your allies can exploit for maximum effect. The bonus is precision targeting from real-time biometric intelligence, not prediction.

- **On an enemy (DM narrative):** Separately, the DM provides one **behavioral prediction** — the enemy's likely next target, whether it's about to use a special ability, its emotional state (panicking, focused, desperate, preparing to flee), or a tactical read ("it's favoring its left side — mobility compromised"). This prediction is narrative, not mechanical, but gives the team real intelligence to work with.

  *(The damage bonus comes from the scanner's biometric overlay — your allies see where to hit. The behavioral prediction comes from YOU: body language, stress responses, behavioral cues, micro-expressions, posture shifts, breathing patterns, pain indicators. This is not the CRV scanner — it's your Antimemetics Division behavioral analysis training. Understanding how minds work means understanding how bodies betray intention. Two separate tools: the scanner marks targets, your training reads intentions.)*

No uses per rest — scanner runs on battery power, behavioral observation is a skill.

*Clarification: The bonus applies to DAMAGE rolls on a hit, not attack rolls. This is consistent with similar mechanics (Hunter's Mark, Hex) and prevents the scaling from becoming too powerful at higher tiers.*

**Cognitive Triage**
*Bonus Action — 2 per short rest — 30 feet range*
When you use Psychometric Reading on an ally and detect **no cognitive compromise**, you can relay their stable CRV readout back to them — showing them, in real time, that their mind is intact. The visual confirmation of neural stability steadies them.

The target gains **advantage on their next saving throw** (any type) before the start of your next turn.

**Uses:** 2 per short rest.

This gives you a second mode for your bonus action. In standard combat: scan an enemy for damage support, or scan an ally for save protection? In mental encounters: the decision shifts — scan the compromised ally (detection) or scan the stable ally (protection against the next wave)?

*"Your CRV is green. 340. You're clean. Stay that way."*

**Residual Imprint**  
*Reactive — Proficiency bonus uses per long rest*  
When an ally within 30 feet succeeds on a saving throw (any type except death saving throws), the post-threat norepinephrine surge briefly enhances their cognitive performance — a neurochemical window your CRV scanner detects in real time. You flag the spike, call it out, and the ally capitalizes on their own brain's heightened state before the window closes.

That ally gains **advantage on their next ability check or saving throw** before the end of the current combat encounter.

**Uses:** Proficiency bonus per long rest.

**Restriction:** Cannot trigger from a saving throw where the ally already had advantage granted by your Cognitive Triage. Stacking your own buffs into a chain cheapens both tools — Cognitive Triage protects the save, Residual Imprint rewards natural resilience. If they needed your help to pass, the imprint doesn't form.

Your scanner logs survived exposures automatically — threat frequencies, neural resistance signatures, the specific pattern of a mind that held. Over time, this data teaches you to recognize the afterimage of successful resistance before the ally even knows they shrugged it off. The imprint fades fast. But for a few seconds, they're sharper than they were.

*"You resisted that. Your CRV spiked to 410 on contact and held. Whatever it just tried, your brain already knows how to reject it. Use that window."*

*Design note: This gives the Memetic Specialist a second reaction option at level 3, but it triggers on success rather than incoming threat. It rewards encounters where saves are frequent (exactly the encounters the MS is designed for) without competing with Cognitive Triage (which fires before the save). Proficiency bonus per long rest keeps it meaningful but limited — at level 3 that's 2 uses, scaling to 4 by level 9. Does not trigger on death saves to prevent interaction with the Combat Medic's death-save ecosystem.*

#### Level 4

**Cognitive Decontamination**  
*Your turn — Action*  
Administer emergency Class-X mnestic injection. Floods neural pathways, forcing re-evaluation of all current cognitive states.

Touch a creature. They immediately repeat a WIS save they previously failed against a charm, compulsion, fear, or memetic effect, **with advantage**.

If the original effect didn't allow a save, target makes WIS save against DC 15. Success = suppressed for 1 hour. Failure = too deeply integrated.

**Immunity window:** On a successful re-save, the target is **immune to the same effect from the same source** until the start of their next turn. The mnestic flush creates a temporary neurochemical buffer that resists immediate re-application. This immunity does NOT apply on a failed re-save — the mnestic didn't clear the effect, so no buffer forms.

**1 per short rest.** You carry one Class-X autoinjector per deployment cycle — they're expensive and the side effects of stacking doses include seizures. You restock during rest periods.

Side effects: severe headache (1-2 hours), nosebleed, disorientation for 30 seconds post-injection.

*Authorization: Class-X mnestics are emergency medical countermeasures — stronger than Class-W, but still within medical authorization scope. Your Division handler signed off on your carrying these. Administration is a medical act (you're treating cognitive compromise), not an operational one.*

**Memetic Inoculation Scaling:** Higher-grade mnestic (Class-W+). Now inoculate up to 5 allies, and each dose grants advantage on the next TWO WIS saves instead of one.

#### Level 5

**First Aid** scales to 3d6 + WIS.

**Pattern Recognition**  
*Passive*  
Proficiency in WIS saves (or expertise if already proficient). Advantage on all saves against being Charmed.

This isn't something you learned in a class. This is the result of Antimemetics Division conditioning that began before you joined this team — controlled exposure therapy, thousands of hours of cognitive resistance drills over years of Foundation service, regular mnestic conditioning cycles that physically altered your neural architecture. Your CRV is in the top 1% of Foundation personnel. The Division identified you early because of that score.

*Backstory note: The "thousands of hours" of conditioning didn't happen between levels 4 and 5. It's been happening since the Foundation identified your CRV potential — possibly during intake, possibly during basic training. Your high CRV is WHY the Division loaned you their equipment at level 3. The level 5 unlock represents your conditioning reaching a threshold where it provides passive combat benefit, not the completion of a training program.*

**SCRAMBLE Eyewear**  
*Passive — Division-issued at level 5*  
Your SCRAMBLE-derivative smart glasses are Division personal protective equipment, issued after your field performance and CRV scores proved you're worth protecting with Division hardware. The glasses run pattern-recognition algorithms that identify and disrupt known cognitohazardous patterns.

**Once per encounter**, you have advantage on a WIS saving throw against a cognitohazard or memetic effect (visual, auditory, or otherwise — the glasses have a broad-spectrum pattern library). After the first save, the glasses need time to recalibrate to the specific anomaly's signature.

If the glasses are removed or destroyed, this benefit is lost until replaced or repaired (Division requisition).

*SCRAMBLE scales at higher levels:*
- *Level 5: Once per encounter — advantage on first WIS save against cognitohazard*
- *Level 8: Twice per encounter — recalibration time halved*
- *Level 11: Always active — advantage on ALL WIS saves against cognitohazards while worn (by this point, the glasses are neurally paired to your conditioning)*

*Lore note: SCRAMBLE technology famously failed against SCP-096. The Foundation knows their gear has limitations. These are SCRAMBLE-derivative — improved, but not infallible. They complement your conditioning; they don't replace it.*

**Psychometric Reading Scaling:** The +1d4 damage bonus increases to **+1d6** (improved biometric targeting resolution from accumulated field calibration data). Still applies to the next two allies to hit the target.

#### Level 6

*The Division starts trusting you with operational equipment, not just medical tools. You're being recruited.*

**First Aid** stays at 3d6 + WIS (scaled at L5).

**Counter-Memetic Barrier**  
*Your turn — Action — Concentration (up to 1 minute) — Once per long rest*  
Deploy a portable SCRAMBLE-derivative emitter array. 15-foot radius, moves with you (clipped to gear):

- **Field Effect:** Allies gain advantage on WIS saves against mental effects. Enemies have disadvantage on attempts to charm, frighten, or compel. Cognitohazardous objects are temporarily suppressed within the field. The emitter broadcasts broad-spectrum neural white noise that raises the cognitive resistance threshold within the field, disrupting incoming memetic carrier signals before they can fully integrate with the target's neural processing.
- **Mental Immunity:** Concentration on the Barrier cannot be broken by mental effects (Stun, Charm, Domination, Fear from mental/memetic sources). The emitter device sustains itself even if the operator's mind is temporarily compromised — the hardware keeps running on its last calibration. This prevents the catch-22 where the barrier's concentration breaks from the exact effects it's designed to protect against.
- **Physical Hardening:** When physical damage forces a concentration save for the Barrier, you make that save **with advantage**. You still make the save (it's not automatic), but the hardware's resilience gives you a second chance.

Concentration = monitoring and adjusting emitter frequency in real time.

> *Design note: Physical Hardening at CON +1 vs DC 10 drops failure rate from 40% to 16% per hit. The emitter array has redundant power cells and auto-calibrating frequency oscillators — a hit that rattles you doesn't immediately crash the device.*

*Authorization: This is the first piece of operational (non-medical) Division equipment you receive. You signed a different requisition form for this one — Division, not Medical. Your Division handler is now checking in regularly. This is the transition point.*

**Advanced CRV Scanner (Firmware v3.0):** When scanning an ally, you now learn the *specific* effect and its likely *source* — not just "compromised" but "Class-IV visual cognitohazard consistent with SCP-████'s pattern." When scanning an enemy, you also learn their WIS score (useful for planning Cognitive Strike deployment later — if you make it that far).

---

### Levels 7–9 (Full Detail)

#### Level 7

*The Division is changing you. Class-Y conditioning is not treatment — it is modification. Your handler visits more frequently. You attend Division briefings now. The team notices you reading scanner data that isn't in their feed.*

**Memetic Hardening (Extended Mnestic Conditioning)**  
*Your turn — Action — 8 hours duration — Touch range — One willing creature*

**Trade-off — Cognitive Lockdown:** The target's mind becomes a closed system. For the duration, the target **cannot benefit from beneficial mental effects** — bardic inspiration analogs, morale effects, telepathic communication, or any ability that requires receptive cognition. The mnestic hardens against ALL external cognitive influence, beneficial or hostile.

For 8 hours, the target gains:
- **Advantage on all WIS saving throws** against mental and memetic effects
- **Resistance to psychic damage** (halved)

**Exception — Operator Recognition:** The Memetic Specialist who administered Hardening can still use their own abilities (Cognitive Warning, Cognitive Triage, Cognitive Decontamination) on the Hardened target. The Class-Y compound is keyed to the operator's specific neurochemical signature during administration — the firewall recognizes you as a trusted source. Another Memetic Specialist's abilities would be blocked.

Administer a sustained-release Class-Y mnestic implant. The compound integrates into the target's neural architecture over 30 seconds, establishing a persistent cognitive firewall that filters all incoming mental influence through a resistance threshold.

Side effects: emotional blunting, reduced dream activity, mild depersonalization for 2-4 hours after the compound metabolizes. Targets describe feeling "sealed in" — present but insulated from the world.

*Authorization: Class-Y is not a medical countermeasure. It is operational conditioning — you are temporarily rewriting someone's neural response patterns. This compound is issued under Division authority, not Medical. Your Division handler approved it. Your Medical chain of command was notified, not consulted.*

**Cognitive Warning**  
*Reactive — 1 per short rest (scales at L9, L11)*  
When an ally within 30 feet would be forced to make a WIS saving throw, you can use your reaction to shout a warning before the effect fully engages. The ally gains **advantage on that save**.

Your CRV scanner detected the incoming cognitive intrusion — a neural interference pattern, anomalous frequency spike, or memetic carrier wave — milliseconds before it reached the target. You don't need to understand the specific threat. You've seen enough scanner signatures to know what a hostile memetic pulse looks like, and your reaction is trained to the point of reflex.

**Uses:** 1 per short rest at L7-8. Scales to 2/SR at L9-10. Scales to 3/SR at L11+.

*This fills the Memetic Specialist's reaction gap. Levels 3-6 offered only Emergency Response and Residual Imprint — physical movement and success-riding. Cognitive Warning is your first dedicated mental-defense reaction. It does not compete with Cognitive Sovereignty (L12 capstone) — Warning gives the ally a better chance to resist; Sovereignty shields the ally and absorbs the effect entirely.*

**Cognitive Decontamination Scaling:** Improves to **2 per short rest**. You now carry a pneumatic mnestic delivery system (Division-issued, belt-mounted) that extends range to **15 feet** — no longer requires touch. The launcher fires a single-use Class-X microdose dart that penetrates skin on impact and delivers the mnestic payload in under one second. Faster, safer, and you don't have to cross a firefight to reach the compromised ally.

#### Level 8 — Division Induction

*You completed the weapons certification. You passed the psychological evaluation. You signed documents you can never discuss. Your BL payload kit was issued — not through Medical, through Division Armory. You're one of them now. The team's medic is also carrying cognitohazardous weapons. Whether they know that yet depends on how you've played it.*

**Cognitive Strike (Berryman-Langford Offensive Payload)**  
*Your turn — Action — Once per short rest — 30 feet range*  
Deploy a weaponized Berryman-Langford cognitohazard against a target you can see within 30 feet. You select the payload type before deployment. The target makes a **WIS save (DC = 8 + your proficiency bonus + your WIS modifier)**.

**On a failed save**, the target suffers one of the following (your choice at deployment):

- **Cognitive Overload (Visual Payload):** A compressed memetic pattern delivered via your CRV scanner's emitter array — the target's visual cortex is flooded with self-referencing pattern data. The target is **Stunned** until the end of their next turn. Their eyes are open but processing nothing useful.
- **Implanted Compulsion (Subliminal Audio Payload):** A subaudible carrier frequency containing an embedded behavioral directive. The target **uses its movement on its next turn to move up to its speed in a direction you choose**. It does not provoke opportunity attacks from this movement. The target is aware something is wrong but cannot override the impulse.
- **Sensory Blackout (Neural Disruption Payload):** A broad-spectrum neural interference burst that temporarily severs sensory processing. The target is **Blinded and Deafened** until the end of their next turn. Complete sensory isolation — they can't see, can't hear, and their proprioception is scrambled.

**On a successful save:** The payload partially engaged but didn't fully integrate. The target has **disadvantage on their next attack roll** as residual cognitive noise disrupts their focus.

*Authorization: BL payloads require Division weapons certification. The training covers: (1) BL memetic architecture and payload construction theory, (2) target selection and payload matching based on cognitive profile, (3) safety protocols — friendly-fire prevention, minimum safe distances, SCRAMBLE confirmation before deployment, (4) environmental containment procedures for lingering memetic residue, (5) self-protection during deployment via your own conditioning. This is a weapons qualification, not medical training.*

*Ethics note: Cognitive Overload and Sensory Blackout are classified as non-lethal incapacitation — equivalent to flashbangs in the Foundation's use-of-force framework. Implanted Compulsion (temporary override of free will) requires post-operation documentation and is flagged for Ethics Committee review in the after-action report.*

**SCRAMBLE Eyewear Scaling:** Recalibration time halved. Now provides advantage on the first **two** WIS saves against cognitohazards per encounter (up from one).

**First Aid** scales to 4d6 + WIS.

#### Level 9

*You carry the highest-grade mnestic in Foundation inventory. Its chemical formula is classified above the clearance level you held six months ago. You know what it does because you've seen it work — on others, and now on yourself during conditioning. The Division trusts you with Class-Z because you've demonstrated you can handle what it reveals.*

**Antimemetic Protocol (Full Cognitive Purge)**  
*Your turn — Action — Once per long rest*  
Administer a Class-Z mnestic — the highest grade in Foundation inventory. A single autoinjector, contents temperature-sensitive and individually serial-numbered. The compound hits like a detonation inside the skull: every neural pathway fires simultaneously, every suppressed memory surfaces, every implanted thought is dragged into conscious awareness and rejected.

Touch a creature (including yourself). **All mental effects currently affecting the target are immediately removed**, regardless of source, duration, or save DC. Domination, memetic compulsion, cognitohazardous influence, anomalous charm, implanted suggestions, fear effects — everything. Gone.

The target is then **immune to all new mental effects for 10 minutes**. Their neural architecture is in a refractory state — nothing gets in. Nothing. This immunity cannot be bypassed, suppressed, or dispelled by any effect short of Keter-class reality alteration (DM discretion).

Side effects: **1d4 hours of hypercognitive state** — the target perceives connections, patterns, and implications in everything they observe. This is not useful. It is overwhelming. Concentration checks during this period are made at **disadvantage**. The target may experience intrusive recall of memories they had forgotten or suppressed. The Foundation provides post-exposure counseling.

*Authorization: Class-Z's existence is classified above standard Foundation clearance. You received access through Division channels — your handler requisitioned it on your behalf, citing operational necessity. Even within the Antimemetics Division, Class-Z authorization is restricted to field operatives with demonstrated need and a clean mnestic tolerance record. Each dose is individually tracked from synthesis to administration. Post-use reporting is mandatory.*

**Psychometric Reading Scaling:** The damage bonus increases to **+1d8**. Years of behavioral analysis have built a predictive model in your head that borders on precognition — you're not reading body language anymore, you're running a neural network trained on thousands of hours of combat observation. Your callouts arrive before the target commits to their action. Still applies to the next two allies to hit the target.

**Cognitive Decontamination Scaling:** Improves to **3 per short rest**. Pneumatic delivery system upgraded — range extends to **30 feet** (improved launch pressure and dart stabilization). You can now decontaminate from across a room without repositioning.

**Cognitive Warning** scales to **2 per short rest**.

SCRAMBLE stays at 2/encounter (scaled at L8).

---

### Levels 10–12 (Full Detail)

#### Level 10

**Antimemetic Concealment**  
*Your turn — Action — Once per long rest — Concentration (up to 1 hour)*  
**Dosing: 1 action per target per round, touch range. Self + up to 3 willing allies (4 rounds max). Effect activates once all intended targets are dosed.**

Administer FORGOTTEN-7 — an experimental antimemetic compound developed by the Division's Applied Concealment Research group. No target gains the antimemetic effect until you finish dosing every intended subject; the compound synchronizes across all recipients simultaneously, so plan your target count before you start. Out of combat, the same procedure applies without initiative pressure — 4 rounds pass narratively (about 24 seconds of prep).

For up to 1 hour, all dosed creatures are **antimemetically shielded**. They are not invisible — they are *irrelevant*. Light still reflects off them. Sound still carries. But the cognitive processing required for an observer to register their presence is suppressed at the neurological level. Enemies who have not been alerted to your presence must make a **WIS save (DC = 8 + your proficiency bonus + your WIS modifier)** to notice any shielded creature. On failure, their brain simply does not process the shielded creature's existence — eyes slide past, sounds don't register, even direct physical contact provokes only momentary confusion before the perception is discarded.

**Enemies who succeed** on the save perceive the shielded creatures normally and can alert others (alerting others does not grant automatic perception — each creature must save independently or have the shielded creatures pointed out with sustained, deliberate effort).

**Breaks on hostile action:** If a shielded creature attacks, casts an offensive ability, or takes any directly hostile action, FORGOTTEN-7's antimemetic suppression shatters for that creature only — the act of violence is too cognitively salient to suppress. Other shielded allies remain concealed.

**Concentration:** You maintain the antimemetic field by monitoring dosage coherence on your CRV scanner. Standard concentration rules apply, including the Counter-Memetic Barrier's mental immunity (FORGOTTEN-7 uses the same hardware backbone — mental effects cannot break your concentration). Physical damage forces concentration saves normally.

Side effects: **1d4 hours of existential unease** after the compound metabolizes. Subjects report feeling "unreal," questioning whether they exist, and experiencing brief depersonalization episodes. The Antimemetics Division has a post-operation support group. Attendance is mandatory. The Division psychologist will ask you how you felt about not existing for an hour. Answer honestly.

*Authorization: FORGOTTEN-7 is experimental Division technology. Access is restricted to operatives on approved covert operations — your handler must authorize each dose, and each dose is individually tracked from synthesis through administration to metabolization. You are functioning as a Division covert operative, not a medic, when you deploy FORGOTTEN-7. Your Medical chain of command is not informed.*

*Design note: This is infiltration, not invisibility. The WIS save means high-WIS enemies (SCP entities, trained Foundation personnel, anomalous psychics) can still detect you. The hostile-action break prevents abuse as a combat cloak. The concentration requirement means the MS cannot deploy FORGOTTEN-7 and Counter-Memetic Barrier simultaneously — choose infiltration or defense, not both.*

#### Level 11

*The person who holds your hand while you're dying and the person who dissolves someone's sense of self are now the same person. Your team knows what you carry. They've seen what it does. Some of them are afraid of you. All of them are glad you're on their side. This is an intentional tension — you are no longer "the team medic." You are a Division weapon who also heals.*

**Advanced Berryman-Langford Weaponization**  
*Upgrade to Cognitive Strike*  
Your Cognitive Strike deployment is upgraded with Division field-tested improvements to payload range, target acquisition, and deployment cadence:

- **Range:** Increases to **60 feet** (improved emitter array with focused-beam delivery)
- **Targets:** You can deploy against **2 targets simultaneously** with a single action. Both targets must be within range. You choose one payload type per deployment (both targets face the same payload). Each target saves independently. **Exception:** Identity Fracture (below) is always single-target — the payload is too complex to split.
- **Uses:** Increases to **2 per short rest** (improved payload synthesis — your kit now generates fresh BL patterns between rests)
- **New Payload — Identity Fracture** (see separate entry below)

---

**Identity Fracture (Cognitohazard ████-Aleph)**  
*Your turn — Action — Once per long rest — separate resource from Cognitive Strike charges*  
*60 feet range — Single target only*

Choose one creature within 60 feet. **Single target only** — the ████-Aleph payload requires focused, single-target delivery. The multi-target upgrade from Advanced BL Weaponization applies to Cognitive Overload, Sensory Blackout, and Implanted Compulsion only.

On a failed WIS save, the target enters a state of total ego dissolution — they do not know who they are, where they are, or what they want. They **cannot attack, cannot defend, cannot take actions or reactions, and automatically fail DEX saves**. At the end of each of their turns, they make a **WIS save** against your Cognitive Strike DC to recover. On success, their identity reassembles and the effect ends. On failure, the dissolution continues. **Maximum duration: 1 minute (10 rounds)** — after that, the payload degrades and the target's identity reassembles regardless of saves.

**Cognitive backlash:** After use, you suffer **disadvantage on all WIS saves** and **cannot activate Counter-Memetic Barrier** until you complete a short rest.

**Witness cost:** Allies who see you deploy Identity Fracture must make a **DC 10 WIS save** or be **Frightened of you** for 1 round.

*Deploying Identity Fracture echoes back through your own neural architecture. Your CRV baseline spikes — you are measurably less "yourself." The Antimemetics Division documented this effect and considers it an acceptable operational cost. You may not agree. Your allies' fear is not irrational — they just watched you erase someone. The target didn't scream — they stopped being a person.*

*Authorization: Cognitohazard ████-Aleph is Thaumiel-class — restricted even within the Division. Deployment requires pre-authorization from Division command AND an Ethics Committee waiver for each specific deployment where it might be used. It cannot be carried without authorization. Post-use investigation is mandatory regardless of outcome. Use against human targets may be prohibited entirely unless they are classified as anomalous entities. The DM should ensure there are institutional consequences every time Identity Fracture is deployed — it is a weapon of last resort, and the campaign world treats it that way.*

*Design note: Identity Fracture is the MS's nuclear option — 1/LR, single target, with a personal cost that strips your defensive axis (WIS saves + Barrier) until you rest. This matches the power budget of Miraculous Save (CM, 1/LR, prevent one death) and Fortify (IM, 1/LR, one round resistance). The cognitive backlash means using Identity Fracture is a genuine trade: you trade your strongest defense for your strongest offense. Save it for the moment that matters.*

**SCRAMBLE Eyewear Scaling:** Neurally paired. Your SCRAMBLE glasses are now fully integrated with your mnestic-conditioned neural architecture — the pattern-recognition algorithms run through your conditioning, not just the hardware. You have **advantage on ALL WIS saves against cognitohazards** while the glasses are worn. No per-encounter limit. The glasses and your brain are one defense system.

**First Aid** scales to 5d6 + WIS.

**Counter-Memetic Barrier** improves to **twice per long rest**.

**Cognitive Warning** scales to **3 per short rest**.

#### Level 12 — Dual Capstone

*You are one of the most dangerous non-anomalous humans in the Foundation's employ. Your conditioning, your equipment, and your clearance place you in a category shared by fewer than a hundred field operatives worldwide. You still carry a trauma kit. You still heal. But the medic who started this journey and the operative who finishes it are not the same person — and you know it, because your CRV scanner tells you your own baseline has shifted.*

**Containment-Class Inoculation**  
*Non-combat — 10 minutes — Once per long rest*  
The culmination of everything your Division training has built toward. Using a combination of Class-Z mnestic (direct-input mode), your CRV scanner locked to the target's neural architecture, and prolonged controlled-exposure cognitive conditioning, you **permanently restructure a creature's neural pathways** to be immune to one specific anomaly's mental influence.

**Requirements:**
- **10 minutes** of uninterrupted procedure time
- **Knowledge of the anomaly's memetic signature** (you must have scanned the anomaly with your Advanced CRV Scanner or been briefed with its Division threat profile)
- **Willing and conscious target** who provides informed consent
- **Controlled environment** — minimum: a secure room with no interruptions. This cannot be performed in the field, mid-combat, or under time pressure. The target's neural architecture is being deliberately restructured; any interruption risks incomplete conditioning or, worse, partial integration of the anomaly's influence

**The procedure:** The target experiences 10 minutes of the anomaly's full memetic influence while the Class-Z mnestic teaches their brain, synapse by synapse, to recognize and reject it. The Foundation's neuroscience division cannot fully explain how Class-Z achieves this level of precision — the mechanism crosses the boundary between pharmacology and anomalous intervention, and the Division accepts this without requiring a complete theoretical framework. This is painful. The target must make a **DC 15 CON save** at the 5-minute mark — on failure, they take **2d6 psychic damage** from the controlled exposure but the procedure continues. At the conclusion, the target's neural architecture is permanently altered. They are **immune to that specific anomaly's mental effects**. Forever. This immunity cannot be removed, suppressed, or overridden by any means short of the anomaly fundamentally changing its memetic structure.

**Permanent. Irreversible.** The target's brain is different after this procedure. Their CRV baseline shifts. Their dreams change. They will never think about the world quite the same way again. But the anomaly that once could break their mind now slides off them like water.

One specific anomaly per application. To inoculate against a second anomaly requires a separate procedure (and a separate long rest).

*"We don't contain the anomaly. We contain its ability to affect us."*

*Authorization: Requires Ethics Committee pre-authorization (submitted in writing, minimum 48 hours before the procedure), full informed consent from the target (written, witnessed by two Foundation personnel), a medical team on standby during the procedure, and post-procedure monitoring for a minimum of 72 hours. The target must be psychologically evaluated before and after. This is a between-mission procedure. The paperwork alone takes longer than the conditioning.*

**Cognitive Sovereignty**  
*Reactive — Once per long rest*  
When an ally within 30 feet **would fail** a WIS saving throw against a mental or memetic effect, you can use your reaction to **shield their cognition**. You use your CRV scanner to generate a counter-signal that shields the ally's neural processing while deliberately lowering your own cognitive defenses to compensate — opening yourself to absorb the overflow. Your Antimemetics Division conditioning and mnestic-restructured neural architecture allow you to contain cognitive threats that would shatter an unprotected psyche.

**The ally automatically succeeds** on the save — they are completely unaffected. The effect never reaches them. You shielded their mind and absorbed what broke through.

**You must then make a WIS save yourself** against the same DC. Your Pattern Recognition (proficiency/expertise in WIS saves), mnestic conditioning (advantage against Charm effects), and any other applicable bonuses apply to this save — you are the most qualified person in the room to resist this. On a **success**, your conditioning holds. You contain the cognitohazard, process it, and discard it. On a **failure**, you suffer the full effect as though you had been the original target — because you opened yourself to it.

You can use Cognitive Sovereignty against effects that don't normally allow saves — if your ally was targeted by a no-save mental effect, you shield them and absorb the overflow, making a WIS save (DC = 15 or the source's spell/ability DC, whichever is higher). This is the only protection in your toolkit that works against no-save mental attacks, and it costs you the risk of taking it yourself.

**Cannot be used on yourself.** This is cognitive shielding, not a self-buff. You must be protecting someone else.

*"I see it. I see what it's doing to you. Look at me. LOOK AT ME. I'll take it."*

This is the Memetic Specialist's capstone MOMENT. The ally's eyes glaze, the cognitohazard starts to take hold — and you shield their mind, opening yours. You've trained for this. You've conditioned your brain for exactly this. Whether you survive it intact is another question. The team has other healing options. The team does not have another person conditioned to absorb cognitohazards.

*Role note: A medic's duty is to stay functional so they can treat others. Deliberately exposing yourself to a cognitohazard violates that principle. But you are not acting as a medic when you use Cognitive Sovereignty — you are acting as a Division operative. Containing cognitohazards is literally your primary mission. The conflict between "stay functional to heal" and "absorb the threat to protect" is the defining tension of the Memetic Specialist at level 12. Every time you use this, you are choosing Division operative over field medic. Make sure it's worth it.*

*Design note: Cognitive Sovereignty does not compete with Cognitive Warning — Warning gives advantage on a save the ally might still fail; Sovereignty triggers AFTER the ally has already failed. They are sequential tools: Warning is your first line, Sovereignty is your last. The once-per-long-rest limit ensures Sovereignty is a dramatic moment, not a routine rotation. The self-save risk prevents it from being a no-cost rescue — the MS pays with their own safety, which is thematically and mechanically correct.*

---

---
## Design Notes for DM

### Progression Overview

| Level | All Medics | Combat Medic | Internal Medic | Memetic Specialist |
|-------|-----------|-------------|----------------|-------------------|
| 1 | First Aid, Stabilize, Medical Assessment | — | — | — |
| 2 | Emergency Response, Medic's Eye | — | — | — |
| **3** | **CHOOSE SPECIALIZATION** | Triage, Combat Stabilization | Preemptive Treatment, Precision Medicine (Purge, charges) | Memetic Inoculation, Psychometric Reading, Cognitive Triage, Residual Imprint |
| 4 | | Under Fire, Proximity Training, Field Forensics, Tactical Medical Assessment | Directed Recovery (mode-select: Heal/Cure/Buff), Directed Triage, Classified Consultation, Clinical Scanner | Cognitive Decontamination (1/SR, +immunity window), Inoculation scaling |
| 5 | | Adrenaline Shot (+ mental re-save + failure rider), **Trauma Extraction**, FA 3d6, Triage 2d6 | Analysis Paralysis, Preemptive Treatment scaling (5 allies, MB-9), FA 3d6 | Pattern Recognition, SCRAMBLE, FA 3d6, Psych Reading +1d6 |
| 6 | | Patch Job (+ Field Remedy), Triage Point | Amnestics (+ certification), **Field Triage Protocol** | Counter-Memetic Barrier (+ concentration hardening), Advanced CRV |
| 7 | | Field Surgery, Battlefield Awareness, After-Action Medical Report | Strategic Preparation (AR-5, CF-2), Analysis Paralysis×2 | Memetic Hardening, Cognitive Warning (1/SR), Cog Decontam×2 |
| 8 | | Mass Triage, FA 4d6 | Class-B Amnestics, Med Authority, FA 4d6 | **Division Induction:** Cognitive Strike, SCRAMBLE×2, FA 4d6 |
| 9 | | Adrenaline Surge, Field Surgery+, Trauma Extraction→BA | Experimental Protocol, Directed Triage×3 | Antimemetic Protocol, Cog Warning×2, Cog Decontam×3, Psych Reading +1d8 |
| 10 | | Adv. Field Surgery, FA 5d6 | Protocol HIPPOCRATES, RC-7→6d6, AP-1, Exp. Protocol×2 | Antimemetic Concealment |
| 11 | | Miraculous Save, Mastery | Class-C Amnestics, FA 5d6, Fortify, Analysis×3 | Adv. BL Weapons, SCRAMBLE always-on, FA 5d6, Barrier×2, Cog Warning×3 |
| 12 | | One More Breath, FA 6d6 | Lazarus Protocol | Containment-Class Inoculation + Cognitive Sovereignty |

### Technology Summary

| Class | Primary Tech | Key Compounds | Key Equipment |
|-------|-------------|---------------|---------------|
| Base Medic | Trauma medicine | Hemostatic gel, analgesics | Field medical kit, biometric scanner |
| Combat Medic | Advanced trauma, surgery | Compound 47/47-B, biofoam, LAZARUS-Light | Tactical trauma rig, defibrillator, surgical kit |
| Internal Medic | Pharmacology, databases | IM-7, DRG-4, PS-12, BR-3, NCD-1, AM-A/B/C, RC-7 | Pharmaceutical case, medical terminal, amnestic kit (from L6) |
| Memetic Specialist | Mnestic science, SCRAMBLE, BL weapons | Class-W/X/Y/Z mnestics, FORGOTTEN-7, BL payloads | CRV scanner (L3), SCRAMBLE (L5), emitter (L6), BL kit (L8) |

### Grounding Philosophy

Nothing in this document is "magic." Every ability has a mechanism:
- **Healing** = trauma medicine, surgical intervention, pharmaceutical compounds
- **Buffs** = drugs with specific biochemical effects (and side effects)
- **Mental protection** = mnestic compounds that reinforce natural cognition
- **Mental offense** = weaponized cognitohazards (Berryman-Langford derivatives)
- **Information** = scanners, databases, behavioral analysis algorithms, biometric readings
- **Authority** = Foundation institutional hierarchy and clearance systems

### Combat Rhythm Comparison (Level 5)

**Combat Medic turn:**
- Action: First Aid (3d6+3 = 13.5 HP) OR Attack
- Bonus Action: Triage (2d6+3 = 10 HP, 3 charges) OR Adrenaline Shot (buff willing ally, 1/LR)
- Reaction: Combat Stabilization (DC scales with distance) OR Emergency Response
- **Total burst: 23.5 HP/turn | Sustained: 13.5/turn | Decision: heal two targets or heal+buff?**

**Internal Medic turn:**
- Action: First Aid — choose ONE mode: **Heal** (3d6+3 = 13.5 HP), **Cure** (Purge a condition, WIS mod charges/SR), or **Buff** (+2 AC, save advantage, or reposition)
- Bonus Action: Clinical Scanner (+1 attack to allies vs target) OR Directed Triage (ally spends hit die + WIS mod)
- Reaction: Analysis Paralysis (impose disadvantage on enemy attack, 1/SR) OR Emergency Response
- **Total: 13.5 HP OR condition removal OR buff + scanner bonus | Decision: which single problem is most urgent right now? Supplement with Directed Triage for flexibility.**

**Memetic Specialist turn:**
- Action: First Aid (3d6+3 = 13.5 HP) OR Cognitive Decontamination (1/SR)
- Bonus Action: Psychometric Reading on enemy (+1d6 damage to 2 allies on hit, plus DM behavioral prediction) OR Cognitive Triage on clean ally (advantage on next save, 2/SR)
- Reaction: Emergency Response or Residual Imprint (PB/LR). Cognitive Warning added at L7
- **Total: 13.5 HP + damage facilitated OR save protection | Decision: heal body or heal mind? Buff offense or protect an ally?**

### Corrected Balance Math (Level 5, WIS 16)

*These numbers use real per-round amortized values, not optimistic estimates.*

**Combat Medic:**
- Burst round (First Aid + Triage): 13.5 + 10 = 23.5 HP
- Sustained round (First Aid only): 13.5 HP
- Over 4-round combat with 3 Triage charges: (23.5 × 3 + 13.5) / 4 = **20.9 avg HP/round**
- Damage facilitated: 0
- Damage prevented: 0 (Combat Stabilization is reactive at 0 HP, not prevention)

**Internal Medic:**
- Healing: 13.5 HP/round (on heal turns only — buff and cure turns contribute 0 HP from action)
- Effective healing over 4 rounds (assume 3 heal, 1 buff/cure): ~10.1 avg HP/round
- Damage prevented from +2 AC (Directed Recovery, buff mode): ~10% miss chance increase × ~12 avg enemy damage = **1.2 on buff turns only**, amortized over 4 rounds = **~0.3/round**
- Damage prevented from Analysis Paralysis: ~25% miss conversion × ~12 damage = 3.0, but 1/SR over 4 rounds = **0.75/round amortized**
- Damage facilitated from scanner +1: +5% hit chance × ~12 damage × 2 allies attacking = **1.2/round**
- Directed Triage (bonus action, 2/SR): ally hit die (~4.5) + WIS mod (3) = 7.5, amortized = **~3.75/round**
- **Total effective value: ~16.1/round** (with Directed Triage compensating for lost healing on non-heal turns)

**Memetic Specialist:**
- Healing: 13.5 HP/round (sustained)
- Damage facilitated from Psychometric Reading (+1d6 damage on hit): 2 allies × 0.6 hit rate × 3.5 avg d6 = **4.2/round** (2 out of 4 rounds — two rounds used for Cognitive Triage instead)
- Save protection from Cognitive Triage: advantage on one ally's save, 2/SR, amortized = **~1.5/round** (hard to quantify, but preventing a failed save can be worth 10+ HP equivalent)
- **Total effective value: ~17+ /round** (with Cognitive Triage's prevention value hard to pin down but real)

### Balance Summary

| Spec | Effective Value/Round (L5) | Character |
|------|-----------------------|-----------|
| Combat Medic | ~20.9 avg (burst-heavy) | Highest throughput, concentrated in healing. Dominates emergencies. |
| Internal Medic | ~16.1 (mode-select + DT + scanner) | Flexible value, highest decision density. Best in varied-threat encounters. |
| Memetic Specialist | ~17.7 (heal + offense) | Offensive support, climbs dramatically when mental threats appear. |

**The gap is 20.9 vs ~16-17. Ratio: ~1.25:1.** The Combat Medic IS the healing specialist. A ~25% advantage in total effective value, concentrated entirely in burst healing, is reasonable. The Internal Medic compensates with flexibility (always has the right mode) and Directed Triage recovers lost healing on non-heal turns. The Memetic Specialist compensates with offensive damage facilitation and mental defense capabilities the other specs lack entirely.

**Important:** These numbers measure COMBAT value only. In non-combat situations (social, investigation, infiltration, research), the Internal Medic and Memetic Specialist contribute significantly while the Combat Medic's tools are narrower (Tactical Medical Assessment for pre-mission prep, Field Forensics for scene analysis, After-Action Medical Report for post-combat intel). The CM's out-of-combat contribution is real but more modest than IM or MS. Total campaign value is more balanced than combat-only numbers suggest, though IM still leads overall.

### Balance Triangle (Revised)

| Category | Combat Medic | Internal Medic | Memetic Specialist |
|----------|-------------|----------------|-------------------|
| **Raw healing/turn** | Highest (burst) | Medium (mode-select: heal turns only) | Medium |
| **Effective total value** | High (burst) / Medium (sustain) | Medium-High (mode-select: right tool, one at a time) | Medium-High (heal+offense) |
| **Offensive support** | Low | Medium (scanner +1, intel) | Highest (+1d6→+1d8 damage) |
| **Prevention** | None | Highest (AC buff, Analysis Paralysis) | Moderate (if mental) |
| **Pre-combat** | Moderate (Triage Point, Tactical Medical Assessment) | Highest (pharmaceutical prep) | Moderate (inoculations, Hardening) |
| **Anti-anomalous** | None | Some (amnestics, ECD-3) | Dominant |
| **Out-of-combat** | Moderate (Field Forensics, Tactical Assessment, After-Action Report) | Highest (databases, authority, amnestics) | Moderate (threat assessment, infiltration) |
| **Mobility** | Highest (Under Fire) | Low | Low |
| **Resource dependency** | High (patches, stim) | Medium (Purge charges, DT limited, mode-select forces trade-offs) | Low (CRV unlimited, Decontam 1/SR) |
| **Decision density** | Medium | Highest (mode-select every turn) | Medium-High |
| **Capstone moment** | Cinematic (defibrillator slam) | Heavy (raising the dead) | Heroic (shielding ally from cognitohazard) |

### Chain of Command Summary

| Spec | Reports To | Notes |
|------|-----------|-------|
| Combat Medic | Medical Division | Clean military medical chain. No conflicts. |
| Internal Medic | Medical Division (primary) | Amnestic operations under Medical authority. Security requests support through Medical. Dual-reporting only emerges at L10+ with Protocol HIPPOCRATES (temporary O5 oversight). |
| Memetic Specialist | Medical Division (L3-7) → Medical + Antimemetics Division (L8+) | Dual-reporting from L8. Division may give orders the team leader doesn't know about. DM should lean into this tension. |

### Ethics Committee Implications

Several abilities trigger Ethics Committee review. The DM should use these as narrative tools, not just mechanical constraints.

| Ability | Spec | Level | Ethics Concern | Likely Ruling |
|---------|------|-------|---------------|---------------|
| Compound 47 (Adrenaline Shot) | Combat | 5 | Guaranteed adrenaline crash (disadvantage) to target | Authorized with verbal consent requirement |
| Amnestic Administration | Internal | 6+ | Memory erasure without informed consent | Authorized with strict logging, post-admin monitoring, misuse = investigation |
| Class-B Amnestics (combat use) | Internal | 8 | Forcible memory erasure on unwilling targets | Authorized for hostile entities only. Use on Foundation personnel requires written consent or O5 authorization |
| Protocol HIPPOCRATES | Internal | 10 | Emergency authority override | Pre-authorized by O5 Council. Mandatory post-incident review. Abuse = career end |
| Lazarus Protocol | Internal | 12 | Creates anomalous entity | Requires pre-authorization. Revived individual subject to Foundation monitoring. Anomalous residue may trigger containment |
| Cognitive Strike | Memetic | 8 | Weaponized cognitohazard on sentient beings | Cognitive Overload/Sensory Blackout = authorized (equivalent to flashbangs). Implanted Compulsion = authorized with documentation |
| Identity Fracture | Memetic | 11 | Psychological weapon — dissolves sense of self | **Restricted.** Pre-authorization from Division command AND Ethics Committee waiver per deployment. Post-use investigation mandatory. May be prohibited against human targets. Institutional consequences every use |
| Containment-Class Inoculation | Memetic | 12 | Permanent irreversible neural restructuring | Requires written informed consent, medical team on standby, Ethics Committee pre-authorization, 72-hour monitoring |
| Cognitive Sovereignty | Memetic | 12 | Deliberate self-exposure to cognitohazard | Authorized under Division conditioning program consent |

### Campaign Requirement: Memetic Specialist

**IMPORTANT — DM commitment required before a player selects Memetic Specialist.**

The Memetic Specialist's effectiveness outside their specialty depends entirely on encounter design. In standard combat with no mental/memetic component, they are a slightly weaker healer with a damage buff. Their signature tools (Cognitive Decontamination, SCRAMBLE, Counter-Memetic Barrier, Cognitive Strike) are partially or wholly irrelevant.

**Before a player picks Memetic Specialist, the DM should commit to: at least 30-40% of encounters will involve some mental, memetic, or cognitohazardous component.** This includes charmed enemies, mind-controlled allies, cognitohazardous environments, memetic SCP encounters, psychic damage, fear effects, and compulsion effects.

If the DM cannot commit to this encounter variety, the Memetic Specialist player will have a frustrating experience — spending 60%+ of combat sessions as a less effective version of the other two specs.

In an SCP campaign, 30-40% cognitohazard encounter rate should be natural. If it's not, the DM should reconsider whether the Memetic Specialist fits this particular campaign's tone.

### Tuning Levers

| Problem | Lever |
|---------|-------|
| Combat Medic heals too much | Reduce Triage charges (WIS mod - 1) or cap at 2d6 |
| Combat Medic feels weak | Remove Triage cap, allow 4d6+ |
| Combat Medic mental override too strong | Remove mental re-save from Adrenaline Shot; accept Combat Medic is helpless vs mental |
| Combat Medic mental override too weak (v0.10 failure rider insufficient) | Add advantage to the initial Adrenaline Shot re-save instead of the failure rider |
| Adrenaline Shot failure rider too generous | Remove failure rider; keep the binary nature as intended design |
| CM Tactical Medical Assessment +1 death save too impactful | Reduce to advantage on first death save only, not +1 to all |
| CM After-Action Medical Report initiative advantage too strong | Remove initiative advantage; keep only the narrative intel |
| Internal Medic mode-select boring | Allow double-stack (Heal+Cure or Heal+Buff) but not triple |
| Internal Medic too weak with mode-select | Allow Cure mode to include half healing (1d6+WIS instead of full dice) |
| Internal Medic Purge charges too generous | Reduce to proficiency bonus per SR instead of WIS mod |
| Internal Medic Purge charges too stingy | Increase to WIS mod + proficiency per SR |
| Internal Medic anomalous Purge too hard | Lower the Medicine DC formula |
| Internal Medic anomalous Purge too easy | Raise the Medicine DC formula or restrict to 1 anomalous Purge attempt per SR |
| Memetic Specialist useless in normal fights | Increase Psychometric Reading scaling further |
| Memetic Specialist too dominant vs mental | Reduce Decontamination to 1/LR; increase emitter costs |
| Counter-Memetic Barrier still too fragile (v0.10 advantage insufficient) | Remove concentration entirely; Barrier is a device, not a spell. Lasts full duration unless physically destroyed (HP threshold). |
| Counter-Memetic Barrier too resilient with advantage | Revert to standard concentration (no advantage); accept 2-4 round average lifespan |
| Counter-Memetic Barrier too strong (immune to mental conc loss + advantage on physical) | Revert physical concentration to standard; keep mental immunity only |
| Cog Decontam immunity window too strong | Reduce to "advantage on next save vs same effect" instead of full immunity |
| Cog Decontam immunity window too weak (enemies with multiple Override types) | Expand to "immune to all effects from the same source" not just "same effect" |
| Cog Decontam charge scaling too generous | Reduce to 1/2/2 instead of 1/2/3 |
| Everyone too hard to kill | Reduce First Aid dice globally by 1 step |
| Everyone dies too easily | Scale First Aid faster or add shared Second Wind |
| Directed Triage too strong | Remove WIS mod addition (ally just rolls hit die) |
| Directed Triage draining party resources | Reduce to 1/SR or change to Internal Medic's own resource |
| Analysis Paralysis too strong | Increase to 1/LR instead of 1/SR |
| SCRAMBLE scaling too fast/slow | Adjust tier breakpoints |
| Cognitive Triage too strong | Reduce to 1/SR, or reduce to advantage on WIS saves only (not all saves) |
| Cognitive Warning scaling too generous | Reduce to 1/1/2 instead of 1/2/3 |
| Field Remedy too broad | Restrict to Frightened only (remove Charm re-save option) |
| Field Remedy blurs spec boundaries | Remove entirely; accept Combat Medic is helpless vs mental |

### Shared Equipment Rule

If a medic goes down, can allies use their supplies? Base medic training allows any Foundation operative to use standard trauma patches and stabilization kits from an unconscious medic's gear (no proficiency bonus on the heal). Specialization-specific equipment (mnestic autoinjectors, pharmaceutical compounds, SCRAMBLE emitters, amnestic doses) requires training to use safely — without it, there's a 50% chance of administering the wrong dose or activating the device incorrectly. DM adjudicates.

### Institutional Consequences Quick Reference

| Action | Consequence |
|--------|------------|
| Using amnestics without documentation | Automatic Security investigation |
| Using amnestics on Foundation personnel without consent/authorization | Certification revocation, possible disciplinary action |
| Invoking Protocol HIPPOCRATES | Mandatory post-incident review (not punishment — just oversight) |
| Abusing Protocol HIPPOCRATES | O5 investigation, career-ending |
| Using Lazarus Protocol | Full incident report, revived individual monitored, possible containment classification |
| Using Identity Fracture | Mandatory post-use investigation regardless of context |
| Using Identity Fracture without pre-authorization | Division disciplinary action, possible ethics violation charge |
| Losing or misusing Division equipment | Division investigation, possible clearance revocation |
| FORGOTTEN-7 use | Post-operation Division debrief, dose accounting |

### Back-Pocket Subclasses

**Anomalous Medic ("Thaumaturge"):** Uses anomalous artifacts and Thaumiel-class compounds to heal. Every treatment requires rolling on a side-effect table. Highest raw healing potential, completely unpredictable. For players who enjoy risk.

**Containment Medic ("Scrubber"):** Decontamination and environmental control. Chemical neutralization agents, radiation barriers, anomalous contamination scrubbing. Creates safe zones, treats reality-warped injuries. Defensive and area-control focused.
