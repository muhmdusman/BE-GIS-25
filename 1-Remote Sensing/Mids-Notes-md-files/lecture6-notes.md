# Lecture 6: Remote Sensing Satellite Orbits and Data Acquisition

---

## 1. What is a Satellite Orbit?

- The **path** followed by a satellite around the Earth
- The orbit is **chosen based on what we want the satellite to observe**
- RS satellite orbits **match the capabilities of their sensors**
- Goal: cover a **large area periodically**

---

## 2. Two Main Types of Orbits

### 2.1 Geostationary (Geosynchronous) Orbit

Think of it as a satellite that **stays still** relative to Earth:

- Satellite **circles Earth at the same speed** Earth spins
- Completes **one revolution in the same time** Earth takes to rotate once (24 hours)
- Moves **West to East** (same direction as Earth)
- Altitude: **~36,000 km** (very high)
- **Always sees the same portion** of Earth → almost full hemisphere view

**Used for:** Meteorological (weather) and communication satellites

> Simple way to remember: "**Geo-STATIONARY** = stays in one place above Earth"

### 2.2 Polar Orbit (Near-Polar)

- Satellite orbits from **pole to pole** (North-South direction)
- Altitude: **about 1000 km or less** (much lower than geostationary)
- As Earth rotates beneath, the satellite covers **different strips** each orbit
- Eventually covers the **entire Earth**

---

## 3. Sun-Synchronous Orbit (Most Common for RS)

- A special type of **near-polar orbit**
- Satellite passes over every point on Earth at the **same local sun time** each day
- This ensures **consistent illumination** in images taken on different days

> Simple way to remember: "**Sun-synchronous** = same sun angle every time it flies over"

### Why Same Illumination Matters:
- Comparing images from **different dates** is easier when lighting is the same
- Makes change detection more reliable

---

## 4. Descending vs Ascending Path

| Path | Direction | Side of Earth | Data Collection? |
|------|-----------|---------------|-----------------|
| **Descending** | North → South | **Sunlit side** (daytime) | YES — sensors collect data here |
| **Ascending** | South → North | **Shadowed side** (nighttime) | Usually NO (no sunlight to reflect) |

> Sensors that need reflected solar light only work during the **descending (daytime) path**.

---

## 5. Best Crossing Time — Why Mid-Morning?

| Crossing Time | Effect | Problem |
|---------------|--------|---------|
| **Early morning** | Low sun angle → good for **topographic features** | Too many **shadows** in hilly areas |
| **Noon** | Maximum & uniform illumination | Sensor **saturation** on bright surfaces, mirror reflection problems |
| **Mid-afternoon** | Moderate illumination | **Solar heating** effect at maximum → difficulties recording reflected energy |
| **Mid-morning** ✓ | Best **compromise** | Balanced illumination, minimal problems |

> Most RS satellites use **mid-morning crossing** time as the best balance.

---

## 6. Key Orbital Terms (Simple Definitions)

| Term | Simple Meaning |
|------|---------------|
| **Equatorial Crossing** | Points where the orbital path crosses the equator |
| **Orbital Inclination** | Angle between satellite track and equator — controls how far North/South it goes |
| **Orbital Period** | Time for one complete orbit — increases with altitude |
| **Altitude** | Height of satellite above Earth |
| **Swath** | The **strip of ground** the sensor can see as it moves — determines scene size |

---

## 7. Swath and Earth Coverage

- As the satellite orbits pole-to-pole, the Earth **rotates beneath it** (West to East)
- So the satellite's swath **shifts westward** with each orbit
- Each new pass covers a **new strip** of ground
- After one complete cycle → **entire Earth's surface** is covered

### Orbit Overlap:
- The **westward shift** between orbits at the equator determines how many orbits needed for full coverage
- **Higher latitudes** get imaged **more frequently** because orbital paths get closer near the poles → more overlap

---

## 8. Orbit Period Formula

$$T = 2\pi(R + H)\sqrt{\frac{R + H}{gR^2}}$$

Where:
- $T$ = Orbit period (time for one orbit)
- $R$ = Radius of Earth ≈ 6380 km
- $H$ = Orbital altitude
- $g$ = Acceleration due to gravity

### Number of Orbits Per Day:

$$N = \frac{T_{earth}}{T_{orbit}}$$

---

## 9. Revisit Period

- The time after which the satellite **revisits the same area** on Earth
- Important for **frequent imaging** needs
- Near the **poles** → revisit is **more frequent** (due to overlapping swaths)
- Near the **equator** → revisit is **less frequent**

---

## Key Definitions to Remember

| Term | Definition |
|------|------------|
| **Geostationary Orbit** | Satellite stays above same point on Earth, ~36,000 km altitude |
| **Polar Orbit** | North-South orbit, ~1000 km, covers entire Earth over time |
| **Sun-Synchronous** | Passes over every point at the same local sun time |
| **Swath** | Strip of ground the sensor sees during one pass |
| **Revisit Period** | Time between two passes over the same location |
| **Descending Path** | North→South on sunlit side — data collection happens here |
| **Orbital Inclination** | Angle of satellite track relative to equator |

---
