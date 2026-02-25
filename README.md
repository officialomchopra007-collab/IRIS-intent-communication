# IRIS — Intent-Based Communication Under Extreme Bandwidth

> We are doing live human interaction at less bandwidth than a WhatsApp text message.

IRIS proves that **video is the wrong abstraction for communication**.
Humans do not transmit pixels — they transmit **intent**.

## ❌ The Problem

Modern communication systems stream **pixels**.

This works only when:
- Bandwidth is abundant
- Latency is low
- Packets are stable

Under real conditions:
- Video freezes
- Frames drop
- Presence collapses

This is not a network problem.

**This is an abstraction problem.**

## 💡 Core Insight

Humans do not perceive the world frame-by-frame.

We infer:
- Motion continuity
- Expression intent
- Temporal coherence

IRIS transmits **decisions**, not frames.

- Video: 30 images / second
- IRIS: 30 intent decisions / second

## 🧠 System Architecture

**Sender**
- Webcam input
- Face landmark + motion extraction
- Intent vector encoding
- Bandwidth-aware throttling

**Transport**
- ≤ 0.1 kbps intent stream
- Packet drop simulation
- No video frames transmitted

**Receiver**
- Intent reconstruction
- Temporal smoothing
- Presence proxy (avatar / mesh)

## 🔴 Live Demo Capabilities

The demo runs **live**, not replayed.

It supports:
- Real-time head motion
- Expression change
- Sudden, non-scripted actions
- Bandwidth throttling
- Packet loss injection

Observed behavior:
- Video collapses under stress
- IRIS degrades gracefully
- Presence remains stable

## ▶️ How to Run

Install dependencies:
```bash
pip install opencv-python mediapipe numpy matplotlib

Run sender: python demo/camera_sender_intent.py
Run receiver: python demo/camera_receiver_avatar.py
optional: python demo/camera_dual_demo.py

```markdown
## 🚀 Final Note

IRIS does not compress video.

**It removes it.**
