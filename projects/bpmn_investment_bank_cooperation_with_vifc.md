# BPMN — Investment Bank Cooperation With VIFC

*Business Process Model and Notation (BPMN) diagram for investment banks and securities firms entering VIFC.*

## Process Diagram

```mermaid
flowchart LR
    subgraph IB ["🏛️ INVESTMENT BANK (APPLICANT)"]
        S((Start))
        T1[Define Service Scope\nECM · DCM · M&A · Brokerage]
        T2[Prepare License\nApplication Package]
        T3[Submit to SSC\nvia VIFC Authority]
        T4[Address\nDeficiencies]
        T7[Register Capital Markets\nActivities with SSC]
        T8[Apply for Tax\nIncentives — Decree 324]
        T9[Establish AML/KYC\nProgramme]
        T10[Register Reporting\nObligations]
        T11[Obtain Work Permits\nfor Key Staff — Decree 325]
        T12[Begin Operations]
        T13[Quarterly Reports\nAnnual Audit]
    end

    subgraph SSC ["🏛️ STATE SECURITIES COMMISSION — SSC"]
        T5{Application\nApproved?}
        T6[Request\nRevisions]
        T14[Issue Securities\nOperating License]
        T15[Ongoing Market\nSupervision]
    end
    E((End))

    S --> T1
    T1 --> T2
    T2 --> T3
    T3 --> T5
    T5 -->|Rejected| T6
    T6 --> T4
    T4 --> T3
    T5 -->|Approved| T14
    T14 --> T7
    T7 --> T8
    T8 --> T9
    T9 --> T10
    T10 --> T11
    T11 --> T12
    T12 --> T13
    T13 --> T15
    T15 --> E

    style S fill:#ffffff,stroke:#1c2f72,stroke-width:3px,color:#1c2f72
    style E fill:#1c2f72,stroke:#1c2f72,color:#ffffff
    style T5 fill:#fff7e6,stroke:#b45309
    style IB fill:#f0f7ff,stroke:#1c2f72
    style SSC fill:#e8f8ef,stroke:#276749
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

### Pool: Investment Bank (Applicant)
1. **Define Service Scope** — ECM, DCM, M&A Advisory, Brokerage, Fund Management
2. **Prepare Application** — Home license, 3yr financials, fit & proper, compliance programme
3. **Submit to SSC via VIFC Authority**
4. **Address Deficiencies** — If SSC requests revisions
5. **Register Capital Markets Activities** — With SSC
6. **Apply for Tax Incentives** — Decree 324
7. **Establish AML/KYC Programme** — Decree 329
8. **Register Reporting Obligations**
9. **Obtain Work Permits for Key Staff** — Decree 325
10. **Begin Operations**
11. **Quarterly Reports and Annual Audit** — Ongoing

### Pool: State Securities Commission (SSC)
1. **Review Application** — Gateway: approve or reject
2. **Request Revisions** — If rejected
3. **Issue Securities Operating License**
4. **Ongoing Market Supervision**

## Related Topics
- [[Investment Banking Opportunities In The Vietnam International Financial Centre]]
- [[Securities Activities In The Vietnam International Financial Centre]]
- [[Decree 329 Banking And Foreign Exchange]]
- [[Bpmn Bank Cooperation With Vifc]]
- [[Bpmn Foreign Company Cooperation With Vifc]]

---

## Detailed Process Information

# Process Map — How Investment Banks Cooperate With VIFC


## Key Requirements

- Valid securities / investment banking license from home jurisdiction
- Minimum 3 years operating history
- Capital adequacy meeting VIFC requirements
- Fit and proper assessment for all licensed representatives
- Segregated client asset accounts
- Compliance officer designated for VIFC operations

## Services Permitted at VIFC
- Equity and debt capital markets underwriting
- Mergers and acquisitions advisory
- Securities brokerage and market making
- Fund structuring and management
- Derivatives and structured products (subject to approval)

## Applicable Decrees
- [[Decree 329 Banking And Foreign Exchange]] — securities and FX
- [[Decree 324 Financial Policies Of Tttc]] — tax incentives
- [[Decree 323 Establishment Of Tttc]] — governance
- [[Decree 325 Labor And Social Security In Tttc]] — key personnel

## Related Topics
- [[Investment Banking Opportunities In The Vietnam International Financial Centre]]
- [[Equity Capital Markets In The Vietnam International Financial Centre]]
- [[Debt Capital Markets In The Vietnam International Financial Centre]]
- [[Securities Activities In The Vietnam International Financial Centre]]
- [[Process Map How Foreign Companies Cooperate With Vifc]]

*Last updated: 2026-06-04*

## Update Log
- **2026-06-04**: Merged detailed process map content.
