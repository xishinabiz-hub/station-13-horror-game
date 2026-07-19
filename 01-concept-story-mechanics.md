# 🚇 STATION 13 — PART 1: CONCEPT, STORY & PLAYER MECHANICS

---

## 1. GAME CONCEPT

**SUBWAY STATION 13** — First-person anomaly-detection horror. You're the night-shift attendant at an abandoned underground metro station. Passengers keep arriving — but the last train was canceled 3 years ago. Some passengers are human. Some are NOT. Serve the real ones. Detect the anomalies. Survive until 6 AM.

**Gameplay Style (like Animal Hospital / Scary Shawarma):** Shift-based service job. Customers (passengers) arrive at your booth. Use CCTV cameras, a photo camera, ticket inspection, and careful observation to spot anomalies. Reject anomalies with the RED SHUTTER BUTTON. Survive random HAZARD events.

## 2. FULL STORY

**3 Years Ago:** Station 13 — deepest station on Metro Line 7, 200m underground. Drilling crew breached an uncharted cavern containing a smooth BLACK MONOLITH (4m tall, unknown material, glowing symbols). Within 48h: passengers saw "doubles" of themselves. A train arrived with 40 passengers — doors opened to an EMPTY train. Workers heard their own voices calling from tunnels. Monolith emitted EMP. Station sealed. Officially "does not exist."

**Present Day:** You're a new METRO-CORP hire assigned to night security at an unnamed station. Follow THE RULES posted in the control booth:

1. Greet every passenger. Look them in the eyes. Check their ticket.
2. If something feels wrong, check the CCTV. Cameras see what you cannot.
3. NO REFLECTION in booth glass → CLOSE SHUTTER IMMEDIATELY.
4. Never enter tunnels alone. Take flashlight + keep booth door open.
5. Lights flicker 3× in a row → HIDE UNDER DESK for 30s. Don't move.
6. Last train left 3 years ago. If you HEAR a train arriving → DON'T LOOK.
7. Survive until 6:00 AM. Morning crew will relieve you. Probably.

**Ending (Shift 15):** 6:00 AM. PA: "Shift complete." Surface door opens. YOUR DOPPELGANGER stands there. "Good work. I'll take the next shift." Doppelganger walks past you into station. Camera sinks through floor → MONOLITH deep below, dozens of player duplicates circling it. Screen white. "Station 13 awaits its next attendant."

## 3. CORE GAMEPLAY LOOP

```
SHIFT START → Passenger arrives (every 45-90s) → Greet → Check ticket →
Take photo → Check CCTV while photo develops → Compare: normal or anomaly? →
APPROVE (green stamp) or REJECT (red button → shutter SLAM) →
[Hazard interrupts randomly] → Next passenger → SHIFT END (6:00 AM) →
Results → Shop → Next Shift
```

- 1 Shift = 8 minutes real time (12 in-game hours: 6PM→6AM)
- 5-12 passengers/shift, 1-5 are anomalies (scales with difficulty)
- 2-5 random Hazard events per shift
- **WIN:** Survive to 6AM. **LOSE:** Sanity reaches 0% → black out.

**Mistakes:** Miss anomaly = -25% sanity. False reject (normal passenger) = -10%. Fail Rule 5 = -40%. Look at Ghost Train = -30%.

## 4. PLAYER CHARACTER

| Param | Value |
|-------|-------|
| Camera | 5.5 studs, FOV 75 |
| Walk/Sprint | 14/20 studs/s (Shift, 3s, 2s cooldown) |
| Jump | DISABLED |
| Crouch | Ctrl, 3.5 studs |
| Head Bob | Gentle sine 0.15 |

**Controls:** WASD move, Mouse look, LMB interact, RMB photo/taser, E interact/pickup, F flashlight, Shift sprint, Ctrl crouch, TAB CCTV tablet, M map, B shop (between shifts)

## 5. INTERACTION SYSTEMS

### 5.1 Ticket Booth
- Glass window 6×4 studs (tinted, bulletproof), ticket slot at bottom
- RED ROLLING SHUTTER above window (slams in 0.5s)
- Interior counter: Rubber stamp + ink pad, Polaroid camera, blank tickets
- RED MUSHROOM EMERGENCY BUTTON under counter (backlit red)
- Swivel stool, clip-on fan, METRO-CORP mug
- Note taped inside: "No reflection → SHUTTER. No hesitation."

### 5.2 CCTV Tablet (TAB key)
- 6 live ViewportFrame feeds: Platform N, Platform S, Ticket Hall, Tunnel, Stairwell, Control Booth
- Scroll = zoom, Space = freeze frame, RMB on tablet = night vision (green tint)
- Battery drains ~0.5%/s (~3 min continuous). Recharge at dock in booth (15s).
- **What CCTV reveals (naked eye doesn't):** Elongated limbs, missing faces, extra passengers, glowing eyes, camera-staring, glitched body parts, attached shadow entities.

### 5.3 Photo System
- RMB at booth → camera flash → Polaroid prints → develops over 3s (black→image)
- Anomalies appear differently on film. Hold RMB to examine close. Auto-discard 10s. Max 3.

### 5.4 Flashlight
- Default ON (30° cone, 35 studs, warm yellow). F toggles. UNLIMITED battery. Flickers at low sanity.

### 5.5 Coffee & Vending
- Coffee: Free, 3 sips/pot, +15% sanity each. 8s brew, 90s cooldown after 3 pots.
- Vending: Energy Bar +10%/50🪙, Chips +8%/35🪙, Soda +12%+speed/75🪙

## 6. SANITY SYSTEM

| Event | Change |
|-------|--------|
| Looking at Hazard | -2%/s |
| Miss anomaly | -25% |
| False reject | -10% |
| Jump scare | -5% |
| Dark >10s | -1%/s |
| Ghost train (no hide) | -15% |
| Look at ghost train | -30% |
| **Recovery:** Coffee +15%, Detect anomaly +5%, Serve normal +2%, Sit in booth +1%/2s, Snacks +8-12% |

**Visual feedback:** 100-70% normal → 70-40% vignette+desaturation → 40-20% heavy vignette+warp+cold blue → 20-5% breathing+pulses+false shadows → 0% black+faint.

## 7. SHIFT PROGRESSION

| Shift | Passengers | Anomalies | Special |
|-------|-----------|-----------|---------|
| 1 | 5 | 1 | Tutorial (no death) |
| 2 | 5-6 | 1-2 | Real start |
| 3 | 6-7 | 1-2 | +H-01 Flesh Ceiling |
| 4 | 6-8 | 1-3 | Taser unlocked |
| 5 | 7-9 | 2-3 | +PA, Door Knocker |
| 6 | 8-10 | 2-3 | +Weeping Woman |
| 7-8 | 8-11 | 2-4 | +Shadow, Ghost Train |
| 9 | 9-12 | 3-4 | P-20 The Child |
| 10 | 10-12 | 3-5 | BOSS (+Blackout) |
| 11-14 | 10-12 | 3-5 | Nightmare |
| 15 | 12 | 5 | FINAL → Ending |

**Rewards:** Base 200🪙+100XP, perfect +100🪙+50XP, no false +60🪙+30XP, no blackout +40🪙+20XP. Max 400🪙/200XP. Fail: 50🪙/25XP.

---

# ⏭️ 02-map-layout.md — Complete station map with every room
