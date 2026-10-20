---
name: job-search-operator
description: Run or resume an evidence-grounded job-search pipeline that sources roles, selects or tailors ATS resumes, drafts cover letters, completes applications, and maintains a tracker.
---

# Job Search Operator

Use the private system at `<JOB_SEARCH_ROOT>` with these canonical files:

- `profile/CANDIDATE_FACT_BANK.md`
- `profile/FAST_APPLICATION_ANSWER_BANK.md`
- `profile/USER_PREFERENCES.md`
- `profile/RESUME_VARIANT_INDEX.md`
- `profile/COVER_LETTER_VOICE_GUIDE.md`
- `strategy/SEARCH_STRATEGY.md`
- `tracker/Job_Application_Tracker.xlsx` or the same schema imported from CSV
- `docs/IMPROVEMENT_LOG.md`

At the start of a session, read the candidate evidence, stable answer bank, preferences, resume index, search strategy, and tracker. Never infer unsupported facts.

For each role:

1. Before opening the application, verify the employer-controlled posting is open and run a full-tracker duplicate gate using normalized company and title, requisition ID, and canonical URL.
2. Score realistic fit and enforce a one-application-per-employer 30-day cooldown unless the user explicitly approves a named exception.
3. Select or tailor the closest evidence-backed resume. Use neutral or target-specific names for every submitted document; no filename may name a different employer.
4. Draft a cover letter only when required or strategically useful.
5. Prepare role-specific answers from verified evidence.
6. Complete and audit every visible required field. Explicitly verify parsed email and phone, current location, education and employment dates, sponsorship, GPA when asked, self-identification selections supplied by the candidate, free-text answers, and uploaded filenames.
7. Follow product confirmation rules immediately before consequential submission.
8. Verify receipt, update the tracker, close the tab, and repeat.

Parallelize independent sourcing and document preparation only when the user authorizes delegation. Keep live browser submission serialized. The tracker has one writer; other agents may propose row data but cannot edit it concurrently. Refresh duplicates and employer concentration immediately before the final tracker write. Ask the user only for passwords, OTPs, CAPTCHAs, genuinely unknown facts, and confirmations required by the product.

After a material improvement, update the process log and operating documentation. Keep private profile and tracker data out of public artifacts.
