# Gesture Layer

Documentation for the finger-worn capacitive tap sensor interface — the physical dimension of the cellular calendar.

## Vision

The gesture layer transforms the cellular calendar from a screen-based tool into an **embodied practice**. Rather than pointing and clicking, the body becomes the navigator of temporal space.

Finger-worn capacitive sensors detect deliberate tap gestures and translate them into interactions with the calendar — creating, connecting, navigating cells through physical intention rather than passive mouse movement.

## Design Principles

**Deliberate over ambient**
Every gesture is a conscious act. The sensors don't monitor your hands continuously — they respond to intentional tap sequences. This mirrors the calendar's own philosophy: temporal containers defined by intention, not by automatic tracking.

**State tracking through touch**
Different tap patterns map to different states:
- single tap — select / enter a cell
- double tap — create new cell
- hold — open editor
- two-finger tap — connect mode
- (patterns evolving through use)

**Somatic coherence**
The physical gesture and the temporal intention become linked. Tapping to enter a week-long cell has a different quality than tapping into a year. The body learns the landscape.

## Hardware

- **Sensors:** Finger-worn capacitive sensors (currently in fabrication)
- **Form factor:** Ring or thimble-style, non-intrusive
- **Connection:** [TBD — wired / wireless / BLE]
- **Fingers:** [TBD — which fingers map to which gestures]

## Current Status

⚙ Hardware in fabrication

## Software Architecture (Planned)

```
Sensor Input
    ↓
Gesture Recognition (tap pattern → state)
    ↓
State Machine (current context → valid actions)
    ↓
Calendar API (translate state to cell interaction)
    ↓
Visual Response (cell responds to gesture)
```

## Gesture Vocabulary (Evolving)

This section will grow as hardware testing informs what gestures feel natural and distinct.

| Gesture | Action | Notes |
|---------|--------|-------|
| Single tap | Select cell | |
| Double tap | New cell | |
| Hold | Open editor | |
| Two-finger tap | Connect mode | |
| Swipe | Navigate space | |

## Integration Points

The gesture layer will interface with `index.html` through:
- A small JavaScript bridge that receives sensor events
- Mapping sensor states to existing calendar interactions
- Eventually: gestures that have no mouse equivalent (e.g., squeeze to merge cells)

## Questions Being Held

- What is the minimum viable gesture vocabulary?
- How does latency affect the felt quality of interaction?
- Can gesture patterns themselves carry meaning beyond function?
- What happens when gesture and intention are misaligned?

## Development Log

*Entries added as fabrication and testing progresses*

---

*This document is living. Update it as the hardware teaches you what it wants to be.*
