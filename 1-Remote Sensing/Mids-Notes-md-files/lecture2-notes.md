# Lecture 2: Electromagnetic Radiation (EMR), Spectrum & Energy Interaction

---

## 1. Introduction

- Remote sensing relies on measuring **Electromagnetic (EM) energy**
- The most important source of EM energy at Earth's surface is **the Sun**
- Interpreting RS imagery requires understanding EM radiation and its interaction with **atmosphere** and **surfaces**

---

## 2. Key Term — Wavelength (λ)

- **Wavelength**: The distance between two successive wave crests
- Units: **Micrometer (µm)** or **Nanometer (nm)**
- 1 µm = 1000 nm

---

## 3. Electromagnetic Spectrum

- Ranges from **shorter wavelengths** (gamma rays, X-rays) to **longer wavelengths** (microwaves, radio waves)
- There are **no natural breaks** — divisions are made for convenience
- Only a **few regions** are useful for remote sensing

### Important Regions:

| Region | Wavelength Range | Notes |
|--------|-----------------|-------|
| **Visible** | 0.38 µm – 0.7 µm | What our eyes can see (Blue, Green, Red) |
| **Reflected / Near IR** | 0.7 µm – 3.0 µm | Solar radiation reflected from Earth; used similarly to visible |
| **Thermal / Emitted IR** | 3.0 µm – 14.0 µm | Heat energy **emitted** by the Earth |

> The visible portion is very **small** relative to the entire EM spectrum.

---

## 4. Interaction with the Atmosphere

EM radiation passing through the atmosphere is modified by three processes:

### 4.1 Scattering

- Occurs when atmospheric **particles or gas molecules** redirect radiation from its original path
- **Atmospheric Path Radiance**: Scattered radiation that reaches the sensor **without ever touching** the Earth's surface (adds unwanted brightness/haze)

#### Factors affecting scattering:
1. **Wavelength** of the radiation
2. **Size and abundance** of suspended particles or gases
3. **Distance** the radiation travels through the atmosphere

#### Three Types of Scattering:

| Type | Particle Size | Wavelengths Affected |
|------|--------------|---------------------|
| **Rayleigh Scattering** | Very small (molecules) | Shorter wavelengths most affected |
| **Mie Scattering** | About equal to wavelength | Longer wavelengths |
| **Nonselective Scattering** | Much larger than wavelength | **All wavelengths** scattered equally |

#### Real-world Examples:
- **Sky appears blue** during the day → Rayleigh scattering (shorter blue wavelengths scattered more)
- **Sunrise/sunset appear red** → Light travels farther through atmosphere, shorter wavelengths scattered away, longer wavelengths (red) penetrate

#### Effects of Scattering on RS Images:
- Creates **skylight** (allows seeing in shadows)
- Image records **brightness of atmosphere** in addition to the target
- **Reduces contrast** → decreases detectability of features

---

### 4.2 Absorption

- Atmospheric molecules **absorb** EM energy at specific wavelengths
- Three main absorbing gases:
  1. **Ozone (O₃)**
  2. **Carbon Dioxide (CO₂)**
  3. **Water Vapour (H₂O)**
- These gases influence **where in the spectrum** we can use for RS

---

### 4.3 Atmospheric Windows

- **Definition**: Regions of the EM spectrum that are **relatively free** from scattering and absorption effects
- Radiation can pass through these windows with **little or no loss**

#### Key Atmospheric Windows:

| Window | Range | Use |
|--------|-------|-----|
| **Optical window** | 0.4 – 2 µm | Optical remote sensors + human eye |
| **Thermal IR window** | ~3 – 5 µm | Thermal sensing |
| **Broad thermal window** | ~8 – 14 µm | Thermal remote sensing |

> RS instruments are designed to operate within these atmospheric windows.

---

### Combined Effect of Scattering + Absorption

- **Add haze** to the image (reduce contrast)
- **Reduce radiation** returning to sensor from Earth's surface
- This is called **attenuation** or **extinction** (weakening of signal)

---

## 5. Interaction with Earth's Surface (EMR and Earth Surface)

Radiation that is **not absorbed or scattered** in the atmosphere reaches the Earth's surface, where **three things happen**:

| Interaction | Meaning |
|-------------|---------|
| **Reflected** | Energy bounces back from the surface |
| **Absorbed** | Energy is taken in by the surface material |
| **Transmitted** | Energy passes through the surface material |

> **The proportions of each depend on:**
> 1. **Wavelength** of the energy
> 2. **Material** type of the feature
> 3. **Condition** of the feature

---

## 6. Types of Reflection

### Specular (Mirror-like) Reflection
- Surface is **smooth** → energy reflected in a **single direction**
- Example: water surface, glasshouse roof
- Creates a **very bright spot** in the image

### Diffuse Reflection
- Surface is **rough** → energy reflected **uniformly in all directions**
- This is the type of reflection most useful for RS

---

## 7. Color of Objects in Remote Sensing Images

> **The color of an object = the color of light it REFLECTS**

### Color Formation Rules (Additive Color Mixing):

| Light Reflected | Color Seen |
|----------------|------------|
| Blue only | **Blue** |
| Green only | **Green** |
| Red only | **Red** |
| Blue + Green + Red | **White** |
| None (all absorbed) | **Black** |
| Green + Red (no Blue) | **Yellow** |
| Blue + Green (no Red) | **Cyan** |
| Blue + Red (no Green) | **Magenta** |

### Why Yellow Appears:
- Object **absorbs Blue** light and **reflects Green + Red** → we see **Yellow**

### Why Magenta Appears:
- Object **absorbs Green** light and **reflects Blue + Red** → we see **Magenta**

---

## 8. Recording of Energy by the Sensor

- After energy has been **reflected, scattered, or emitted** from the target
- A **sensor collects and records** the electromagnetic energy

---

## 9. Radiation Range Useful for Remote Sensing

- RS images are primarily made in the range from **Visible (0.4 µm) to Infrared (14 µm)** and also **Microwave** region
- These are the regions where **atmospheric windows** allow radiation to pass

---

## Key Definitions to Remember

| Term | Definition |
|------|------------|
| **EMR** | Electromagnetic Radiation — energy that travels as waves through space |
| **Atmospheric Path Radiance** | Scattered radiation reaching sensor without touching Earth's surface |
| **Atmospheric Window** | Spectral region relatively free from absorption/scattering |
| **Attenuation / Extinction** | Weakening of signal due to scattering + absorption |
| **Rayleigh Scattering** | Scattering by very small particles — affects shorter wavelengths most |
| **Specular Reflection** | Mirror-like reflection from smooth surfaces |
| **Diffuse Reflection** | Uniform reflection in all directions from rough surfaces |

---
