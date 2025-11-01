<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/777efd2e-f1fc-4386-9583-8414c6be0861" />

# 🌌 Interstellar Propulsion Analytics
### *Presented by the AstroDynamics Research Division*  
#### United Terran Federation · Luna Prime Headquarters  

---

> *“Between the stars, energy is the language of survival.”*

Welcome, Cadet Engineer.  
You are joining the **AstroDynamics Research Division (ADR)** — the research wing of the **United Terran Federation**.  
Your assignment: analyse the propulsion and energy systems of the **Helios-V Deep-Space Vessel**, operating within the **Epsilon Eridani** system.

This assessment evaluates your ability to:
- Analyse high-dimensional telemetry from an interstellar propulsion platform  
- Build quantitative models that predict system behaviour  
- Translate noisy data into actionable insight for long-range missions  

---

### Mission Context
Telemetry from two consecutive orbital cycles has been logged by the Helios-V:

| Cycle | Description | Collector Status |
|:--|:--|:--|
| **Cycle 1** | Nominal operation under stable stellar conditions | ✅ Active |
| **Cycle 2** | Nominal operation under stable stellar conditions | ✅ Active |
| **Cycle 3 (The next cycle)** | Expect slightly lower irradiance | ✅ Active |

The first two cycles contain full system telemetry, including irradiance and energy reserve readings.  
We are preparing for our third cycle, **the ship follows a pre-defined trajectory and speed profile**, but most data (like irradiance) are still unknown.

Your mission is to **forecast the Helios-V’s remaining energy at the end of Cycle 3**.

---

### Dataset Overview
Each record corresponds to a snapshot of the vessel’s propulsion and energy state.

| Column | Description |
|:--|:--|
| `mission_time` | Mission timestamp (local ship time). |
| `ship_speed_kps` | Ship velocity (km/s). |
| `reactor_output_A` | Main reactor output current (A). |
| `reactor_voltage_V` | Reactor bus voltage (V). |
| `stellar_irradiance_Wm2` | Incident stellar irradiance (W/m²). |
| `collector_A_W`, `collector_B_W`, `collector_C_W` | Output from three independent radiant-energy collectors (W). |
| `helio_remaining_energy` | Remaining Helios-core energy reserve (arbitrary units). |
| `orbital_inclination_deg` | Orbital inclination (°). |
| `orbital_longitude_deg` | Orbital longitude (°). |
| `orbital_altitude_km` | Altitude above the reference plane (km). |

> **Note:**  
> - For Cycle 3, most of the columns are missing.

---

### Mission Objective
1. Explore and interpret Cycles 1–2 telemetry to understand **energy inflow and outflow dynamics**.  
2. Identify relationships between propulsion load, stellar irradiance, and collector performance.  
3. Develop a model that can **predict the evolution of `helio_remaining_energy`** over time for Cycle 3.  
4. Estimate the **end-of-cycle energy reserve** once the vessel completes its trajectory and powers down.

While analysing, you are encouraged to:
- Report **any anomalies or inconsistencies** in the telemetry (e.g., sensor drift, missing values, unrealistic transients).  
- Discuss potential **physical explanations** behind these behaviours.  
- Balance **data-driven modelling** with **physics-based reasoning**.

---

### Evaluation Criteria
| Criterion | Description |
|:--|:--|
| **Analytical Depth** | Explore, interpret, and visualise telemetry effectively. |
| **Modelling Rigor** | Use sound, reproducible methods supported by quantitative reasoning. |
| **Communication** | Present results with clarity, structure, and good visuals. |

---

### Deliverables
Submit a single **Python notebook (`.ipynb`)** containing:
- Data exploration for Cycles 1–2  
- Modelling and justification
- Predicted `helio_remaining_energy` curve for Cycle 3  
- A single numeric estimate: **End-of-Cycle Energy Reserve**  

> **Good luck, Cadet.**  
> *The Helios-V will sail the void on the strength of your models.*

