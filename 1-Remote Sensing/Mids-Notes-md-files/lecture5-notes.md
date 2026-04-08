# Lecture 5: Remote Sensing Sensors and Data Acquisition

---

## 1. Multispectral vs Hyperspectral RS

| Type | Definition |
|------|-----------|
| **Multispectral RS** | Collection of energy from an object in **multiple bands** (few bands, e.g., 3–10) |
| **Hyperspectral RS** | Data collection in **hundreds of bands** (very detailed spectral info) |

---

## 2. Remote Sensors — Types

- **Remote Sensors** = Detection and recording instruments for RS
- Two broad sensor categories:
  1. **Photographic cameras** (Analog and Digital)
  2. **Electro-Mechanical Scanners**

### Two Main System Types:

| System | How It Works |
|--------|-------------|
| **Framing Systems** | Captures the entire scene at once (like a camera) |
| **Scanning Systems** | Builds the image line by line |

---

## 3. Scan Line

- A **scan line** = one horizontal row of pixels in an image
- Collected either:
  - **Sequentially** — sensor moves left to right (**Whisk Broom**)
  - **Simultaneously** — using a linear array of detectors (**Push Broom**)

---

## 4. Understanding Along-Track vs Across-Track (Simple Explanation)

Before learning scanner types, understand these two directions:

- **Along-Track** = **parallel** to flight path = the **forward direction** the satellite/aircraft moves
- **Across-Track** = **perpendicular** to flight path = the **left-right sideways** direction

```
Direction of Flight →→→→→→
     ________________________
     |  |  |  |  |  |  |  |   ← Across-Track (perpendicular)
     |  |  |  |  |  |  |  |      Whisk broom sweeps this way
     |  |  |  |  |  |  |  |
     ↑
Along-Track (parallel)
Push broom captures this way
```

---

## 5. Multispectral Scanner (MSS)

- A scanning system that collects data over **different wavelength ranges**
- Two main acquisition technologies:

### 5.1 Whisk Broom (Across Track) — Simple Explanation

Imagine a **mirror swinging left-to-right** like a pendulum under the aircraft:

- The mirror **sweeps sideways** (across track = perpendicular to flight path)
- It captures **one pixel at a time** as it swings
- After one sweep, the aircraft moves forward and it sweeps again
- Like **reading one letter at a time** across a page
- **Point Geometry** — sees only a single point at any instant

**How it works technically:**
- Oscillating mirror redirects EMR into detectors
- EMR is split into wavelengths via mirrors and prisms
- Each detector records brightness for one point

### 5.2 Push Broom (Along Track) — Simple Explanation

Imagine a **long row of tiny cameras** lined up sideways under the aircraft:

- Thousands of **CCD detectors** sit in a line across the flight path
- They capture an **entire row of pixels at once** (like a scanner)
- As the aircraft moves forward, each new position = new row
- Like **photocopying one full line at a time**
- **Line Geometry** — captures a complete scan line at any instant

**How it works technically:**
- Charged Couple Devices (CCDs) aligned perpendicular to flight
- Each CCD aimed at a specific ground point
- All pixels in one line recorded simultaneously

### Comparison:

| Feature | Whisk Broom | Push Broom |
|---------|-------------|------------|
| **Also called** | Across-Track scanner | Along-Track scanner |
| **Mechanism** | Oscillating mirror (swings sideways) | Linear CCD array (row of detectors) |
| **How it captures** | One pixel at a time (point) | Entire line at once (line) |
| **Simple analogy** | Reading one letter at a time | Scanning one full line at a time |
| **Speed** | Slower | Faster |
| **Geometry** | Point Geometry | Line Geometry |

---

## 5. Airborne Digital Cameras (Examples)

| Camera | Key Features |
|--------|-------------|
| **Leica ADS-40/80** | 4 bands (RGB + NIR), forward/nadir/aft arrays |
| **RedEdge MicaSense** | 8 cm/pixel, 5 narrow bands, 12 bit, 168 g |
| **Parrot Sequoia** | 13 cm/pixel, 4 bands (G, R, RedEdge, NIR), 12 bit, 107 g |
| **Altum MicaSense** | 4 cm/pixel, 5 bands + Thermal IR (8–14 µm), 16 bit, 406 g |
| **OCI Hyperspectral** | 120 bands, 460–970 nm, push-broom, 272 g |

---

## 6. Dwell Time

- **Dwell Time** = The time the Instantaneous Field of View (IFOV) "sees" a ground area
- Generally **very short**
- Influences the design of **spatial, spectral, and radiometric** resolutions

---

## 7. Trade-offs Between Resolutions

This is a critical concept — the three resolutions are **interdependent**:

| If You Want... | What Happens |
|---------------|-------------|
| **High spatial resolution** | Small IFOV → less energy detected → **reduced radiometric resolution** |
| **Better radiometric resolution** (without losing spatial) | Must broaden wavelength range → **reduced spectral resolution** |
| **Coarser spatial resolution** | Allows **improved radiometric and/or spectral** resolution |

### Direct vs Inverse Relationships:

| Pair | Relationship | Explanation |
|------|-------------|-------------|
| Spatial ↔ Radiometric | **Inverse** | ↑ Spatial (smaller pixel) → ↓ Radiometric (less energy per pixel → fewer brightness levels detectable) |
| Spatial ↔ Spectral | **Inverse** | ↑ Spatial (smaller pixel) → ↓ Spectral (must use wider bands to collect enough energy) |
| Spectral ↔ Radiometric | **Inverse** | ↑ Spectral (narrower bands) → ↓ Radiometric (each narrow band gets less energy → fewer brightness levels) |

> **All three pairs are INVERSELY related.** Improving one forces a compromise on the others because a smaller IFOV or narrower band captures **less total energy**, reducing the sensor's ability to distinguish fine brightness differences.

### Simple Memory Trick:
```
Spatial ↑  →  Radiometric ↓  →  Spectral ↓
   (all three fight over the same limited energy)
```

> Think of it as a **fixed energy budget**: a smaller pixel (high spatial) with a narrow band (high spectral) gets very little energy — so it can't distinguish many brightness levels (low radiometric). To fix one, you must sacrifice another.

---

## 8. Data Transmission

### From Aircraft:
- Data is **retrieved when aircraft lands**, then processed and delivered

### From Satellite:
Three methods:
1. **Direct Transmission** — if satellite and ground station are in **line of sight**
2. **On-board Recording** — data recorded on board and **transmitted later**
3. **Relay via TDRSS** — data relayed through **Tracking and Data Relay Satellite System** (communications satellites in **geosynchronous orbit**), satellite-to-satellite until reaching the ground station

---

## Key Definitions to Remember

| Term | Definition |
|------|------------|
| **Multispectral** | Sensing in multiple (few) wavelength bands |
| **Hyperspectral** | Sensing in hundreds of wavelength bands |
| **Whisk Broom** | Across-track scanner using oscillating mirror (point geometry) |
| **Push Broom** | Along-track scanner using linear CCD array (line geometry) |
| **Scan Line** | One horizontal row of pixels in an image |
| **Dwell Time** | Time the IFOV views a ground area |
| **IFOV** | Instantaneous Field of View — ground area seen by sensor at one instant |
| **TDRSS** | Tracking and Data Relay Satellite System for data transmission |
| **CCD** | Charged Couple Device — detector used in push broom scanners |

---
