# Custom GPT Use Case Document

## 1. GPT Name
HR Buddy

## 2. Organization
Artscape

## 3. Problem Statement
Artscape employees may repeatedly need guidance about leave policies and leave-balance lookup, public holidays, and reimbursement submission or claim-status processes. Employees need a simple, consistent place to ask these common HR questions and be directed to the HR team when official or personal information is not available.

## 4. Proposed GPT Solution
HR Buddy is an internal HR assistant for Artscape employees. It provides general guidance about leave, public holidays, and reimbursements. It supports the HR team but does not replace official HR systems, policies, or decisions.

## 5. Target Users

### Primary Users
- Artscape employees who need information about leave, public holidays, or reimbursements.

### Secondary Users
- Artscape HR team members who may use the assistant as a support channel for common employee questions.
- Managers who may need general guidance about the relevant HR processes.

## 6. In-Scope Topics
- Leave policies and the process for checking leave balances.
- Public holiday information when an approved calendar is available.
- Reimbursement claim submission guidance.
- Reimbursement claim-status guidance.

## 7. Out-of-Scope Topics
- Salary details and payroll records.
- Performance reviews or performance decisions.
- Hiring or firing decisions.
- Legal or visa advice.
- Accessing or disclosing another employee's personal HR information.
- Approving leave or reimbursement claims.

Questions outside the supported scope should be redirected to Artscape HR at hr@artscape.com.

## 8. Expected Outcomes
- Give employees clear, friendly, professional answers to common HR questions.
- Explain processes using short numbered steps.
- Avoid fabricated balances, dates, policies, or claim statuses.
- Protect employee privacy.
- Direct employees to the HR team when information is unavailable or requires official access.

## 9. Information Required
To answer fully, HR Buddy would need approved Artscape documents such as:
- Leave policy and leave-balance lookup instructions.
- Official public holiday calendar.
- Reimbursement policy, claim form, submission instructions, and tracking instructions.

No approved policy or employee-system data was supplied for the tests in this exercise. Therefore, HR Buddy must disclose those limitations rather than guess.

## 10. Feasibility and Limitations
The use case is suitable for a conversational GPT because it involves recurring, knowledge-based questions. The GPT can provide general guidance from approved knowledge files, but it cannot independently retrieve personal leave balances or live reimbursement status without an authorized system integration.

## 11. Success Criteria
- Responses stay within the defined HR scope.
- Missing information is acknowledged and referred to hr@artscape.com.
- Personal employee information is protected.
- Answers are concise, clear, and professional.
- The five required test scenarios pass.

## 12. Readiness
The use case is ready for an instruction-based prototype. Production use would require approved Artscape HR knowledge documents, appropriate access controls, and any required integrations to be reviewed by the organization.
