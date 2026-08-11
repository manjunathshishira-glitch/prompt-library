# HR Recruitment AI Prompt Library

## BUS4005 Assessment 1 — Prompt Library & Consultancy Pitch

### Project overview

This portfolio documents a proposed AI-enabled recruitment workflow for a medium-to-large retail organisation. The objective is to use a library of 10 carefully designed prompts to support repetitive recruitment activities while retaining human oversight for consequential decisions.

The proposed workflow is:

**Job description analysis → CV information extraction → CV/job matching → skills-gap identification → candidate screening support → interview question generation → interview-note summarisation → candidate comparison → recommendation drafting → recruitment summary**

The assessment requires each prompt to document:

1. Prompt text
2. Intended workflow or task
3. Problem being solved
4. Automation potential
5. Risks and limitations

It also requires evidence of iterative improvement. This repository therefore contains prompt versions and an iteration log.

---

## Business context

**Business field:** Human Resources  
**Organisation type:** Medium-to-large retail organisation  
**Workflow:** Recruitment and candidate screening

### Business problem

Recruitment teams can spend substantial administrative effort reviewing applications, extracting candidate information, comparing applicants with role requirements, preparing interview material, summarising interview information and preparing recruitment documentation.

The proposed prompt library is intended to support these repetitive activities, improve consistency of information handling and reduce manual preparation work.

The AI is **not** intended to make autonomous hiring decisions. HR remains responsible for validating AI outputs and making final recruitment decisions.

---

## Prompt library

| # | Prompt | Recruitment workflow stage |
|---|---|---|
| 01 | Job Description Analysis | Understand role requirements |
| 02 | CV Information Extraction | Structure candidate information |
| 03 | CV-to-Job Matching | Compare candidate with role |
| 04 | Skills and Qualification Gap Analysis | Identify missing requirements |
| 05 | Candidate Screening Support | Support consistent initial screening |
| 06 | Structured Interview Question Generation | Prepare interviews |
| 07 | Interview Note Summarisation | Structure interview evidence |
| 08 | Shortlisted Candidate Comparison | Compare candidates consistently |
| 09 | Recruitment Recommendation Draft | Prepare evidence-based draft |
| 10 | Recruitment Management Summary | Prepare management-facing summary |

The individual prompt files are stored in the `prompts/` folder.

---

## Prompting strategies used

The prompts use the assessment's suggested prompting strategies and related design principles, including:

- **RACE-style structure:** role, action, context and expectation
- **Context specification:** defining the recruitment situation and required inputs
- **Structured outputs:** tables, headings and defined categories
- **Constraints:** instructions such as using only supplied information and not inventing missing information
- **Task decomposition/chaining:** using separate prompts for different stages of the recruitment workflow
- **Human-in-the-loop controls:** requiring HR review for outputs that may influence recruitment decisions
- **Iterative refinement:** improving prompts after testing and observing outputs

---

## Responsible use

Recruitment is a high-impact business context. AI outputs should therefore be treated as decision-support rather than final decisions.

Key risks include:

- hallucinated or unsupported candidate information
- misclassification of qualifications or experience
- bias or inconsistent treatment of candidates
- privacy and handling of personal information
- over-reliance on AI-generated recommendations
- incorrect or misleading summaries

Potential controls include:

- using only information supplied in approved inputs
- requiring the AI to flag missing information instead of inventing it
- applying consistent assessment criteria
- minimising unnecessary personal information
- requiring human review before consequential decisions
- keeping prompt versions and testing evidence

---

## Iteration evidence

The `iteration-log.md` file records the intended development of each prompt.

**Important:** The `Observed effect` and `Lesson learned` fields must be completed using the actual outputs obtained when each prompt version is tested. Do not present hypothetical observations as real testing evidence.

For each prompt, the recommended development process is:

1. Test v1.0
2. Record what happened
3. Identify a specific weakness
4. Create v1.1
5. Test again
6. Record the new result
7. Create v1.2 if another improvement is justified
8. Test again
9. Select the final version

---

## Suggested portfolio structure

```text
README.md
prompt-library.md
iteration-log.md
prompts/
  prompt-01-job-description-analysis.md
  prompt-02-cv-information-extraction.md
  prompt-03-cv-job-matching.md
  prompt-04-skills-gap-analysis.md
  prompt-05-candidate-screening.md
  prompt-06-interview-questions.md
  prompt-07-interview-summary.md
  prompt-08-candidate-comparison.md
  prompt-09-recommendation-draft.md
  prompt-10-management-summary.md
```

---

## Assessment connection

The portfolio is designed to support the assessment requirements for a 10-prompt workflow automation library, iterative prompt development, business value analysis, risk evaluation, responsible use and a management-level consultancy pitch.

The portfolio should be linked in the final assessment submission.

