# CPAS Sound Signals

This document defines the normative use of sound within the Cyber-Physical Aesthetic Stack (CPAS).

Sound in CPAS is a safety-critical signaling mechanism.  
It is not an interface, personality channel, or experiential layer.

---

## 1. Core Rule

Normal operation SHALL be silent.

Sound SHALL be used only to communicate safety-critical or time-sensitive state changes that require immediate human attention.

Any sound that does not convey urgency or safety information is non-compliant.

---

## 2. Sound Classes (Permitted)

### 2.1 Emergency / Fault Alarm (Highest Priority)

Emergency alarms indicate unsafe or critical conditions requiring immediate response.

#### Examples
- safety interlock breach
- human-in-danger condition
- critical system fault
- evacuation or exclusion-zone violation

#### Requirements
- non-verbal
- non-melodic
- unmistakable
- directionally local where possible
- continuous or repeating until the condition clears or is acknowledged by a safety system
- SHALL correspond to a RED visual state

Emergency alarms SHALL override all other sounds.

---

### 2.2 Warning Tone (Limited Use)

Warning tones indicate degraded or abnormal conditions that may escalate.

#### Examples
- degraded performance
- pending shutdown
- maintenance threshold exceeded

#### Requirements
- non-verbal
- short duration where possible
- lower urgency than emergency alarms
- SHALL correspond to an AMBER visual state
- SHALL escalate or resolve

Persistent warning tones without escalation or resolution are prohibited.

---

## 3. Prohibited Sound

### 3.1 Voice Output (Prohibited)

CPAS-compliant systems SHALL NOT:
- speak
- use text-to-speech
- narrate system state
- address humans verbally

Language introduces interpretation and delay.  
CPAS relies on trained signals, not conversation.

---

### 3.2 Conversational or Feedback Sounds (Prohibited)

The following are prohibited:
- confirmation chimes
- success tones
- button beeps
- “acknowledged” sounds
- interaction feedback designed for reassurance or delight

Visual confirmation is sufficient.

---

### 3.3 Ambient or Atmospheric Sound (Prohibited)

CPAS-compliant systems SHALL NOT emit:
- background hums
- drones
- musical tones
- “AI presence” audio
- environmental sound design unrelated to safety

If a system is audible during nominal operation, it is non-compliant.

---

## 4. Visual–Auditory Coupling (Mandatory)

Sound SHALL reinforce visual state.

### Requirements
- sound SHALL NOT contradict visual signaling
- emergency alarms SHALL NOT occur during GREEN nominal state
- warning tones SHALL NOT occur without an AMBER visual indicator
- escalation from AMBER to RED SHALL escalate sound priority accordingly

Any mismatch between sound and visual state constitutes non-compliance.

---

## 5. Alarm Fatigue Avoidance

Sound design SHALL minimize unnecessary repetition.

Designs that train operators to ignore sound signals are non-compliant.

Silence is the default and desired state.

---

## Summary

CPAS sound usage enforces the following outcome:

- silence is normal
- sound signals urgency, not personality
- alarms are rare, clear, and truthful
- no system appears conversational or alive

If a system needs to speak, CPAS has already failed.
