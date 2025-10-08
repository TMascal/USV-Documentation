# Handbook of Marine Craft Hydrodynamics and Motion Control
***
# *Handbook of Marine Craft Hydrodynamics and Motion Control* (1st ed.) — brief intro & relevance to USVs

Thor I. Fossen’s 1st-edition handbook ties together **hydrodynamic modeling** and **guidance–navigation–control (GNC)** for marine vehicles. It starts from first principles (6-DOF kinematics/dynamics, added mass, damping, restoring forces) and then layers on **environmental loads** (wind, waves, current), **reference frames**, **parameter identification**, and **modern control/estimation** (e.g., PID/LQR/backstepping, observers/Kalman filters). For USV work, it’s a turnkey pathway from equations → simulation → controller → sea trials.

**How this maps to USV development (at a glance)**

* **Model the plant:** Build 3-DOF (surge–sway–yaw) or 6-DOF equations; include added mass, nonlinear/linear damping, and hydrostatics for your hull form.
* **Capture the environment:** Add quasi-steady wind loads, wave-induced disturbances, and current; define your operating envelope and design margins.
* **Design the GNC stack:** LOS/path-following guidance → state estimation (GNSS/IMU fusion) → autopilots for speed/heading/track/station-keeping.
* **Parameter identification:** Use bollard-pull, zig-zag, and turning-circle trials (or CFD/tank data) to fit damping/response constants for control-oriented models.
* **Toolchain:** Translate models to state space for simulation and controller tuning; implement control allocation for differential thrust or rudder-prop setups.

---

# [Chapter 7 (1st ed.): *Models for Ships, Offshore Structures, and Underwater Vehicles*](Info Sheets/Additional References/Handbook Marine Craft Hydrodynamic and Motion Control Chapter 7.pdf) — what’s inside & how to use it for USVs

**What Chapter 7 gives you**

* A **canonical way to build dynamic models**: rigid-body inertia, **added-mass** matrices, **Coriolis/centripetal** terms (rigid-body and added-mass), **hydrostatic restoring**, and **damping** (linear & nonlinear).
* **Environment & excitation** templates: wind, wave, and current representations ready to plug into the equations of motion.
* **Control inputs & actuators**: how to represent propulsion/rudder (or thrusters) inside the model and handle constraints/saturation.
* A **control-oriented reduction**: how to step down from full 6-DOF to practical **3-DOF yaw-plane** models (e.g., Nomoto-type) for heading/course control.

**Direct USV applications (step-by-step)**

1. **Choose model order**

    * Harbor/coastal USV: start with **3-DOF (u, v, r)**; add heave/roll/pitch only if seakeeping or sensor alignment demands it.
2. **Assemble system matrices**

    * Form **M = MRB + MA**, **C(ν) = CRB(ν) + CA(ν)**, **D(ν)** (split linear/quadratic surge/sway/yaw damping), and **g(η)** (restoring).
3. **Add loads & disturbances**

    * Include **wind moments** about CG, **current-relative velocities** for hydrodynamic damping, and optional low-order **wave disturbances** for robustness tests.
4. **Map actuators to forces**

    * Build a **control-allocation matrix** for your layout (twin outboards, azimuth thrusters, differential thrust). Enforce **saturation & rate limits**.
5. **Derive a course/heading model**

    * Identify a **Nomoto 1st/2nd-order** yaw model (fit **K, T** or higher-order coefficients) from **zig-zag** or **PMM**/free-running trials.
6. **Design the autopilots**

    * Start with **heading PI/PID** (anti-windup; rate feedback if available). Extend to **track-keeping** with **LOS guidance** and **speed control**.
7. **Estimate states & reject disturbances**

    * Fuse **GNSS + IMU** (and compass/DVL if available) via an **EKF**; include a bias/disturbance state for wind/wave rejection.
8. **Verify in simulation, then wet-test**

    * Run scripted missions (transit, loiter, station-keep) with gusts and currents. Check **gain/phase margins**, actuator usage, and energy draw before sea trials.

**Quick implementation checklist for your USV**

* [ ] Define hull CG/CB, principal dimensions; estimate **added mass** (literature/CFD/tank).
* [ ] Build **M, C, D, g** and validate numerically (energy/passivity checks).
* [ ] Specify **propulsor models** (thrust vs. RPM or command), dead-zones, and rate limits.
* [ ] Collect data (10/10 **zig-zag**, step rudder/thrust) and **fit Nomoto** parameters.
* [ ] Implement **heading → course → track** controllers with **LOS** and limiter logic.
* [ ] Add **EKF** for pose/velocity; include gyro bias and sideslip (if needed).
* [ ] Stress-test with wind/current; tune for **robustness** and **actuator thermal limits**.
* [ ] Prepare **on-water acceptance tests** (waypoint accuracy, path-keeping RMS, station-keeping error, fuel/power metrics).

---

### Disclaimer
Markdown formatting and copyediting done with the aid of OpenAI ChatGPT-5. Content was reviewed and curated by  
Tim Mascal, October 2025.

NOT REVIEWED as of 10.8.25

*Prepared by: Embry-Riddle Department of Mechanical Engineering*  
*Last Updated: October 8, 2025*  
