# Workflow

```text
Candidate evidence + preferences + resumes
                  |
                  v
       Official job verification
                  |
                  v
  Full-tracker duplicate/cooldown gate
     (company/title, req ID, URL)
                  |
                  v
            Fit scoring
                  |
        +---------+---------+
        |         |         |
        v         v         v
   Resume fit  Cover letter  Answer prep
        +---------+---------+
                  |
                  v
      One live browser application
                  |
                  v
      Full form and filename audit
                  |
                  v
     Human checkpoint when required
                  |
                  v
        Submit and verify receipt
                  |
                  v
       Update tracker and close tab
                  |
                  v
     Daily application target met?
             |           |
            no          yes
             |           |
             |           v
             |   Research one relevant contact
             |           |
             |           v
             |   Draft and audit outreach note
             |           |
             |           v
             |   Confirm, send, and log result
             |           |
             |           v
             |   One follow-up after five
             |   business days if no reply
             |           |
             +-----------+
                  |
                  v
       Record reusable improvements
```

Preparation may run in parallel when authorized. Browser submission and tracker writes remain serialized to prevent conflicting state. Outreach uses one initial contact per company, a verified business address where possible, manual-only LinkedIn research, and a private outreach log linked to the exact Application ID.
