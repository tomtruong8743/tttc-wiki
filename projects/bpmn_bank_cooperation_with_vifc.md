# BPMN — Bank Cooperation With VIFC

*Business Process Model and Notation (BPMN) diagram for banks (foreign and domestic) entering VIFC.*

## Process Diagram

```mermaid
flowchart LR
    subgraph BANK ["🏦 BANK (APPLICANT)"]
        S((Start))
        G1{Foreign or\nDomestic Bank?}
        T1A[Prepare Foreign Bank\nApplication Package]
        T1B[Prepare Domestic Bank\nApplication Package]
        T2[Submit to SBV\nvia VIFC Authority]
        T3[Address\nDeficiencies]
        T6[Register with\nVIFC Authority]
        T7[Apply for Foreign\nExchange License]
        T8[Establish AML/KYC\nProgramme]
        T9[Register Reporting\nObligations]
        T10[Open Branch /\nSubsidiary Operations]
        T11[Quarterly SBV\nReports]
    end

    subgraph SBV ["🏛️ STATE BANK OF VIETNAM — SBV"]
        T4{Application\nApproved?}
        T5[Request\nRevisions]
        T12[Issue Banking\nLicense for VIFC]
        T13[Ongoing\nSupervision]
    end
    E((End))

    S --> G1
    G1 -->|Foreign| T1A
    G1 -->|Domestic| T1B
    T1A --> T2
    T1B --> T2
    T2 --> T4
    T4 -->|Rejected| T5
    T5 --> T3
    T3 --> T2
    T4 -->|Approved| T12
    T12 --> T6
    T6 --> T7
    T7 --> T8
    T8 --> T9
    T9 --> T10
    T10 --> T11
    T11 --> T13
    T13 --> E

    style S fill:#ffffff,stroke:#1c2f72,stroke-width:3px,color:#1c2f72
    style E fill:#1c2f72,stroke:#1c2f72,color:#ffffff
    style G1 fill:#fff7e6,stroke:#b45309
    style T4 fill:#fff7e6,stroke:#b45309
    style BANK fill:#f0f7ff,stroke:#1c2f72
    style SBV fill:#e8f8ef,stroke:#276749
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

### Pool: Bank (Applicant)
1. **Gateway: Foreign or Domestic?** — Determines document requirements
2. **Prepare Application Package** — License, financials, fit & proper, compliance programme
3. **Submit to SBV via VIFC Authority**
4. **Address Deficiencies** — If SBV requests revisions
5. **Register with VIFC Authority** — After license issued
6. **Apply for Foreign Exchange License** — Decree 329
7. **Establish AML/KYC Programme**
8. **Register Reporting Obligations** — With SBV
9. **Open Branch / Subsidiary Operations**
10. **Submit Quarterly SBV Reports** — Ongoing

### Pool: State Bank of Vietnam (SBV)
1. **Review Application** — Gateway: approve or reject
2. **Request Revisions** — If rejected
3. **Issue Banking License for VIFC**
4. **Ongoing Supervision**

## Related Topics
- [[Decree 329 Banking And Foreign Exchange]]
- [[Foreign Banks In The Vietnam International Financial Centre]]
- [[Domestic Banks In The Vietnam International Financial Centre]]
- [[Aml And Compliance Summary For Investment Banks In Tttc]]
- [[Bpmn Foreign Company Cooperation With Vifc]]

---

## Detailed Process Information

# Process Map — How Banks Cooperate With VIFC


## Key Requirements for Banks

### Foreign Banks
- Valid banking license from home jurisdiction
- Minimum 3 years of profitable operation
- Minimum capital as specified under Decree 329
- Fit and proper assessment for all directors and key executives
- Demonstrated compliance programme (AML/CFT)

### Domestic Banks
- Existing SBV license
- Board resolution to establish VIFC presence
- Capital ring-fenced for VIFC operations
- Designated VIFC compliance officer

## Applicable Decrees
- [[Decree 329 Banking and Foreign Exchange]] — primary licensing decree
- [[Decree 324 Financial Policies of TTTC]] — tax incentives
- [[Decree 323 Establishment of TTTC]] — governance framework

## Related Topics
- [[Foreign Banks In The Vietnam International Financial Centre]]
- [[Domestic Banks In The Vietnam International Financial Centre]]
- [[Foreign Exchange Rules In The Vietnam International Financial Centre]]
- [[Aml And Compliance Summary For Investment Banks In Tttc]]
- [[Process Map How Foreign Companies Cooperate With Vifc]]

*Last updated: 2026-06-04*

## Update Log
- **2026-06-04**: Merged detailed process map content.
