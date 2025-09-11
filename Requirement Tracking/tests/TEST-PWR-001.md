---
id: "T-NAV-045"
title: "Power Input Check (24V Drill Battery) — SYS-PWR-001"
type: "test_procedure"
status: "Draft"            # Draft | Ready | Executed | Archived
owner: "MOB-SEA"
requirement_ref: "SYS-PWR-001"
verification_method: "Test"
acceptance_criteria: "Every measured voltage at the system's main power input is between 20.0 V and 29.2 V (inclusive) while powered by a 24 V drill battery."
location: "LB-172"
---

# 1) Goal
Prove the system uses a 24 V class input by **measuring the voltage at the main power connector** while running from a **24 V drill battery**. Pass if all measurements are **20.0–29.2 V**.

# 2) What you need
- **24 V drill battery** (fully charged) and the **battery-to-system adapter/cable** (with inline fuse if available)
- **Digital Multimeter (DMM)**, DC volts
- The **system (USV)**

# 3) Safety (read this)
- Batteries can supply high current. **Check polarity**, avoid shorting leads, and keep metal objects away.
- If you have a fused adapter, use it. If anything smells hot or looks damaged, **stop**.

# 4) Setup
1. Write down the battery **brand/model** and **charge status** (e.g., “full”, “2 bars”).
2. With the system **OFF**, connect the DMM to the **main power input** test points/pins (measure where the system actually receives power, not at the battery terminals).
3. Verify the adapter wiring and polarity match the system pinout.

# 5) Test steps (record in the table)
1. **Open-circuit check (before connecting):**  
   Measure battery voltage at the adapter **without** the system connected. Record as **OCV**.
2. **Power the system (Idle):**  
   Connect the battery to the system and turn the system **ON**. Wait ~5–10 s.  
   Measure and record **V_in (Idle)** at the main input.
3. **Nominal activity (if available):**  
   Put the system in a typical operating mode (motors off, sensors on—whatever “normal” is).  
   Measure and record **V_in (Nominal)**.
4. **Low battery (optional but nice):**  
   If you have another pack that’s partly discharged (or after some runtime), repeat Step 2 for **V_in (Low)** when the pack indicator shows near-low.  
   *If no low pack is available, skip this row.*

5. Power **OFF** and disconnect.

# 6) Data table
| Condition         | Voltage at Main Input (V) | Pass? (20.0–29.2) | Notes |
|-------------------|---------------------------:|:------------------:|-------|
| OCV (no load)     |                           |        N/A         |       |
| ON – Idle         |                           |                    |       |
| ON – Nominal (opt)|                           |                    |       |
| ON – Low (opt)    |                           |                    |       |

# 7) Pass/Fail
- **Pass** if every measured “ON” value is **≥ 20.0 V and ≤ 29.2 V**.
- Otherwise **Fail**.

# 8) Attachments (optional but helpful)
- Photo of the connection at the main input
- Photo of the DMM display during “ON – Idle”

# 9) Sign-off
- Tester: __________________  Date: ______
- Witness (opt): ___________  Date: ______
- Approver: ________________  Date: ______

# 10) Change log
- 2025-09-11: Initial student-friendly, battery-based procedure for SYS-PWR-001.
