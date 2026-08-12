# Prompt Iteration Log

## BUS4005 Assessment 1 — HR Recruitment

This log is designed to document genuine iterative testing of the 10 prompts.

## Iteration method

For each prompt:

1. Run v1.0 using a controlled test case.
2. Save/capture the output.
3. Identify one or more concrete weaknesses.
4. Revise the prompt.
5. Run v1.1 using the same or equivalent test case.
6. Compare the outputs.
7. Revise again if justified.
8. Run v1.2.
9. Record the final version and the reason for selecting it.

---

## Prompt 01 — Job Description Analysis

| Version | Change made | Observed effect | Lesson learned |
|---|---|---|---|
| v1.0 | Initial requirement extraction and categories | **The prompt successfully identified the main job requirements, but it did not clearly distinguish mandatory requirements from desirable requirements.** | **The prompt needed an explicit instruction to classify the importance of each requirement.** |
| v1.1 | Added Mandatory/Desirable classification and preservation of original meaning | **The output separated mandatory and desirable requirements more clearly, but the categories did not consistently distinguish soft skills from technical skills.** | **More specific categories were needed to improve the usefulness of the output.** |
| v1.2 | Added soft-skill classification, evidence column and no-inference constraint | **The output became more structured and traceable, with requirements linked to evidence from the job description and fewer unsupported assumptions.** | **Explicit categories, evidence requirements and constraints improved output reliability.** |

## Prompt 02 — CV Information Extraction

| Version | Change made | Observed effect | Lesson learned |
|---|---|---|---|
| v1.0 | Basic extraction of candidate information | **The prompt extracted the main candidate information, but the information was not consistently structured and missing information was not clearly identified.** | **The prompt needed defined categories and a rule for handling unavailable information.** |
| v1.1 | Added categories and missing-information rule | **The output was more organised and clearly identified information that was not provided in the CV.** | **Structured categories and an explicit missing-information rule improved consistency.** |
| v1.2 | Added evidence column and no-inference constraint | **The output linked candidate information to evidence from the CV and reduced the risk of unsupported assumptions.** | **Requiring evidence and prohibiting inference made the extraction more reliable for HR review.** |

## Prompt 03 — CV-to-Job Matching

| Version | Change made | Observed effect | Lesson learned |
|---|---|---|---|
| v1.0 | Basic CV/job comparison | **The prompt identified several areas where the candidate matched the role, but the level of match was not consistently defined or supported with evidence.** | **A standard classification system and evidence requirement were needed.** |
| v1.1 | Added Present/Partially Present/Not Present classification and evidence | **The output provided a clearer comparison of the candidate against each requirement and included supporting CV evidence.** | **Defined categories improved consistency when comparing requirements.** |
| v1.2 | Added Not Evidenced category, table structure and no recommendation | **The output better distinguished between a requirement being absent from the CV and there simply being insufficient evidence. It also presented the comparison more consistently without making a hiring recommendation.** | **Separating missing evidence from an actual absence and retaining human decision-making improved responsible use.** |

## Prompt 04 — Skills and Qualification Gap Analysis

| Version | Change made | Observed effect | Lesson learned |
|---|---|---|---|
| v1.0 | Basic gap identification | **The prompt identified potential gaps, but some missing information could be interpreted as meaning that the candidate did not have the skill.** | **The prompt needed to distinguish between a missing skill and missing evidence.** |
| v1.1 | Added categories and caution against unsupported conclusions | **The output became more cautious and organised gaps into clearer categories, but the status of each requirement was still not sufficiently standardised.** | **A defined status system was needed to make the analysis more consistent.** |
| v1.2 | Added Evidenced/Partially Evidenced/Not Evidenced status and explicit distinction between missing evidence and lack of skill | **The output clearly separated documented skills from requirements that were only partially or not evidenced in the CV.** | **Explicit status definitions reduced the risk of treating missing CV information as proof that a candidate lacks a skill.** |

## Prompt 05 — Candidate Screening Support

| Version | Change made | Observed effect | Lesson learned |
|---|---|---|---|
| v1.0 | Asked AI whether candidate should be shortlisted | **The prompt produced a direct shortlisting judgement, but it gave the AI too much responsibility for a consequential recruitment decision.** | **AI should support evidence assessment rather than independently decide whether a candidate is hired or rejected.** |
| v1.1 | Shifted to criteria-based evidence summary and human decision | **The output focused more on evidence against the selection criteria and left the final decision to the recruiter.** | **Criteria-based evaluation and human decision-making provided a safer approach.** |
| v1.2 | Added consistent criteria, exclusion of irrelevant/protected characteristics and mandatory human review | **The output applied the same job-related criteria more consistently and explicitly required human review before candidate action.** | **Recruitment prompts need consistent job-related criteria and strong human oversight.** |

