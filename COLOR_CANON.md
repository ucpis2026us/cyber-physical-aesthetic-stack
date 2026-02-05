# CPAS Color Canon

This document defines the normative color semantics for the Cyber-Physical Aesthetic Stack (CPAS).

Color in CPAS is not aesthetic.  
It is a signaling mechanism used to communicate system state, priority, and safety.

Any use of color that does not encode operational meaning is non-compliant.

---

## 1. Core Rule

Color SHALL be used only to communicate system state, priority, or safety-relevant information.

Color SHALL NOT be used for:
- decoration
- branding
- ambience
- emotional framing
- stylistic differentiation

If color does not change interpretation, it SHALL NOT exist.

---

## 2. Structural Neutrals (Default)

Structural neutrals comprise the majority of the visual field in CPAS-compliant systems.

### Allowed Neutral Colors
- graphite
- industrial gray
- brushed metal
- matte black (limited use)
- neutral white (illumination only)

### Purpose
- communicate mass and constraint
- minimize perceptual noise
- provide contrast for signal colors

Structural neutrals SHOULD occupy approximately 85–95% of visible surfaces.

---

## 3. State Colors (Health and Safety)

State colors communicate system health and safety status.  
They are mutually exclusive and SHALL NOT overlap.

### Green — Nominal / Operational
Indicates:
- normal operation
- safe, expected behavior
- no action required

Green SHALL NOT be persistent if operation is not active.

---

### Amber — Degraded / Warning
Indicates:
- degraded performance
- abnormal condition
- attention required, but not immediate danger

Amber SHALL escalate or resolve.  
Persistent amber states are prohibited.

---

### Red — Fault / Unsafe
Indicates:
- critical fault
- unsafe condition
- immediate action required
- system halted or entering safe state

Red SHALL override all other colors in visibility and priority.

---

## 4. Cyber-Presence Color

### Cyan / Blue — Computation / Control Presence

Cyan or blue MAY be used to indicate:
- active computation
- control plane availability
- network or cyber-layer presence

### Constraints
- Blue SHALL NOT indicate health or safety state
- Blue SHALL NOT compete with green, amber, or red
- Blue SHALL be lower in brightness and salience than state colors
- Blue SHALL NOT be ambient or architectural

Blue answers the question:
> “Is the system present?”

It does not answer:
> “Is the system safe?”

---

## 5. Signal Hierarchy (Mandatory)

Color priority SHALL be enforced as follows:

1. Red — highest priority
2. Amber
3. Green
4. Cyan / Blue
5. Structural neutrals

Lower-priority colors SHALL NOT visually dominate higher-priority colors.

Priority inversion constitutes non-compliance.

---

## 6. Spatial Constraints

Color SHALL be spatially constrained.

### Allowed Locations
- indicator lights
- control panels
- dashboards
- beacons
- safety markings

### Prohibited Locations
- walls
- floors
- ceilings
- structural elements
- ambient lighting

Color bleed into architectural surfaces is prohibited.

---

## 7. Temporal Constraints

Color SHALL be temporally meaningful.

### Requirements
- State colors SHALL appear only when the corresponding state exists
- Transitions SHALL be clear and deterministic
- No color SHALL remain active without justification

Color that becomes background noise is non-compliant.

---

## 8. Motion and Animation Constraints

Color animation is permitted only when:
- a state transition occurs
- escalation or de-escalation is occurring

Pulsing, cycling, or decorative animation is prohibited.

---

## 9. Normative Visual References

The following images are normative references defining CPAS color usage:

1. State-Transition Strip (Temporal Use)
2. Spatial Zoning Diagram (Architectural Use)
3. Signal Hierarchy Stack (Priority & Salience)
4. Compliant vs Non-Compliant Comparison
5. Visual Hazard Scenarios (Non-Compliant)

These images define acceptable bounds of interpretation.

---

## Summary

CPAS color usage enforces a single outcome:

- state is immediately legible
- priority is unambiguous
- safety signals dominate perception
- decoration is eliminated

If color attracts attention without conveying truth, CPAS has been violated.
