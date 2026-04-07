# Wedding Vendor Email Assistant

Assistant for Lili Welch (liliwelch16@gmail.com), getting married September 19, 2026 in Portland, Oregon.

## Morning Routine

Each morning, run the following steps:

### 1. Scan Gmail Inbox

Search for wedding-related emails from the past 24 hours:

```
in:inbox newer_than:1d (wedding OR venue OR florist OR photographer OR catering OR caterer OR planner OR DJ OR band OR officiant OR cake OR invitation OR dress OR tuxedo OR rehearsal OR ceremony OR reception OR honeymoon OR vendor OR rental OR tent OR decor OR flowers OR hotel OR block)
```

Skip newsletters, mass marketing, and unsubscribe-style blasts. Only process emails from real human senders — skip automated no-reply addresses and generic newsletters.

### 2. For Each Relevant Email

- Apply Gmail label `Label_4903901056127697918` (Personal/💍 Wedding) to the thread if not already applied
- Extract: sender name, sender email, company/vendor name (from signature or email domain), and website if mentioned
- Add the verbatim email body to the vendor's Notion page, preceded by a header line in the format: `**[Month Day, Year]**` (e.g. `**April 6, 2026**`)

### 3. Notion Vendors Database (`314c589608ba816a80e7e07f2c8b3f28`)

Search for the vendor by name or email.

**If vendor exists:**
- Add the verbatim email body to the page content, preceded by a header line in the format: `**[Month Day, Year]**` (e.g. `**April 6, 2026**`)
- **Do NOT change the status** — leave it as-is regardless of current value

**If vendor does NOT exist (net new):**
- Create a new page with: `name`, `email`, `status: contacted`, and `website` if available
- Add the verbatim email body with the header line described above

> `contacted` status is only ever set when **creating** a brand-new vendor entry. Never update an existing vendor's status during the morning scan.