## Prompt 06 — Structured Interview Question Generation

| Version | Change made | Observed effect | Lesson learned |
|---|---|---|---|
| v1.0 | Basic interview question generation | **The prompt generated relevant questions, but the questions were not consistently balanced or clearly connected to individual job requirements.** | **The prompt needed clearer requirements for question type and role alignment.** |
| v1.1 | Added number, type and job-requirement alignment | **The output became more structured and produced a defined number of technical/role-specific and behavioural questions linked to the position.** | **Specifying the expected number and type of questions improved consistency.** |
| v1.2 | Added requirement mapping, evidence to listen for and neutral wording | **The output provided interview questions together with the requirement being assessed and indicators interviewers could listen for.** | **Mapping questions to requirements makes AI generated interview material more useful and defensible.** |

## Prompt 07 — Interview Note Summarisation

| Version | Change made | Observed effect | Lesson learned |
|---|---|---|---|
| v1.0 | Basic interview summary | **The prompt produced a general summary, but important evidence and areas requiring clarification were not consistently separated.** | **A fixed structure was needed to make interview summaries more useful.** |
| v1.1 | Added structured headings and no-assumption rule | **The output was more organised and was less likely to introduce information that was not present in the interview notes.** | **Defined headings and constraints improved the reliability of summaries.** |
| v1.2 | Added evidence references, distinction between evidence and interpretation, and 'Not assessed' status | **The output more clearly separated candidate evidence from interpretation and identified competencies that had not been assessed.** | **Evidence-based summarisation and explicit uncertainty controls reduce the risk of misleading recruitment summaries.** |

## Prompt 08 — Shortlisted Candidate Comparison

| Version | Change made | Observed effect | Lesson learned |
|---|---|---|---|
| v1.0 | Asked AI to identify the best candidate | **The AI produced a direct candidate preference, but the result risked giving the AI too much influence over the final recruitment decision.** | **AI should compare evidence rather than independently select the successful candidate.** |
| v1.1 | Shifted to criteria-based comparison without autonomous decision | **The output provided a more transparent comparison of candidates against the selection criteria and avoided making the final decision.** | **Using consistent criteria makes comparisons easier for human decision-makers to review.** |
| v1.2 | Added identical criteria/output structure, evidence requirements and human-panel judgement | **The candidates were presented using the same structure and supporting evidence, while final judgement remained with the hiring panel.** | **Standardised outputs and human judgement improve consistency and reduce inappropriate reliance on AI.** |

## Prompt 09 — Recruitment Recommendation Draft

| Version | Change made | Observed effect | Lesson learned |
|---|---|---|---|
| v1.0 | Basic recommendation request | **The prompt generated a recruitment recommendation, but it could be interpreted as an AI-generated final decision** | **The output needed to be clearly positioned as decision support rather than a final recruitment decision.** |
| v1.1 | Added evidence, unresolved concerns and human review | **The output provided more supporting evidence and identified issues that required further consideration by HR.** | **Recommendations should show evidence and uncertainty rather than presenting a simple conclusion.** |
| v1.2 | Added draft label, evidence-only requirement and explicit prohibition on autonomous decisions | **The output clearly identified itself as a draft for human review and focused on documented evidence rather than unsupported conclusions.** | **Explicit human-review controls are important when AI outputs could influence consequential employment decisions.** |

## Prompt 10 — Recruitment Management Summary

| Version | Change made | Observed effect | Lesson learned |
|---|---|---|---|
| v1.0 | Basic management summary | **The prompt produced a general recruitment summary, but the information was not consistently organised around the issues management would need to review.** | **The prompt needed defined management-focused sections.** |
| v1.1 | Added required management sections and missing-information rule | **The output became more structured and highlighted missing information that required further verification.** | **Specifying the expected management structure improved usefulness and completeness.** |
| v1.2 | Added evidence/uncertainty controls, data minimisation and human-review label | **The final output better separated documented evidence from unresolved information, reduced unnecessary personal information and clearly positioned the summary for human review.** | **Management summaries benefit from structured evidence, uncertainty controls and responsible handling of candidate information.** |

---

## Evidence checklist

For every prompt, save:

- [ ] v1.0 prompt
- [ ] v1.0 output
- [ ] v1.0 observation
- [ ] v1.1 prompt
- [ ] v1.1 output
- [ ] v1.1 observation
- [ ] v1.2 prompt, if used
- [ ] v1.2 output, if used
- [ ] Final-version decision
- [ ] Lesson learned

Screenshots can be used as evidence where appropriate. Keep the test inputs consistent enough that the effect of the prompt change can be evaluated.

---
