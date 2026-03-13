# GDPR Compliance Analysis: Cognition Legal Practice

**Unit 4 — Cyberlaws Consolidation Activity**

---

## Introduction

Cognition is a multi-disciplinary legal practice processing personal data across multiple stages: insurer referral, client onboarding, algorithmic claim assessment, medical referral to a third-party (Doctors Lab), and claims handling by a South Africa-based team with access to UK-stored data. This analysis evaluates the lawful bases for each processing activity and the accountability obligations Cognition must discharge as data controller under the UK GDPR.¹

---

## (1) Lawful Basis for Data Processing

### (i) Insurer's Transfer of Claimant Details to Cognition

**Consent (Article 6(1)(a))**

The insurance contract states that claimants "consent to their details being passed to Cognition." However, this consent is legally problematic. GDPR requires consent to be "freely given, specific, informed and unambiguous."² Consent embedded in standard insurance terms as a condition of obtaining cover risks failing the "freely given" requirement where refusal carries a significant disadvantage. Recital 43 expressly warns that consent is presumed not freely given where there is a "clear imbalance" between the data subject and controller.³ Furthermore, the consent is insufficiently specific: it covers referral to Cognition but does not extend to algorithmic processing, medical referral, or international transfer to South Africa. Consent must be granular and purpose-specific.⁴

**Legitimate Interests (Article 6(1)(f))**

A more robust basis is the insurer's legitimate interest in efficient claims management. The insurer has a genuine commercial interest in directing injured policyholders to a specialist legal representative promptly. A properly conducted balancing test would likely favour the insurer, as claimants who have suffered road traffic accidents hold reasonable expectations that their insurer will facilitate recovery services.⁵ However, the insurer must conduct and document this balancing test and provide transparent information in its privacy notice.⁶

**Assessment:** Consent as currently constituted is likely invalid. **Legitimate interests under Article 6(1)(f)** is the stronger lawful basis, provided the insurer documents the balancing test and gives adequate transparency.

---

### (ii) Cognition's Processing of Claimant Data

**Contract Performance (Article 6(1)(b))**

Once a claimant enters a legal retainer, processing necessary to perform that contract is lawful under Article 6(1)(b).⁷ This covers: collection of personal details, management of the claim, and liaison with the insurer. This is the primary lawful basis for core claims handling and does not require separately obtained consent.

**Legitimate Interests — Algorithmic Assessment**

The proprietary algorithm, which assesses claim viability and likely compensation, operates beyond strict contract necessity and requires an independent basis. Legitimate interests may apply, but only if Cognition passes the three-part test: (a) a genuine legitimate interest exists (commercial efficiency); (b) the processing is necessary for that interest; and (c) the interest is not overridden by the claimant's rights.⁸

**Critically**, if the algorithm produces a decision that significantly affects a claimant's ability to pursue their claim, this triggers Article 22 GDPR, which prohibits decisions based solely on automated processing that produce legal or similarly significant effects without human review, the right to object, or explicit consent.⁹ Absent these safeguards, the algorithm processing is unlawful.

**Special Category Data — Medical Information**

The claimant's injury details and Doctors Lab medical report constitute health data under Article 9, requiring an explicit legal basis beyond Article 6. Explicit consent under Article 9(2)(a) or processing necessary for legal claims under Article 9(2)(f)¹⁰ are the most applicable derogations. Cognition must also ensure a written Data Processing Agreement (DPA) with Doctors Lab under Article 28.¹¹

**International Transfers — South Africa**

Transferring data to the South Africa-based team is a restricted transfer under Chapter V of the UK GDPR. South Africa does not benefit from a UK adequacy decision.¹² Cognition must implement Standard Contractual Clauses (SCCs) and conduct a Transfer Impact Assessment (TIA) to evaluate whether South African law provides essentially equivalent protection to UK GDPR.¹³ Following *Schrems II*, the mere use of SCCs is insufficient without supplementary technical and organisational measures (e.g., encryption, access restrictions) if the legal framework of the recipient country does not guarantee adequate protection.¹⁴ This is a critical compliance gap.

