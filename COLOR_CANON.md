# CPAS Color Canon

This document defines the **normative color semantics** for the Cyber-Physical Aesthetic Stack (CPAS).

Within CPAS, color is not aesthetic.  
Color is a **safety-critical signaling system**.

Any use of color that does not convey operational meaning constitutes non-compliance.

---

## 1. Core Rule

Color SHALL be used only to communicate:

- system state
- safety condition
- operational priority

Color SHALL NOT be used for:
- decoration
- branding
- ambience
- emotional effect
- stylistic differentiation

If removing a color does not change interpretation, that color is prohibited.

---

## 2. Structural Neutrals (Default State)

Structural neutrals SHALL dominate the visual field.

These colors communicate mass, constraint, and infrastructure.

### Permitted Neutral Classes
- industrial gray
- graphite
- brushed or matte metal
- neutral white (illumination only)
- limited matte black (non-dominant)

Structural neutrals SHOULD occupy approximately **85–95%** of visible surfaces.

---

## 3. State Colors (Health and Safety)

State colors communicate **system condition**.

They are mutually exclusive and SHALL NOT overlap.

---

### Green — Nominal / Operational

Indicates:
- normal operation
- safe condition
- no human action required

Green SHALL NOT be persistent if the system is idle.

---

### Amber — Degraded / Warning

Indicates:
- abnormal condition
- degraded performance
- attention required

Amber SHALL resolve or escalate.  
Persistent amber states are prohibited.

---

### Red — Fault / Unsafe

Indicates:
- critical fault
- unsafe condition
- immediate action required

Red SHALL override all other colors in visibility and salience.

---

## 4. Cyber-Presence Color

### Cyan / Blue — Computation Presence

Cyan or blue MAY be used to indicate:
- control plane availability
- cyber-layer activity
- network presence

Constraints:
- Blue SHALL NOT indicate safety or health
- Blue SHALL NOT compete with green, amber, or red
- Blue SHALL be lower in brightness and salience
- Blue SHALL NOT be architectural or ambient

Blue answers:
- “Is the system present?”

Blue does NOT answer:
- “Is the system safe?”

---

## 5. Signal Hierarchy (Mandatory)

Color priority SHALL be enforced in the following order:

1. Red
2. Amber
3. Green
4. Cyan / Blue
5. Structural neutrals

Lower-priority colors SHALL NOT visually dominate higher-priority colors.

Priority inversion constitutes non-compliance.

---

## 6. Spatial Constraints

Color SHALL be spatially constrained.

Permitted locations:
- indicator lights
- control panels
- dashboards
- beacons
- safety markings

Prohibited locations:
- walls
- floors
- ceilings
- structural elements
- ambient lighting

Color bleed into architecture is prohibited.

---

## 7. Temporal Constraints

Color SHALL be temporally meaningful.

Requirements:
- colors appear only while the state exists
- transitions are deterministic and legible
- no color remains active without justification

Color that becomes background noise is non-compliant.

---

## 8. Animation and Motion

Color animation is permitted only for:
- state transition
- escalation or de-escalation

Decorative pulsing, cycling, or motion is prohibited.

---

## 9. Normative Visual References

The following images located in:

    APPENDICES/IMAGES/NORMATIVE/

are **normative references** for this document:

- 01_state_color_transitions.png
- 02_color_reference.png
- 03_spatial_zoning.png
- 04_signal_hierarchy.png

Any configuration substantially similar to those images SHALL be considered compliant or non-compliant accordingly.

---

## Summary

CPAS color usage ensures:

- state is immediately legible
- priority is unambiguous
- safety dominates perception
- decoration is eliminated

If color attracts attention without conveying truth, CPAS has been violated.
