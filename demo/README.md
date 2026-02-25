# IRIS — Live Demo Evidence

This folder documents **live, real-time execution** of IRIS under extreme bandwidth constraints.

This is NOT a simulation.

---

## Demo Overview

IRIS replaces video frames with **intent signals**:
- Head pose
- Facial landmarks
- Motion timing
- Expression dynamics

No pixels are transmitted.

---

## What Was Demonstrated Live

### 1. Baseline Failure (VIDEO)
- Network throttled to ≤10 kbps
- Video freezes, jitters, collapses
- Human presence is lost

### 2. IRIS Intent Stream
- Webcam input → intent vectors
- Bandwidth observed: ~0.02–0.12 kbps
- Motion and expression preserved

### 3. Receiver-Only Presence
- No video received
- Avatar / face mesh driven purely by intent
- Smooth recovery under packet loss

### 4. Phase Transition Curve
- Error vs Bandwidth plotted live
- Clear stability → instability → collapse regions
- Intent saturates earlier than pixels

---

## Proof Artifacts (Added Below)

- Screenshots of live runs
- Phase curves
- Jerk stability plots
- Sender / Receiver split view

(All images are real captures from execution, not mockups.)
