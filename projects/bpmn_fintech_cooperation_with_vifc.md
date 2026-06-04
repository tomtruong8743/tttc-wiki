# BPMN — Fintech Company Cooperation With VIFC

*Business Process Model and Notation (BPMN) diagram for fintech companies entering VIFC.*

## Process Diagram

```mermaid
flowchart LR
    subgraph FINTECH ["💻 FINTECH COMPANY (APPLICANT)"]
        S((Start))
        G1{Entry\nPath?}
        T1A[Prepare Sandbox\nApplication\n— Decree mechanism]
        T1B[Prepare Full\nLicense Application]
        T4[Address\nDeficiencies]
        T7[Operate Under\nSandbox Conditions\nMax 2 Years]
        G2{Sandbox\nOutcome?}
        T8[Remediate Issues\n& Extend Sandbox]
        T9[Apply for\nFull Operating License]
        T10[Complete AML/KYC\nSetup]
        T11[Data Protection\nRegistration]
        T12[Begin Full\nOperations]
        T13[Monthly Reports\nAnnual Audit]
    end

    subgraph AUTH ["🏛️ VIFC FINTECH REGULATORY AUTHORITY"]
        T2{Application\nApproved?}
        T3[Request\nRevisions]
        T5[Grant Sandbox\nApproval]
        T6[Issue Full\nOperating License]
        T14[Ongoing\nSupervision]
    end
    E((End))

    S --> G1
    G1 -->|Sandbox First| T1A
    G1 -->|Full License| T1B

    T1A --> T2
    T1B --> T2
    T2 -->|Rejected| T3
    T3 --> T4
    T4 --> G1
    T2 -->|Approved Sandbox| T5
    T5 --> T7
    T7 --> G2
    G2 -->|Issues Found| T8
    T8 --> T7
    G2 -->|Successful| T9
    T2 -->|Approved Full| T6
    T9 --> T6
    T6 --> T10
    T10 --> T11
    T11 --> T12
    T12 --> T13
    T13 --> T14
    T14 --> E

    style S fill:#ffffff,stroke:#1c2f72,stroke-width:3px,color:#1c2f72
    style E fill:#1c2f72,stroke:#1c2f72,color:#ffffff
    style G1 fill:#fff7e6,stroke:#b45309
    style G2 fill:#fff7e6,stroke:#b45309
    style T2 fill:#fff7e6,stroke:#b45309
    style FINTECH fill:#f0f7ff,stroke:#1c2f72
    style AUTH fill:#e8f8ef,stroke:#276749
```

## BPMN Element Key

| Symbol | Meaning |
|--------|---------|
| ○ Thin circle | Start Event |
| ● Thick circle | End Event |
| ▭ Rectangle | Task / Activity |
| [Diamond | Gateway (Decision) |
| Swimlane | Participant / Role |

## Process Steps

### Pool: Fintech Company
1. **Gateway: Entry Path** — Regulatory sandbox or direct full license
2. **Prepare Application** — Sandbox: tech description, risk assessment, consumer protection plan, exit strategy
3. **Address Deficiencies** — If authority requests revisions
4. **Operate Under Sandbox** — Limited users, transaction caps, monthly reporting, max 2 years
5. **Gateway: Sandbox Outcome** — Successful or issues found
6. **Remediate and Extend** — If issues found during sandbox
7. **Apply for Full License** — After successful sandbox
8. **Complete AML/KYC Setup**
9. **Data Protection Registration**
10. **Begin Full Operations**
11. **Monthly Reports and Annual Audit** — Ongoing

### Pool: VIFC Fintech Regulatory Authority
1. **Review Application** — Gateway: approve or reject
2. **Request Revisions** — If rejected
3. **Grant Sandbox Approval** or **Issue Full License**
4. **Ongoing Supervision**

## Related Topics
- [[Co Che Thu Nghiem Co Kiem Soat In The Context Of Tttc]]
- [[Special Legal Mechanisms In The Vietnam International Financial Centre]]
- [[Compliance Requirements In The Vietnam International Financial Centre]]
- [[Bpmn Foreign Company Cooperation With Vifc]]

---

## Detailed Process Information

# Process Map — How Fintech Companies Cooperate With VIFC


## Key Requirements

### Regulatory Sandbox Entry
- Innovative financial technology with clear use case
- Consumer protection and risk mitigation plan
- Technical documentation of the solution
- Exit/wind-down strategy
- Minimum capital as required

### Full License Requirements
- Completed sandbox (or equivalent overseas track record)
- Full AML/KYC compliance programme
- Data localisation compliance
- Cybersecurity assessment

## Applicable Decrees
- [[Special Legal Mechanisms In The Vietnam International Financial Centre]] — sandbox framework
- [[Decree 329 Banking And Foreign Exchange]] — payment fintech
- [[Decree 324 Financial Policies Of Tttc]] — tax incentives

## Related Topics
- [[Co Che Thu Nghiem Co Kiem Soat In The Context Of Tttc]]
- [[Compliance Requirements In The Vietnam International Financial Centre]]
- [[Process Map How Foreign Companies Cooperate With Vifc]]

*Last updated: 2026-06-04*

## Update Log
- **2026-06-04**: Merged detailed process map content.
