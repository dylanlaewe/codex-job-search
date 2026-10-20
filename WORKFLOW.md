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
       Record reusable improvements
```

Preparation may run in parallel when authorized. Browser submission remains serialized to prevent conflicting form state and unclear submission status.
