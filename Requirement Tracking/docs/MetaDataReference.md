# ID
| Aspect     | Guidance                                                            | Example                              | 
|------------|---------------------------------------------------------------------|--------------------------------------|
| Purpose    | Stable, unique handle for the requirement. **Never changes.**       | `SYS-NAV-0012`                       |
| Location   | Front matter **and** file name (file name is authoritative).        | `requirements/SYS-NAV-0012.md`       |
| Format     | `CLASS-DOMAIN-####` (4 digits).                                     | `IFC-COMM-0021`                      |
| Classes    | `STKH` \| `SYS` \| `SUB` \| `IFC` \| `SAF` \| `SEC` \| `CON`        | `SAF-HULL-0005`                      | 
| Domain     | 2–8 uppercase letters (your subsystems list).                       | `NAV`, `PWR`, `CTRL`, `COMM`, `HULL` | 
| Numbering  | **Counts within the prefix bucket** (`SYS-NAV-*`, `IFC-COMM-*`, …). | `SYS-NAV-0001`, `SYS-NAV-0002`       |
| Validation | STKH                                                                | SYS                                  |
| Don’t      | Rename/reuse IDs; encode dates/priority in the ID.                  | —                                    |




# Type Reference
|        Type         |                                      Definition                                      |                     When to use                     |     Typical verification     |                            Example (AUV-flavored)                             |
|:-------------------:|:------------------------------------------------------------------------------------:|:---------------------------------------------------:|:----------------------------:|:-----------------------------------------------------------------------------:|
|   **stakeholder**   |            Stated need/goal from users/customers—not fully technical yet.            |      Early capture of mission/operator needs.       |     Review / Inspection      |     “The operator shall be able to deploy the vehicle within 10 minutes.”     |
|     **system**      |             Top-level system behavior/capability that must be delivered.             |          Whole-system “shall” statements.           |     Test / Demonstration     |              “The AUV shall follow a preplanned waypoint route.”              |
|     **derived**     |           Flow-down from higher-level reqs or design decisions to a part.            |   Allocate requirements to subsystems/components.   |       Test / Analysis        |            “The DVL shall measure velocity with ≤0.02 m/s error.”             |
|    **interface**    |    Interactions between items (mechanical, electrical, data, protocols, timing).     |      Anything about connections or exchanges.       |      Inspection / Test       |       “Telemetry shall use UDP on 192.168.2.0/24, port 5600, at ≥5 Hz.”       |
|   **performance**   |  Quantifies *how well* a behavior occurs (accuracy, latency, throughput, capacity).  |           Numeric service-level targets.            |       Test / Analysis        |                 “Position error ≤2.0 m CEP (95%) over 10 km.”                 |
|   **constraint**    |     Limits you must not exceed (mass, size, power, cost) or mandated approaches.     |       Physical/resource caps; mandated tech.        |    Inspection / Analysis     |                          “Vehicle dry mass ≤ 28 kg.”                          |
|     **safety**      |                      Hazard controls, interlocks, safe states.                       |             Preventing/mitigating harm.             |      Test / Inspection       |          “Thrusters shall remain de-energized while hatch is open.”           |
|    **security**     |                 AuthN/AuthZ, confidentiality, integrity, hardening.                  |    Protect command/telemetry, data, and access.     |       Test / Analysis        |         “Command link shall use TLS 1.3 with mutual authentication.”          |
|   **reliability**   |           Availability, MTBF/MTTR, graceful degradation, restart behavior.           |        Up-time and failure behavior targets.        |       Analysis / Test        |  “System shall achieve ≥95% mission completion without manual intervention.”  |
| **maintainability** |                    Service time, diagnostics, modularity, access.                    |       How quickly/easily it can be serviced.        |  Demonstration / Inspection  |               “Battery replacement ≤ 5 minutes without tools.”                |
|    **usability**    |          HMI clarity, operator load, alerts/acknowledgments, accessibility.          |         Human interaction and UI behavior.          |      Test / Inspection       |                  “Alarm banner readable at 1 m in 10k lux.”                   |
|  **environmental**  |           Operating/storage conditions; ingress; vibration/shock; EMI/EMC.           |  Physical environment constraints & survivability.  |       Test / Analysis        |                    “Operate 0–35 °C; IP68 to 30 m depth.”                     |
|   **compliance**    |                      Conformance to laws/standards/regulations.                      |       When a recognized standard must be met.       |      Inspection / Test       |                 “Conform to IEC 60945 environmental testing.”                 |