---

## (2) Accountability Principle Compliance — Article 5(2) GDPR

Article 5(2) imposes a proactive obligation on Cognition to demonstrate compliance with all Article 5(1) principles.¹⁵ The following actions are required:

**Records of Processing Activities (ROPA) — Article 30**

Cognition must maintain a documented ROPA covering each processing activity: purpose, legal basis, data categories, recipients, retention periods, and any transfers. The multi-purpose processing here — referral, onboarding, algorithm, medical, international transfer — requires separate, detailed entries. *Risk:* absence of a ROPA is a direct breach of Article 30 and undermines all accountability defences.

**Data Protection Impact Assessment (DPIA) — Article 35**

A DPIA is mandatory for the proprietary algorithm: it involves automated processing with "a systematic and extensive evaluation" producing decisions that significantly affect individuals.¹⁶ The DPIA must assess necessity, proportionality, and risk, and identify mitigations. A DPIA is also required for the South Africa transfer (Transfer Impact Assessment). *Risk:* without a DPIA, Cognition cannot lawfully operate the algorithm or the international data transfer; the ICO may impose an enforcement notice and fines up to £17.5 million or 4% of global turnover.¹⁷

**Data Processing Agreements — Article 28**

Written DPAs must be executed with Doctors Lab (medical reports) and the South Africa claims handler. Each DPA must specify processing scope, obligations, data subject rights, security, sub-processor authorisation, and audit rights.¹⁸ *Risk:* without DPAs, Cognition cannot contractually allocate processor liability and loses significant Article 82 protections.¹⁹

**Privacy by Design and Data Minimisation — Article 25 & 5(1)(c)**

The scenario discloses that South Africa handlers have access to "all" claimant personal data. This violates the data minimisation principle.²⁰ Cognition must implement role-based access controls restricting South Africa handlers to only the data fields necessary for their specific functions. Privacy by Design must also be embedded in the web-based collection system. *Risk:* disproportionate access creates unnecessary exposure in the event of a breach and constitutes a standalone compliance failure.

**Privacy Notices — Articles 13–14**

Claimants must be provided with clear privacy notices at or before the point of data collection, disclosing: controller identity; processing purposes and legal bases; recipients (Doctors Lab, South Africa handlers); international transfer details; retention periods; and data subject rights.²¹ The scenario gives no indication such notices exist. *Risk:* absence of privacy notices constitutes a breach of the transparency principle (Article 5(1)(a)) and the accountability principle simultaneously.

**Data Subject Rights — Articles 15–22**

Cognition must establish mechanisms to respond to Subject Access Requests (Article 15), rectification (Article 16), erasure (Article 17), objection (Article 21), and Article 22 safeguards for automated decisions (human review, right to contest, right to explanation). *Risk:* failure to facilitate these rights exposes Cognition to individual complaints and ICO enforcement.

**Data Retention Policy**

A documented retention schedule is required. Data must not be kept longer than necessary.²² Once a claim is resolved, personal data should be deleted or anonymised except where retention is required by law (e.g., limitation periods under the Limitation Act 1980). *Risk:* indefinite retention violates Article 5(1)(e).

**Breach Response — Articles 33–34**

Cognition must implement an incident response plan capable of detecting breaches, assessing risk, and notifying the ICO within 72 hours where there is risk to individuals.²³ High-risk breaches also require direct notification to affected claimants. *Risk:* the scenario is silent on breach procedures — a critical accountability gap.

---

## Risk Assessment Summary

