# HR Recruitment Prompt Library

## BUS4005 Assessment 1

**Business field:** Human Resources  
**Organisation type:** Medium-to-large retail organisation  
**Workflow:** Recruitment and candidate screening

## Proposed workflow

1. Job Description Analysis
2. CV Information Extraction
3. CV-to-Job Matching
4. Skills and Qualification Gap Analysis
5. Candidate Screening Support
6. Structured Interview Question Generation
7. Interview Note Summarisation
8. Shortlisted Candidate Comparison
9. Recruitment Recommendation Draft
10. Recruitment Management Summary

---

## Prompt 01 — Job Description Analysis

### Prompt Text — Proposed final version

```text
You are an HR recruitment assistant. Analyse the job description provided below and identify the key requirements for the position. Separate the requirements into education, technical skills, soft skills, experience, responsibilities and other relevant requirements. For each requirement, classify it as Mandatory or Desirable based only on the wording of the job description. Preserve the original meaning and importance of each requirement. Classify communication, teamwork, customer service and similar interpersonal abilities as soft skills. Present the results in a clear table with columns for Category, Requirement, Mandatory/Desirable, and Evidence from the Job Description. Do not infer requirements that are not stated in the job description.
```

### Intended Workflow or Task

Understand the role requirements before candidate screening.

### Problem Being Solved

Recruiters may need to manually extract and organise requirements from unstructured job descriptions before they can consistently screen applicants.

### Automation Potential

High potential for initial requirement extraction and structuring. HR should validate the output before using it as a screening basis.

### Risks and Limitations

The AI may misinterpret a requirement or change the distinction between mandatory and desirable criteria. Mitigate by requiring evidence from the job description, preserving the original meaning and requiring HR review.

---

## Prompt 02 — CV Information Extraction

### Prompt Text — Proposed final version

```text
You are an HR recruitment assistant. Extract candidate information from the CV provided. Return a table with these columns: Category, Information, Evidence from CV. Use the categories Education, Employment History, Technical Skills, Soft Skills, Certifications and Relevant Achievements. Use only information explicitly stated in the CV. Do not infer skills, qualifications, years of experience or achievements. If information is unavailable, write 'Not stated'.
```

### Intended Workflow or Task

Convert an applicant CV into structured information for screening.

### Problem Being Solved

Recruiters may repeatedly read CVs and manually extract education, experience and skills before comparing candidates.

### Automation Potential

High potential for first-pass information extraction and formatting. HR should verify important candidate information against the original CV.

### Risks and Limitations

The AI may omit, misread or invent information. Mitigate by requiring only explicit CV evidence and an 'Not stated' response for missing information.

---

## Prompt 03 — CV-to-Job Matching

### Prompt Text — Proposed final version

```text
You are an HR recruitment assistant supporting recruitment screening. Compare the supplied CV with the supplied job description. Evaluate every explicitly stated job requirement using only evidence contained in the CV. Classify each requirement as Present, Partially Present or Not Present, and provide a short evidence statement. If the CV does not provide enough information, classify it as Not Evidenced rather than making an assumption. Return a table with Requirement, Classification, Evidence and Notes. Do not make a hiring recommendation.
```

### Intended Workflow or Task

Compare an applicant's documented qualifications and experience against the job requirements.

### Problem Being Solved

Manual CV-to-job comparison can be repetitive and may produce inconsistent assessments when many applications are reviewed.

### Automation Potential

High potential for a first-pass comparison against predefined criteria. HR must review the evidence before any candidate decision.

### Risks and Limitations

The AI may treat inferred skills as evidence or incorrectly classify a requirement. Mitigate with explicit evidence requirements and a controlled Present/Partially Present/Not Present classification.

---

## Prompt 04 — Skills and Qualification Gap Analysis

### Prompt Text — Proposed final version

```text
You are an HR recruitment assistant. Using only the supplied job description and CV, identify requirements that are not sufficiently evidenced in the CV. Categorise each item as Technical Skill, Soft Skill, Experience, Education/Qualification or Other. Use one of these statuses: Evidenced, Partially Evidenced, Not Evidenced. Do not interpret 'Not Evidenced' as proof that the candidate lacks the requirement. Provide the relevant job requirement and the evidence or missing evidence in a table. Do not make a hiring recommendation.
```

### Intended Workflow or Task

Identify requirements that are not sufficiently evidenced in the candidate's CV.

### Problem Being Solved

Recruiters may spend time manually identifying missing or unclear requirements after an initial CV comparison.

### Automation Potential

High potential for identifying documented gaps and unresolved requirements. Human review is needed before interpreting gaps as evidence against a candidate.

### Risks and Limitations

A missing item in a CV does not necessarily mean the candidate lacks the skill. Mitigate by distinguishing 'not stated/not evidenced' from 'does not have'.

---

## Prompt 05 — Candidate Screening Support

### Prompt Text — Proposed final version

```text
You are an HR recruitment assistant supporting a human recruiter. Evaluate the candidate only against the supplied, job-related selection criteria. Apply the same criteria consistently and do not consider protected or irrelevant personal characteristics. For each criterion, provide Status (Evidenced, Partially Evidenced or Not Evidenced), supporting evidence and any information requiring verification. Produce an overall screening summary but do not make an autonomous hiring or rejection decision. Flag the case for human review before any candidate action is taken.
```

### Intended Workflow or Task

Support consistent initial screening against predefined recruitment criteria.

### Problem Being Solved

Initial screening can involve repetitive comparison of multiple candidates against the same criteria.

