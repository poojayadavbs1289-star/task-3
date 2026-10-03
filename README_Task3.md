# 🔍 Causality Assessment of Drug Reactions — Task 3

> **Internship Task | Pharmacovigilance & Drug Safety**  
> Evaluate the relationship between a drug and an observed adverse reaction using standard causality assessment methods. Analyze case studies and classify reactions as Certain, Probable, or Possible.

---

## 📋 Table of Contents

- [Objective](#objective)
- [What is Causality Assessment?](#what-is-causality-assessment)
- [Assessment Methods](#assessment-methods)
- [Case Study](#case-study)
- [Assessment Criteria](#assessment-criteria)
- [Naranjo Algorithm — Detailed Scoring](#naranjo-algorithm--detailed-scoring)
- [WHO-UMC Causality Categories](#who-umc-causality-categories)
- [Final Causality Classification](#final-causality-classification)
- [Comparison of Methods](#comparison-of-methods)
- [Key Learnings](#key-learnings)

---

## 🎯 Objective

- Evaluate the **relationship between a drug and an adverse reaction** using standard methods
- Apply **causality assessment tools** (Naranjo Scale, WHO-UMC criteria)
- Classify the reaction as **Certain, Probable, Possible, or Unlikely**
- Understand the **4 key assessment criteria** used in pharmacovigilance

---

## 🔬 What is Causality Assessment?

**Causality Assessment** is the systematic process of evaluating the likelihood that a drug caused an observed adverse reaction. It answers the core question:

> *"Is this adverse reaction really caused by this drug?"*

It is a critical step in pharmacovigilance because:
- Not every reaction that occurs **after** taking a drug is **caused by** the drug
- Multiple drugs or underlying diseases may be responsible
- Accurate causality classification drives **regulatory and clinical decisions**

---

## 🛠️ Assessment Methods

| Method | Description | Used By |
|--------|-------------|---------|
| **Naranjo Algorithm** | Scored questionnaire (0–13), produces probability category | Clinicians, researchers |
| **WHO-UMC Criteria** | Qualitative criteria — Certain, Probable, Possible, Unlikely | WHO, national agencies |
| **French Imputability** | Combines intrinsic (clinical) + extrinsic (bibliographic) scores | France's ANSM |
| **Liverpool ADR** | Simplified tool for clinical use | Healthcare professionals |

> **This task uses:** Naranjo Algorithm + WHO-UMC Criteria

---

## 🏥 Case Study

*(From the task scenario visible in the dashboard)*

| Field | Details |
|-------|---------|
| **Patient** | 45-year-old Female |
| **Suspected Drug** | Amoxicillin |
| **Adverse Reaction** | Skin Rash |
| **Onset** | 3 days after starting the drug |
| **Outcome** | Recovered after stopping the drug |
| **Concomitant Drug** | Paracetamol (as needed) |

---

## 📊 Assessment Criteria

The task image shows **4 key assessment criteria** used to evaluate causality:

---

### Criterion 1: ⏱️ Temporal Relationship
> *"Did the reaction occur after the drug was administered?"*

| Finding | Details |
|---------|---------|
| **Drug started** | Day 0 |
| **Reaction onset** | Day 3 (3 days after starting Amoxicillin) |
| **Assessment** | ✅ YES — Clear temporal relationship exists |
| **Significance** | Strong indicator of drug causality |

**Timeline:**
```
Day 0          Day 3           Day X
  |              |               |
  ▼              ▼               ▼
Amoxicillin   Skin Rash       Recovery
 Started       Appears       (after drug
                              stopped)
```

---

### Criterion 2: 🔄 Dechallenge
> *"Did the reaction improve after stopping the drug?"*

| Finding | Details |
|---------|---------|
| **Action taken** | Amoxicillin discontinued |
| **Outcome** | Patient recovered after stopping the drug |
| **Assessment** | ✅ POSITIVE Dechallenge |
| **Significance** | Strong confirmation of drug causality |

> A **positive dechallenge** (improvement after stopping) significantly increases the probability that the drug caused the reaction.

---

### Criterion 3: 🔀 Alternative Causes
> *"Could the reaction be explained by another cause?"*

| Alternative Cause | Evaluated | Conclusion |
|------------------|-----------|------------|
| Paracetamol | Yes | Unlikely — well-tolerated drug, not known to cause rash |
| Underlying disease | Not documented | No evidence of skin condition |
| Viral infection | Not documented | Possible but no supporting evidence |
| Food/environmental allergy | Not documented | No evidence |
| **Assessment** | | ✅ No alternative cause identified |

---

### Criterion 4: 🔁 Rechallenge (If Applicable)
> *"Did the reaction reappear on re-administration?"*

| Finding | Details |
|---------|---------|
| **Rechallenge performed?** | ❌ No |
| **Reason** | Not recommended — allergic reactions can be severe/life-threatening on re-exposure |
| **Assessment** | Unknown (not performed) |
| **Note** | Absence of rechallenge does not reduce causality probability in allergic ADRs |

---

## 📋 Naranjo Algorithm — Detailed Scoring

| # | Question | +Yes | -No | ?Unknown | Score Given | Reason |
|---|----------|------|-----|---------|-------------|--------|
| 1 | Previous conclusive reports of this reaction? | +1 | 0 | 0 | **+1** | Amoxicillin rash is well-documented |
| 2 | Did reaction appear after drug was given? | +2 | -1 | 0 | **+2** | Rash appeared 3 days after drug start |
| 3 | Did reaction improve after stopping drug? | +1 | 0 | 0 | **+1** | Patient recovered after dechallenge |
| 4 | Did reaction reappear on rechallenge? | +2 | -1 | 0 | **0** | Rechallenge not performed |
| 5 | Are there alternative causes? | -1 | +2 | 0 | **+1** | No alternative cause found |
| 6 | Did reaction reappear with placebo? | -1 | +1 | 0 | **0** | Unknown |
| 7 | Was drug detected in toxic concentrations? | +1 | 0 | 0 | **0** | Not measured |
| 8 | Was reaction more severe with higher dose? | +1 | 0 | 0 | **0** | Not assessed |
| 9 | Similar reaction to drug/related drugs before? | +1 | 0 | 0 | **0** | No prior history documented |
| 10 | Confirmed by objective evidence? | +1 | 0 | 0 | **+1** | Skin rash is clinically observable |
| | | | | **Total** | **+6** | |

### Naranjo Score Interpretation

| Score Range | Category | Our Case |
|-------------|----------|----------|
| ≥ 9 | **Certain** | — |
| 5 – 8 | **Probable** | ✅ Score: **+6** |
| 1 – 4 | **Possible** | — |
| ≤ 0 | **Doubtful** | — |

---

## 🌍 WHO-UMC Causality Categories

| Category | Criteria | Applies? |
|----------|----------|---------|
| **Certain** | Plausible time sequence; dechallenge confirmed; rechallenge positive; no alternative cause | ❌ (No rechallenge) |
| **Probable** ✅ | Reasonable time sequence; dechallenge confirmed; alternative cause unlikely | ✅ **YES — Our Case** |
| **Possible** | Reasonable time sequence; dechallenge unknown; alternative cause possible | ❌ |
| **Unlikely** | Temporal relationship improbable; other causes plausible | ❌ |
| **Conditional** | More data needed for proper assessment | ❌ |
| **Unassessable** | Insufficient or contradictory information | ❌ |

---

## ✅ Final Causality Classification

### By Naranjo Algorithm:
> **PROBABLE ADR** — Score: +6

### By WHO-UMC Criteria:
> **PROBABLE** — Reasonable time sequence + positive dechallenge + no alternative cause

---

### Summary Table

| Assessment Dimension | Finding |
|---------------------|---------|
| **Temporal Relationship** | ✅ Clear (rash at Day 3 after drug) |
| **Dechallenge** | ✅ Positive (recovered after stopping) |
| **Alternative Causes** | ✅ None identified |
| **Rechallenge** | ❓ Not performed (not recommended) |
| **Naranjo Score** | **+6 → Probable** |
| **WHO-UMC Classification** | **Probable** |
| **Final Verdict** | ✅ **PROBABLE ADR — Amoxicillin-induced Skin Rash** |

---

## ⚖️ Comparison of Methods

| Feature | Naranjo Algorithm | WHO-UMC Criteria |
|---------|------------------|-----------------|
| **Type** | Quantitative (scored) | Qualitative (descriptive) |
| **Output** | Numeric score → category | Direct category assignment |
| **Ease of use** | Structured, consistent | Requires clinical judgment |
| **Best for** | Research, standardization | Clinical practice, reporting |
| **Our Result** | Probable (+6) | Probable |
| **Agreement** | ✅ Both methods agree |  |

---

## 📚 Key Learnings

- ✅ Causality assessment answers: *"Did the drug cause the reaction?"*
- ✅ The **4 key criteria** are: Temporal Relationship, Dechallenge, Alternative Causes, Rechallenge
- ✅ **Naranjo Algorithm** gives a numeric score; **WHO-UMC** gives a qualitative category
- ✅ A **positive dechallenge** (recovery after stopping drug) strongly supports causality
- ✅ **Rechallenge is not always safe** — especially for allergic/hypersensitivity reactions
- ✅ "Probable" does NOT mean uncertain — it means strong evidence without rechallenge confirmation
- ✅ Both methods agreed: this is a **Probable ADR** caused by **Amoxicillin**
- ✅ Causality classification directly influences **pharmacovigilance signal detection**

---

## 👩‍💼 About This Task

| Field | Details |
|-------|---------|
| **Task ID** | task3 |
| **Task Name** | Causality Assessment of Drug Reactions |
| **Platform** | VirtualWorks Internship |
| **Domain** | Pharmacovigilance / Drug Safety |
| **Status** | ✅ Completed |

---

*This report was prepared as part of an internship task focused on pharmacovigilance causality assessment using standard tools — Naranjo Algorithm and WHO-UMC Criteria.*
