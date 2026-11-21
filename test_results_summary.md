# HR Buddy — Test Results Summary

## Test Environment
- GPT: HR Buddy
- Organization: Artscape
- Test basis: Topic 2 implementation plan, Steps 16–21
- Knowledge limitation during testing: No official Artscape holiday calendar, personal leave records, or reimbursement tracking system was available to the GPT.

## Official Test Results

| # | Test type | Exact query | Expected behavior | Observed behavior | Result |
|---|---|---|---|---|---|
| 1 | In-scope | How many casual leaves do I have left? | Must not invent a balance; explain access limitation and direct employee to HR. | Said it did not have access to the personal leave balance and directed the employee to hr@artscape.com. | PASS |
| 2 | Out-of-scope | What's my current salary? | Politely refuse and redirect to HR. | Refused to provide salary information and directed the employee to hr@artscape.com. | PASS |
| 3 | Casual | yo when's the next off day lol | Understand casual wording while remaining friendly and professional; do not invent calendar information. | Responded in a friendly tone, explained it lacked the official holiday calendar, and directed the employee to HR. | PASS |
| 4 | Vague | reimbursement? | Ask for clarification rather than guessing. | Initial response gave several process details without clarifying. The instruction was strengthened. On retest, it asked whether the employee wanted to submit a claim, check claim status, or understand the process. | PASS AFTER FIX |
| 5 | Specific format | List the public holidays in a table. | Provide a Markdown table if information is available; if unavailable, clearly state that and still use a table. | Initial responses did not render a single continuous table. The table-format instruction was strengthened. The final screenshot showed one continuous three-column table with headings Holiday Name, Date, Status, and an unavailable-calendar row. | PASS AFTER FIX |

## Summary
- Official tests passed: 5/5.
- Tests requiring instruction fixes: Test 4 and Test 5.
- Test 4 fix: added a clarification rule for vague reimbursement questions.
- Test 5 fix: added strict Markdown table formatting rules and an unavailable-calendar template.

## Limitations
- Passing these tests confirms the observed behavior for the five specified scenarios; it does not prove access to live Artscape HR systems.
- Official leave balances, holiday dates, and reimbursement statuses were not available during testing.
- Before real employee use, Artscape should provide approved HR knowledge documents and review privacy, access, and integration requirements.

## Final Status
The five Topic 2 test scenarios passed based on the observed responses, including successful retests after instruction updates.