### Automation Potential

Medium-to-high potential for standardised first-pass screening. A human recruiter must review the evidence and retain decision authority.

### Risks and Limitations

Automated screening can amplify biased criteria or over-rely on proxy information. Mitigate through predefined job-related criteria, evidence requirements, consistent application and human review.

---

## Prompt 06 — Structured Interview Question Generation

### Prompt Text — Proposed final version

```text
You are an HR recruitment assistant preparing a structured interview. Using only the supplied job description, create 8 interview questions aligned with the role requirements: 4 role-specific/technical questions and 4 behavioural questions. For each question, state the job requirement being assessed and the competency or evidence the interviewer should listen for. Use neutral, job-related wording. Do not ask about protected or irrelevant personal characteristics. Do not invent role requirements that are not in the job description.
```

### Intended Workflow or Task

Prepare structured interview questions aligned to the role requirements.

### Problem Being Solved

Recruiters and hiring managers may spend repetitive time preparing role-specific interview questions.

### Automation Potential

High potential for drafting a consistent question set. HR or the hiring manager should review questions for relevance, fairness and suitability.

### Risks and Limitations

The AI may generate irrelevant, leading or inappropriate questions. Mitigate by grounding questions in job requirements and excluding protected personal characteristics.

---

## Prompt 07 — Interview Note Summarisation

### Prompt Text — Proposed final version

```text
You are an HR recruitment assistant. Structure the supplied interview notes into four sections: 1) Technical/Role Capability, 2) Behavioural Competencies, 3) Evidence Provided by the Candidate, and 4) Areas Requiring Clarification. For each finding, include a concise evidence reference using the candidate's stated information. Distinguish observed evidence from interpretation. Do not infer personality, motivation, background or suitability beyond the supplied notes. If a competency was not assessed, state 'Not assessed'.
```

### Intended Workflow or Task

Convert interview notes into structured evidence for later review.

### Problem Being Solved

Interview notes can be lengthy and inconsistently structured, creating additional administrative work when recruiters prepare candidate summaries.

### Automation Potential

High potential for summarisation and organisation. The recruiter should compare the summary with the original notes before using it.

### Risks and Limitations

Summarisation may omit important evidence or introduce interpretation. Mitigate by requiring evidence-based summaries and clearly separating stated evidence from areas requiring clarification.

---

## Prompt 08 — Shortlisted Candidate Comparison

### Prompt Text — Proposed final version

```text
You are an HR recruitment assistant supporting a human hiring panel. Compare the shortlisted candidates using only the supplied job-related selection criteria and documented candidate evidence. Apply the same criteria and output structure to every candidate. Return a table with Candidate, Criterion, Evidence, Status and Clarification Needed. Do not use protected or irrelevant personal characteristics. Do not create evidence that is not supplied. Do not make an autonomous hiring recommendation; instead identify where the hiring panel should exercise judgement.
```

### Intended Workflow or Task

Compare shortlisted candidates using the same predefined criteria.

### Problem Being Solved

Comparing multiple candidates manually can be time-consuming and may lead to inconsistent presentation of evidence.

### Automation Potential

Medium-to-high potential for standardised comparison tables. HR must verify evidence and make the final decision.

### Risks and Limitations

The AI may create false rankings or give weight to irrelevant information. Mitigate by using predefined criteria, equal treatment and no autonomous final recommendation.

---

## Prompt 09 — Recruitment Recommendation Draft

### Prompt Text — Proposed final version

```text
You are an HR recruitment assistant preparing a decision-support document for a human hiring panel. Use only the supplied job criteria and documented candidate evidence. Prepare a draft recommendation that includes: role requirements, evidence for each shortlisted candidate, unresolved issues, information requiring verification and suggested next steps. Clearly label the document as 'Draft — Human Review Required'. Do not invent evidence, infer protected characteristics or make an autonomous hiring decision. If evidence is insufficient, state that it is insufficient.
```

### Intended Workflow or Task

Prepare a draft evidence summary for HR or a hiring panel.

### Problem Being Solved

Recruiters may spend time consolidating candidate evidence into a management-ready draft after screening and interviews.

### Automation Potential

Medium potential because the output can consolidate evidence, but human review is essential because recruitment decisions are consequential.

### Risks and Limitations

A draft recommendation may be treated as an objective decision even when the underlying AI analysis is incomplete. Mitigate by labelling it as a draft, requiring evidence and keeping final authority with HR.

---

## Prompt 10 — Recruitment Management Summary

### Prompt Text — Proposed final version

```text
You are an HR recruitment assistant preparing a management-facing recruitment summary. Use only the supplied recruitment evidence. Structure the output under: Role, Selection Criteria, Shortlisted Candidates, Key Evidence, Outstanding Verification, Risks/Considerations and Next Steps. Clearly distinguish documented evidence from unresolved information. Do not include unnecessary personal information or protected characteristics. Do not make an autonomous hiring decision. Label any recommendation content as a draft requiring human review.
```

### Intended Workflow or Task

Prepare a concise management-facing summary of the recruitment process and outstanding decisions.

### Problem Being Solved

Recruitment information may be spread across screening notes, interview summaries and candidate comparisons, requiring manual consolidation for managers.

### Automation Potential

Medium-to-high potential for drafting a concise management summary. HR should verify all information before circulation.

### Risks and Limitations

The AI may omit important caveats or present an uncertain assessment as fact. Mitigate through evidence requirements, explicit uncertainty labels and human review.

---

