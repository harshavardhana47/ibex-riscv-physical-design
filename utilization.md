# Core Utilization

## 1. What is Core Utilization?

Core utilization is the percentage of the available core area occupied by the design cells.

It indicates how densely the standard cells and other placed objects are packed inside the core.

### Formula

**Core Utilization (%) = (Occupied Cell Area / Core Area) × 100**

---

## 2. Why is Utilization Important?

Utilization has a direct impact on placement, routing, timing, and congestion.

* **Very high utilization** → less available whitespace, higher congestion, difficult routing, and less flexibility for optimization.
* **Very low utilization** → more whitespace, easier routing and optimization, but larger chip/core area.
* **Balanced utilization** → provides enough space for placement, routing, buffering, clock tree synthesis, and timing optimization.

Therefore, utilization is an important floorplanning parameter.

---

## 3. Utilization Used in This Project

For the Ibex RISC-V core implemented using the SKY130HD technology, the initial target utilization is:

**CORE_UTILIZATION = 50%**

This means the initial floorplan is designed with approximately 50% of the available core area intended to be occupied by the design cells, leaving the remaining area as whitespace for physical implementation.

---

## 4. Why 50%?

A relatively moderate utilization is selected for the initial floorplan to provide sufficient whitespace for:

* Standard-cell placement
* Routing
* Buffer and inverter insertion
* Clock Tree Synthesis (CTS)
* Timing optimization
* Congestion reduction
* Physical-only cells and other implementation requirements

The actual optimum utilization may need to be adjusted based on placement congestion, timing, and routing results.

---

## 5. ORFS Configuration

The utilization is specified in the design configuration using:

CORE_UTILIZATION = 50

This parameter is used by the OpenROAD-flow-scripts flow during floorplan generation.

---

## 6. Expected Trade-off

| Utilization | General Effect                                                    |
| ----------- | ----------------------------------------------------------------- |
| Low         | Larger core area, more whitespace, easier placement/routing       |
| Moderate    | Balanced area and routability                                     |
| High        | Smaller core area but increased congestion and routing difficulty |

The objective is not simply to maximize utilization. The goal is to achieve a floorplan that provides a good balance between **area, timing, congestion, power, and routability**.

---

## 7. Project Result

### Initial Target

**50%**

### Actual Result

Added in future stages

### Congestion Observation

Added in future stages

### Timing Observation

Added in future stages

---

## 8. Evidence

The following project evidence will be added:

Added in future stages
