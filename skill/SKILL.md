---
name: job-search-operator
description: Run or resume an evidence-grounded job-search pipeline that sources roles, completes applications, maintains a tracker, and conducts personalized post-application outreach.
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
- `docs/OUTREACH_PLAYBOOK.md`
- `docs/IMPROVEMENT_LOG.md`

At the start of a session, read the candidate evidence, stable answer bank, preferences, resume index, search strategy, and tracker. Never infer unsupported facts.

For each role:

1. Before opening the application, verify the employer-controlled posting is open and run a full-tracker duplicate gate using normalized company and title, requisition ID, and canonical URL.
2. Score realistic fit and enforce a one-application-per-employer 30-day cooldown unless the user explicitly approves a named exception.
3. Select or tailor the closest evidence-backed resume. Use neutral or target-specific names for every submitted document; no filename may name a different employer.
4. Draft a cover letter only when required or strategically useful.
5. Prepare role-specific answers from verified evidence.
6. Complete and audit every visible required field. Explicitly verify parsed email and phone, current location, education and employment dates, sponsorship, GPA when asked, self-identification selections supplied by the candidate, free-text answers, and uploaded filenames. On controlled forms such as Ashby, a rendered contact field can be correct while DOM or accessibility inspection reports an empty value; use a visual check before retyping so contact data is not duplicated.
7. Follow product confirmation rules immediately before consequential submission.
8. Verify receipt, update the tracker, close the tab, and repeat. At the end of a daily batch, count applications directly from the tracker by date rather than relying on the running conversational total.

Parallelize independent sourcing and document preparation only when the user authorizes delegation. Keep live browser submission serialized. The tracker has one writer; other agents may propose row data but cannot edit it concurrently. Refresh duplicates and employer concentration immediately before the final tracker write. Ask the user only for passwords, OTPs, CAPTCHAs, genuinely unknown facts, and confirmations required by the product.

After the requested daily target is verified directly in the tracker, run the post-application outreach phase when requested:

1. Build the outreach queue from exact Applied rows for the current local date.
2. Research up to two relevant people per company, prioritizing the hiring manager or team lead, then a function-aligned recruiter, then a related employee or alum.
3. Select one initial contact per company and prefer a verified work address. Keep LinkedIn research and messaging manual; do not scrape or automate LinkedIn.
4. Draft a concise note that names the applied role, explains why the person is relevant, connects one verified experience point, and makes a small informational ask. Do not attach a resume or ask a stranger directly for a referral in the first message.
5. Record the contact, source, address verification, subject, and complete draft in the private Outreach table linked to the Application ID.
6. Audit the batch, obtain the product-required action-time confirmation immediately before sending, and record only visibly sent messages as Sent.
7. Follow up once after five business days if there is no reply, then close the sequence. Stop immediately after a decline, opt-out, or request not to contact.

After a material improvement, update the process log and operating documentation. Measure outreach reply, conversation, and interview conversion rather than send volume alone. Keep private profile, tracker, contact, and message data out of public artifacts.
