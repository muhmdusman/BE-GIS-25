# Lecture 4: Remote Sensing Platforms

---

## 1. What is a Platform?

- A **platform** is the vehicle or carrier of remote sensing sensors
- Three main types:
  1. **Airborne** (aircraft, UAVs/drones)
  2. **Spaceborne** (satellites, space shuttles)
  3. **Ground-based** (ladder trucks, cherry pickers)

---

## 2. Factors for Selection of a Platform

- **Purpose** of the mission
- **Coverage** needed:
  - Less or large area
  - Single or repeated coverage
- **Orbits** (for satellites)
- **Atmospheric conditions** depending on the altitude

---

## 3. Aircraft Platforms

### History:
- First widespread use in **World War I** for military intelligence
- First aerial photograph taken in **1858**
- Kite-based aerial photos in **1888**; pigeons used in **1903**

### Advantages of Aircraft:
1. **Most easily available** RS data
2. **Higher resolution** data
3. Instruments can be **tuned and repaired**
4. Images can be taken at **any solar illumination angle**
5. **Flexible** operation over any desired area at any time

### Advantages of Wider Aircraft over Less Wide Aircraft:
- Wider aircraft can carry **more/larger sensors** (greater payload)
- Cover a **wider swath** in a single pass → more area per flight
- More **stable platform** → less distortion in images
- Can fly longer missions with better fuel capacity

### Limitations of Aircraft:
1. **Obtaining permission** is required
2. **Coordination** of pilot and photographer needed
3. **Smaller area coverage** compared to satellites
4. **Weather dependent**
5. **Higher cost** per area covered
6. Possibility of **systematic distortions** (roll, pitch, yaw)

---

## 4. UAV/Drones

### Advantages:
1. **Quick image acquisition**
2. Operation in **confined areas** (urban)
3. Relatively **very low cost** data
4. **High resolution** images
5. Not limited to lengthy image acquisition **planning and coordination**
6. **Less weather dependency** — can fly below clouds
7. Operational in **hostile environments**
8. Can operate in **emergency situations** (rain, snow, fog, rough terrain)
9. **Safer** than manned aircraft in dangerous conditions

### Limitations:
1. **Obtaining permission** / regulatory challenges (safety, security, privacy)
2. **Very small area coverage**
3. **Less payload** (limited weight capacity)
4. **Low altitude** operation only
5. **Less flight time** / power issues
6. **Weather dependent** (wind, etc.)
7. **Systematic distortions** (roll, pitch, yaw)
8. **Security reasons**

---

## 5. Spacecraft Platforms

### Types:
| Type | Examples |
|------|---------|
| **Manned** | Soviet Cosmonauts, Gemini, Apollo, Space Shuttle |
| **Unmanned** | TIROS-1, LANDSAT, SPOT, Sentinel |

### Advantages of Unmanned Satellites:
1. **No complex life support system** needed
2. **Complete global coverage** (whole Earth)
3. Can operate for **very long periods**
4. **Repeated coverage** of the same area
5. **Large area coverage at lower cost**

### Disadvantages of Unmanned Satellites:
1. Coverage limited to **fixed orbital path**
2. **Fixed repeat cycle** (cannot image on demand)
3. **Atmospheric effects** degrade image quality
4. **Cloud coverage** blocks optical sensors

---

## 6. Mission Classification

| Type | Purpose | Examples |
|------|---------|---------|
| **Earth Resource Imaging** | Imaging Earth's surface | LANDSAT, SPOT, IKONOS |
| **Planetary Missions** | Imaging other celestial objects | Hubble Space Telescope, Apollo |

---

## 7. Roll, Pitch, and Yaw — Platform Distortions (Simple Explanation)

Think of an airplane moving forward. It can rotate in **three ways**, and each causes **distortion** in the image:

| Motion | What Happens | Simple Way to Remember |
|--------|-------------|------------------------|
| **Roll** | Platform **tilts sideways** (left wing goes up, right goes down) | Like a boat rocking side to side |
| **Pitch** | Platform **tilts forward or backward** (nose goes up or down) | Like nodding your head yes |
| **Yaw** | Platform **rotates horizontally** (nose turns left or right) | Like shaking your head no |

```
        Roll             Pitch              Yaw
     \       /         ___/               ___
      \     /         /                  /   \
  ←----✈----→       ✈ nose up/down      ✈ turns left/right
   tilts sideways    tilts front/back    rotates flat
```

> These movements cause the image to **shift, stretch, or rotate** compared to the real ground, creating systematic errors that need correction.

---

## Key Definitions to Remember

| Term | Definition |
|------|------------|
| **Platform** | Vehicle/carrier of remote sensing sensors |
| **Airborne** | Aircraft, helicopters, UAVs — flexible, high-res, limited area |
| **Spaceborne** | Satellites — global coverage, fixed orbit, repeated coverage |
| **UAV/Drone** | Unmanned aerial vehicle — low cost, confined areas, very high resolution |
| **Roll** | Sideways tilt of the platform (left-right rocking) |
| **Pitch** | Forward-backward tilt (nose up or down) |
| **Yaw** | Horizontal rotation (nose turns left or right) |

---
