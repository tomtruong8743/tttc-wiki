# BPMN — Import and Export Company Cooperation With VIFC

*Business Process Model and Notation (BPMN) diagram for import/export companies entering VIFC.*

## Process Diagram

```mermaid
flowchart LR
    subgraph COMPANY ["📦 IMPORT/EXPORT COMPANY (APPLICANT)"]
        S((Start))
        G1{Activity\nType?}
        T1A[Apply for Commodities\nExchange Membership\n— Decree 330]
        T1B[Apply for Trade\nFinance Registration]
        T1C[Apply for General\nImport/Export License]
        T4[Address\nDeficiencies]
        T7A[Access Trading\nFloor]
        T7B[Register AML/KYC\n— Decree 329]
        T7C[Register with\nCustoms Authority]
        T8[Begin Trading /\nOperations]
        T9[Ongoing Transaction\nReporting]
    end

    subgraph AUTH ["🏛️ VIFC AUTHORITY / EXCHANGE"]
        T2A{Membership\nApproved?}
        T2B{Registration\nApproved?}
        T2C{License\nApproved?}
        T3[Request\nRevisions]
        T5A[Issue Exchange\nMembership Certificate]
        T5B[Issue Trade Finance\nRegistration]
        T5C[Issue Import/Export\nBusiness License]
        T6[Ongoing Compliance\nMonitoring]
    end
    E((End))

    S --> G1
    G1 -->|Commodities| T1A
    G1 -->|Trade Finance| T1B
    G1 -->|General Trade| T1C

    T1A --> T2A
    T2A -->|Rejected| T3
    T2A -->|Approved| T5A
    T5A --> T7A

    T1B --> T2B
    T2B -->|Rejected| T3
    T2B -->|Approved| T5B
    T5B --> T7B

    T1C --> T2C
    T2C -->|Rejected| T3
    T2C -->|Approved| T5C
    T5C --> T7C

    T3 --> T4
    T4 --> G1

    T7A --> T8
    T7B --> T8
    T7C --> T8
    T8 --> T9
    T9 --> T6
    T6 --> E

    style S fill:#ffffff,stroke:#1c2f72,stroke-width:3px,color:#1c2f72
    style E fill:#1c2f72,stroke:#1c2f72,color:#ffffff
    style G1 fill:#fff7e6,stroke:#b45309
    style T2A fill:#fff7e6,stroke:#b45309
    style T2B fill:#fff7e6,stroke:#b45309
    style T2C fill:#fff7e6,stroke:#b45309
    style COMPANY fill:#f0f7ff,stroke:#1c2f72
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

### Pool: Import/Export Company
1. **Gateway: Activity Type** — Commodities trading, trade finance, or general import/export
2. **Submit relevant application** to VIFC Authority / Exchange
3. **Address Deficiencies** — If revisions requested
4. **Access Trading Floor / Register AML-KYC / Register with Customs**
5. **Begin Operations**
6. **Ongoing Transaction Reporting**

### Pool: VIFC Authority / Exchange
1. **Review Application** — Gateway per activity type
2. **Request Revisions** — If rejected
3. **Issue relevant certificate or license**
4. **Ongoing Compliance Monitoring**

## Related Topics
- [[Decree 330 Commodities Exchange In Tttc]]
- [[Decree 329 Banking And Foreign Exchange]]
- [[Cross Border Payments In The Vietnam International Financial Centre]]
- [[Bpmn Foreign Company Cooperation With Vifc]]

---

## Detailed Process Information

# Process Map — How Import and Export Companies Cooperate With VIFC


## Key Requirements

### Commodities Exchange Members (Decree 330)
- Registered company in Vietnam or foreign branch
- Minimum capital as specified in Decree 330
- Designated compliance officer
- Trading system compatibility

### Trade Finance Operators
- Financial services license or banking partnership
- AML/KYC programme compliant with Decree 329
- Foreign exchange registration for cross-border transactions

### General Import/Export Companies
- Valid business registration certificate
- Import/export business license
- Customs registration with General Department of Vietnam Customs

## Applicable Decrees
- [[Decree 330 Commodities Exchange In Tttc]] — commodities trading
- [[Decree 329 Banking And Foreign Exchange]] — cross-border payments
- [[Decree 324 Financial Policies Of Tttc]] — tax incentives on trade
- [[Decree 326 Land And Environment In Tttc]] — warehousing and logistics zones

## Related Topics
- [[Cross Border Payments In The Vietnam International Financial Centre]]
- [[Financial Products And Instruments In The Vietnam International Financial Centre]]
- [[Tax Incentives In The Vietnam International Financial Centre]]
- [[Process Map How Foreign Companies Cooperate With Vifc]]

*Last updated: 2026-06-04*

## Update Log
- **2026-06-04**: Merged detailed process map content.
