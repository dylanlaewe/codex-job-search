# Human-in-the-Loop Job Search Starter Kit

This share-safe kit shows how to configure Codex as a repeatable job-search operator. It contains blank templates only. It does not include resumes, contact information, demographic answers, job applications, passwords, or tracker data.

## What to prepare

Upload or provide:

1. Current resumes and editable source files.
2. Two or three representative cover letters.
3. LinkedIn, portfolio, and GitHub links.
4. Work history, education, projects, certifications, and verified metrics.
5. Target roles, locations, compensation range, relocation preferences, work authorization, sponsorship status, and notice period.
6. Stable application answers you want the system to reuse.
7. An existing application tracker, if any.

## Setup

1. Create a private job-search root outside this `public/` directory using `PRIVATE_ROOT_LAYOUT.md`.
2. Copy `templates/PROFILE_INTAKE_TEMPLATE.md` into the private root as `profile/CANDIDATE_FACT_BANK.md`, then complete the private copy.
3. Copy `templates/APPLICATION_ANSWER_BANK_TEMPLATE.md` into the private root as `profile/FAST_APPLICATION_ANSWER_BANK.md`, then complete the private copy.
4. Copy the preferences, search-strategy, resume-index, cover-letter-voice, tracker-schema, playbook, and improvement-log templates into the private filenames listed in `PRIVATE_ROOT_LAYOUT.md`.
5. Install or adapt `skill/SKILL.md` and replace `<JOB_SEARCH_ROOT>` with the private system path.

Never enter personal data into the template files inside `public/`. Treat them as clean masters that can be copied again.

## First prompt

Use the prompt in `templates/MASTER_PROMPT.md`. Start with one application, audit the output, then expand the batch size.

## Operating principle

Parallelize research and document preparation. Keep live form completion and tracker writes one application at a time. Require evidence for every claim, audit all required questions and submitted filenames, and let the user handle passwords, OTPs, CAPTCHAs, genuinely unknown facts, and any required final confirmation.

## Privacy

Keep the private profile, tracker, resumes, and application artifacts outside this public directory. Do not publish browser sessions, account URLs, demographic answers, or unredacted application screenshots.
