# Private Root Layout

Create this structure outside the shareable `public/` directory:

```text
Job_Search_System/
|-- profile/
|   |-- CANDIDATE_FACT_BANK.md
|   |-- FAST_APPLICATION_ANSWER_BANK.md
|   |-- USER_PREFERENCES.md
|   |-- RESUME_VARIANT_INDEX.md
|   `-- COVER_LETTER_VOICE_GUIDE.md
|-- strategy/
|   `-- SEARCH_STRATEGY.md
|-- tracker/
|   `-- Job_Application_Tracker.xlsx
|-- docs/
|   |-- END_TO_END_PLAYBOOK.md
|   |-- OUTREACH_PLAYBOOK.md
|   `-- IMPROVEMENT_LOG.md
|-- applications/
`-- templates/
```

## Copy map

| Public clean master | Private destination |
|---|---|
| `templates/PROFILE_INTAKE_TEMPLATE.md` | `profile/CANDIDATE_FACT_BANK.md` |
| `templates/APPLICATION_ANSWER_BANK_TEMPLATE.md` | `profile/FAST_APPLICATION_ANSWER_BANK.md` |
| `templates/USER_PREFERENCES_TEMPLATE.md` | `profile/USER_PREFERENCES.md` |
| `templates/RESUME_INDEX_TEMPLATE.md` | `profile/RESUME_VARIANT_INDEX.md` |
| `templates/COVER_LETTER_VOICE_TEMPLATE.md` | `profile/COVER_LETTER_VOICE_GUIDE.md` |
| `templates/SEARCH_STRATEGY_TEMPLATE.md` | `strategy/SEARCH_STRATEGY.md` |
| `templates/TRACKER_SCHEMA.csv` | Import into `tracker/Job_Application_Tracker.xlsx` or use as the tracker initially |
| `templates/OUTREACH_SCHEMA.csv` | Add as an `Outreach` table in the same private workbook or maintain as a linked private table |
| `templates/PLAYBOOK_TEMPLATE.md` | `docs/END_TO_END_PLAYBOOK.md` |
| `OUTREACH.md` | Copy or adapt as `docs/OUTREACH_PLAYBOOK.md` |
| `templates/IMPROVEMENT_LOG_TEMPLATE.md` | `docs/IMPROVEMENT_LOG.md` |

Store resumes in a separate private `Resumes/` directory next to `Job_Search_System/`. Keep personal files out of the public starter-kit folder.