| Issue | Severity | Key Risk |
|---|---|---|
| No DPIA for algorithm / automated decisions | **Critical** | Unlawful processing; Article 22 violation; ICO fine |
| No TIA / SCCs for South Africa transfer | **Critical** | Unlawful restricted transfer; *Schrems II* non-compliance |
| Excessive data access for South Africa handlers | **High** | Data minimisation breach; disproportionate exposure |
| No privacy notices | **High** | Breach of transparency and accountability principles |
| No DPAs with Doctors Lab / South Africa | **High** | Article 28 breach; unallocated processor liability |
| Invalid consent basis for insurer referral | **Medium** | Unlawful initial transfer; undermines downstream processing |
| No data retention schedule | **Medium** | Article 5(1)(e) violation; indefinite storage of sensitive data |
| No breach response procedures | **High** | Failure to comply with 72-hour notification obligation |

---

## Conclusion and Priority Remedial Actions

Cognition's current practices exhibit multiple serious accountability failures. To comply with Article 5(2), Cognition must, as a matter of priority:

1. Commission DPIAs for the algorithm and international transfer immediately.
2. Execute SCCs and complete a TIA for the South Africa processing arrangement, implementing encryption and access restrictions as supplementary measures.
3. Restrict South Africa handlers' access to claim-relevant data only.
4. Issue comprehensive privacy notices to all claimants at the point of data collection.
5. Execute Article 28-compliant DPAs with Doctors Lab and the South Africa team.
6. Implement Article 22 safeguards (human review, objection rights) for algorithm-based assessments.
7. Document a ROPA, data retention schedule, and breach response procedures.

Without these measures, Cognition cannot discharge the accountability obligation and faces significant regulatory action by the Information Commissioner's Office.

---

## Footnotes

¹ UK GDPR (retained from Regulation (EU) 2016/679 by the European Union (Withdrawal) Act 2018), as amended by the Data Protection Act 2018.

² GDPR Article 4(11); Recital 32.

³ GDPR Recital 43; ICO, *Guide to the UK GDPR: Consent* (2023).

⁴ Article 29 Working Party (now EDPB), *Guidelines on Consent under Regulation 2016/679*, WP259 rev.01, pp. 10–12.

⁵ GDPR Article 6(1)(f); Recital 47; ICO, *Guide to the UK GDPR: Legitimate Interests* (2023).

⁶ GDPR Article 13(1)(d); *Fashion ID GmbH & Co KG v Verbraucherzentrale NRW eV* (C-40/17) [2019] ECR I-, para 95.

⁷ GDPR Article 6(1)(b); EDPB, *Guidelines 2/2019 on Article 6(1)(b)*, paras 25–30.

⁸ ICO, *Legitimate Interests* guidance, three-part test at pp. 7–14.

⁹ GDPR Article 22(1) and (3); EDPB, *Guidelines on Automated Individual Decision-Making and Profiling*, WP251 rev.01.

¹⁰ GDPR Article 9(2)(a) and 9(2)(f).

¹¹ GDPR Article 28(3).

¹² UK GDPR, s. 17A Data Protection Act 2018; ICO, *Adequacy* guidance — no UK adequacy decision for South Africa as of 2024.

¹³ UK GDPR Article 46; ICO International Data Transfer Agreement (IDTA) / Addendum to EU SCCs.

¹⁴ *Data Protection Commissioner v Facebook Ireland Limited and Maximillian Schrems* (C-311/18) [2020] ECR I- (*Schrems II*), paras 103–105, 132–134; EDPB Recommendations 01/2020 on supplementary measures.

¹⁵ GDPR Article 5(2); Recital 85.

¹⁶ GDPR Article 35(3)(a); ICO, *Guidance on DPIAs* (2023).

¹⁷ Data Protection Act 2018, s. 157; GDPR Article 83(4).

¹⁸ GDPR Article 28(3)(a)–(h).

¹⁹ GDPR Article 82(2).

²⁰ GDPR Article 5(1)(c); Article 25(1) (Data Protection by Design and Default).

²¹ GDPR Articles 13–14; ICO, *Privacy Notices* guidance (2023).

²² GDPR Article 5(1)(e) (storage limitation principle).

²³ GDPR Articles 33–34; ICO, *Guide to the UK GDPR: Personal Data Breaches* (2023).
