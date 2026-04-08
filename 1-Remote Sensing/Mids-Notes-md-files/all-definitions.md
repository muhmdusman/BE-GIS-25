# All Definitions — Remote Sensing (Lectures 1–11)

> Quick-reference glossary for exam prep. Organized alphabetically within categories.

---

## A. Core Remote Sensing Terms

| Term | Definition | Lecture |
|------|-----------|---------|
| **Remote Sensing (RS)** | Acquiring information about an object **without physical contact** | L1 |
| **Remote** | Not in contact with / away from the target | L1 |
| **Sensing** | The act of observation | L1 |
| **Remote Sensor** | Detection and recording instrument **not in contact** with the target | L1 |
| **Scene** | Earth's surface + Atmosphere (what the sensor sees) | L1 |
| **Platform** | Vehicle or carrier of remote sensing sensors (aircraft, satellite, drone) | L4 |
| **Data** | Raw representation that can be operated upon | L1 |
| **Information** | Interpreted / processed data (data + meaning) | L1 |
| **Geospatial Data** | Data with a spatial (location) component | L1 |
| **Earth Resource Information** | Info about vegetation, soils, minerals, rocks, water, atmosphere, urban areas | L1 |

---

## B. The 4 M's of Remote Sensing

| Term | Definition | Lecture |
|------|-----------|---------|
| **Mapping** | Collecting thematic and quantitative baseline data | L1 |
| **Measuring** | More rigorous mapping — quantifying and documenting attributes | L1 |
| **Modelling** | Describing a system through precise mathematical relations to simulate behavior | L1 |
| **Monitoring** | Regular assessment by recording changes in natural phenomena and human activities | L1 |

---

## C. Electromagnetic Radiation (EMR)

| Term | Definition | Lecture |
|------|-----------|---------|
| **EMR** | Electromagnetic Radiation — energy that travels as waves through space | L2 |
| **Wavelength (λ)** | Distance between two successive wave crests | L2 |
| **Electromagnetic Spectrum** | Full range from gamma rays (short λ) to radio waves (long λ) | L2 |
| **Visible Light** | 0.38–0.7 µm — what our eyes can see (Blue, Green, Red) | L2 |
| **Near Infrared (NIR)** | 0.7–3.0 µm — solar radiation reflected from Earth; strongly reflected by healthy vegetation | L2, L9 |
| **Thermal / Emitted IR** | 3.0–14.0 µm — heat energy **emitted** by the Earth | L2 |
| **SWIR** | Shortwave Infrared — between NIR and thermal IR | L2, L9 |

---

## D. Atmospheric Interactions

| Term | Definition | Lecture |
|------|-----------|---------|
| **Scattering** | Atmospheric particles or gas molecules **redirect** radiation from its path | L2 |
| **Rayleigh Scattering** | By very small particles — affects **shorter wavelengths** most (why sky is blue) | L2 |
| **Mie Scattering** | By particles about equal to wavelength — affects **longer wavelengths** | L2 |
| **Nonselective Scattering** | By particles much larger than wavelength — **all wavelengths** scattered equally (why clouds are white) | L2 |
| **Absorption** | Atmospheric molecules **absorb** EM energy at specific wavelengths | L2 |
| **Absorbing Gases** | Ozone (O₃), Carbon Dioxide (CO₂), Water Vapour (H₂O) | L2 |
| **Atmospheric Window** | Spectral region relatively free from absorption/scattering — sensors can "see through" | L2 |
| **Atmospheric Path Radiance** | Scattered radiation reaching sensor **without touching** Earth's surface (noise) | L2 |
| **Attenuation / Extinction** | Weakening of signal due to scattering + absorption combined | L2 |

---

## E. Surface Interactions

| Term | Definition | Lecture |
|------|-----------|---------|
| **Reflected** | Energy bounces back from the surface | L2 |
| **Absorbed** | Energy is taken in by the surface material | L2 |
| **Transmitted** | Energy passes through the surface material | L2 |
| **Specular Reflection** | Mirror-like reflection from **smooth** surfaces | L2 |
| **Diffuse Reflection** | Uniform reflection in **all directions** from rough surfaces | L2 |

---

## F. The Four Resolutions

| Term | Definition | Lecture |
|------|-----------|---------|
| **Resolution** | Ability of a sensor to render a sharply defined image; smallest detectable difference | L3 |
| **Spatial Resolution** | Size of the ground area represented by **one pixel** — how small an object you can see | L3 |
| **Spectral Resolution** | Number and **width of wavelength bands** a sensor records — how finely it splits the spectrum | L3 |
| **Radiometric Resolution** | Number of **brightness levels** a sensor can distinguish (e.g., 8-bit = 256 levels) | L3 |
| **Temporal Resolution** | How **often** a sensor revisits and images the same area | L3 |

### Spatial Resolution Categories

| Category | Pixel Size |
|----------|-----------|
| Very High | < 1 m (sub-meter) |
| High/Fine | 1–4 m |
| Medium | 4–30 m |
| Coarse/Low | > 30 m to > 1000 m |

### Radiometric Resolution — Bit Depth

| Bits | Levels (2ⁿ) | Range |
|------|-------------|-------|
| 1-bit | 2 | Black or white |
| 2-bit | 4 | 4 shades |
| 8-bit | 256 | 0–255 |
| 16-bit | 65,536 | 0–65,535 |

---

## G. Pixel & Image Basics

| Term | Definition | Lecture |
|------|-----------|---------|
| **Pixel** | Smallest element of a digital image — has spatial and spectral properties | L3 |
| **DN (Digital Number)** | The brightness value stored in a pixel | L3 |
| **Aspect Ratio** | Ratio of pixel dimensions; = 1 means pixel is square | L3 |
| **Map Scale** | Ratio of map distance to actual ground distance (1:5,000 = large scale, more detail; 1:100,000 = small scale, less detail) | L3 |
| **Panchromatic** | Single-band image — shows as grayscale | L3 |
| **Multispectral** | Image with 3+ bands — shows as color (e.g., RGB) | L3, L5 |
| **Hyperspectral** | Image with **hundreds** of very narrow bands — extremely detailed spectral info | L5 |

---

## H. Platforms

| Term | Definition | Lecture |
|------|-----------|---------|
| **Airborne Platform** | Aircraft, helicopters, UAVs — flexible, high-res, limited coverage area | L4 |
| **Spaceborne Platform** | Satellites — global coverage, fixed orbit, repeated revisits | L4 |
| **UAV / Drone** | Unmanned Aerial Vehicle — low cost, confined areas, very high resolution | L4 |
| **Ground-based Platform** | Ladder trucks, cherry pickers — closest to target | L4 |
| **Roll** | Platform **tilts sideways** (left-right rocking, like a boat) | L4 |
| **Pitch** | Platform **tilts forward/backward** (nose up or down) | L4 |
| **Yaw** | Platform **rotates horizontally** (nose turns left or right, like a compass) | L4 |

---

## I. Sensors & Scanning

| Term | Definition | Lecture |
|------|-----------|---------|
| **Framing System** | Captures the **entire scene at once** (like a camera click) | L5 |
| **Scanning System** | Builds the image **line by line** | L5 |
| **Along-Track** | Direction **parallel** to the flight path (forward direction) | L5 |
| **Across-Track** | Direction **perpendicular** to the flight path (sideways, left-right) | L5 |
| **Whisk Broom Scanner** | **Across-track** scanner — oscillating mirror sweeps sideways, captures **one pixel at a time** (point geometry) | L5 |
| **Push Broom Scanner** | **Along-track** scanner — linear CCD array captures an **entire row at once** (line geometry) | L5 |
| **IFOV** | Instantaneous Field of View — the ground area "seen" by the sensor at any one instant | L5 |
| **Scan Line** | One horizontal row of pixels in an image | L5 |
| **Dwell Time** | Time the IFOV spends viewing a single ground area — longer = more energy collected | L5 |
| **CCD** | Charged Couple Device — electronic detector used in push broom scanners | L5 |
| **Point Geometry** | Whisk broom — sensor sees only a **single point** at any instant | L5 |
| **Line Geometry** | Push broom — sensor captures a **complete line** at any instant | L5 |
| **Resolution Trade-off** | Improving one resolution (spatial/spectral/radiometric) often **degrades** another | L5 |

---

## J. Satellite Orbits

| Term | Definition | Lecture |
|------|-----------|---------|
| **Geostationary Orbit** | ~36,000 km altitude — satellite matches Earth's rotation, stays **fixed** over one point (weather monitoring) | L6 |
| **Polar Orbit** | ~700–1,000 km — satellite orbits pole to pole (north-south), covers whole Earth over time | L6 |
| **Sun-Synchronous Orbit** | Special polar orbit — passes over every point at the **same local sun time** each revisit (consistent lighting) | L6 |
| **Descending Path** | North → South (daytime, sunlit side) — **data collection happens here** | L6 |
| **Ascending Path** | South → North (nighttime, shadowed side) — usually no imaging | L6 |
| **Swath / Swath Width** | The strip of ground the sensor images in one pass — wider swath = more coverage | L6 |
| **Revisit Period** | Time for satellite to return and image the **same area** again (e.g., Landsat = 16 days) | L6 |
| **Orbital Period** | Time for one complete orbit around Earth — increases with altitude | L6 |
| **Orbital Inclination** | Angle of satellite track relative to equator — controls how far N/S it goes | L6 |
| **Mid-morning Crossing** | ~10:00–10:30 AM — best compromise between good sunlight and minimal clouds/shadows | L6 |
| **TDRSS** | Tracking and Data Relay Satellite System — relays data from sensor satellite to ground station | L5 |

---

## K. Data Formats & Storage

| Term | Definition | Lecture |
|------|-----------|---------|
| **Digital Image** | A numerical record of brightness leaving each pixel in each band | L7 |
| **BIP** | Band Interleaved by **Pixel** — all bands of **one pixel** stored together, then next pixel | L7 |
| **BIL** | Band Interleaved by **Line** — all bands of **one line** stored together, then next line | L7 |
| **BSQ** | Band **Sequential** — entire image for **one band** at a time | L7 |
| **Raster** | Grid/matrix of pixels — how RS images are stored | L7 |
| **Unsigned Integer** | Only positive values (0 and up) | L7 |
| **Signed Integer** | Both positive and negative values | L7 |
| **Floating Point** | Decimal numbers with very wide range — for continuous data like elevation | L7 |

### Data Type Ranges

| Type | Range |
|------|-------|
| Unsigned 8-bit | 0 to 255 |
| Unsigned 16-bit | 0 to 65,535 |
| Signed 8-bit | -128 to 127 |
| Signed 16-bit | -32,768 to 32,767 |

### Image Types

| Type | Bands | Bits |
|------|-------|------|
| Black & White | 1 | 2-bit (2 tones) |
| Grayscale | 1 | 8-bit (256 shades) |
| Color (RGB) | 3 | 8-bit each |

---

## L. Digitization (Analog → Digital)

| Term | Definition | Lecture |
|------|-----------|---------|
| **Analog Image** | Physical form (film, photo print) — degrades over time | L8 |
| **Digitization** | Process of converting analog to digital = **Sampling + Quantization** | L8 |
| **Sampling** | Dividing continuous scene into a **grid of pixels** — determines spatial resolution | L8 |
| **Quantization** | Assigning a **brightness number** to each pixel — determines radiometric resolution | L8 |
| **BV(i, j, k)** | Brightness Value at **row i, column j, band k** | L8 |
| **Pixel Neighborhood** | The 4 or 8 pixels surrounding a given pixel (4-connected = N,S,E,W; 8-connected = all 8) | L8 |
| **Metadata** | "Identity card" of the image — file name, date, rows, columns, bands, pixel size, georeferencing, statistics | L8 |
| **Auxiliary Data** | Additional info alongside the image — map projection, sun angle, cloud cover % | L8 |

---

## M. Image Processing — Subset, Mosaic & Display

| Term | Definition | Lecture |
|------|-----------|---------|
| **Image Subset** | Cutting out a **smaller area** from a large image (cropping) — saves storage & time | L9 |
| **Image Mosaicking** | Stitching **multiple overlapping images** into one seamless image (needs same projection, datum, pixel size, 20–30% overlap) | L9 |
| **Base Image** | The **reference image** in mosaicking — all other images align to it | L9 |
| **Band Composite** | Assigning spectral bands to R, G, B color guns to create a color display | L9 |
| **True Color Composite** | RGB = **3, 2, 1** — shows natural colors as our eyes see them | L9 |
| **False Color Composite** | RGB = **4, 3, 2** — NIR assigned to Red gun; **vegetation appears bright red** | L9 |
| **SWIR Composite** | RGB = **7, 4, 2** — useful for geology, soil, and moisture | L9 |

### Why Vegetation Looks Red in False Color
NIR (Band 4) → assigned to Red gun → vegetation reflects strongly in NIR → red gun fires hard → **vegetation = bright red**

---

## N. Univariate Statistics (One Band)

| Term | Definition | Formula | Lecture |
|------|-----------|---------|---------|
| **Histogram** | Bar chart of frequency of each brightness value (x = BV, y = count) | — | L10 |
| **Mean** | Average brightness | Σx / n | L10 |
| **Median** | Middle value when sorted | — | L10 |
| **Mode** | Most frequently occurring value | — | L10 |
| **Range** | Spread of data | Max − Min | L10 |
| **Variance (σ²)** | Average of squared deviations from the mean — measures spread | Σ(xi − mean)² / n | L10 |
| **Standard Deviation (σ)** | Square root of variance — spread in **same units** as data | √variance | L10 |
| **Population** | Complete set of **all** values | — | L10 |
| **Sample** | A **subset** of the population used for analysis | — | L10 |
| **Biased Sample** | Sample that does NOT fairly represent the whole population | — | L10 |
| **Sampling Error** | Difference between sample result and true population value | — | L10 |
| **Normal Distribution** | Bell-shaped curve — most values near the mean, fewer at extremes | — | L10 |

### Histogram Quick Guide

| Shape | Meaning |
|-------|---------|
| Narrow, clustered | Low contrast (dull image) |
| Wide, spread out | High contrast (sharp image) |
| Skewed left | Most pixels are dark |
| Skewed right | Most pixels are bright |

---

## O. Multivariate Statistics (Two+ Bands)

| Term | Definition | Formula | Lecture |
|------|-----------|---------|---------|
| **Univariate** | Stats of **one band** at a time | — | L11 |
| **Multivariate** | Stats of **two or more bands** together | — | L11 |
| **Covariance** | How two bands change together (+ve = same direction, −ve = opposite, 0 = no relation) | SP_kl / n | L11 |
| **SP (Sum of Products)** | Sum of multiplied deviations of two bands | Σ(BV_ik − mean_k)(BV_il − mean_l) | L11 |
| **Correlation Coefficient (r)** | Standardized covariance, ranges **-1 to +1** | cov_kl / (σ_k × σ_l) | L11 |
| **Variance-Covariance Matrix** | Table: diagonal = **variance** of each band, off-diagonal = **covariance** between pairs | — | L11 |
| **Correlation Matrix** | Table: diagonal = always **1**, off-diagonal = correlation between pairs (-1 to +1) | — | L11 |
| **Redundant Bands** | Highly correlated bands (r > 0.9) that carry **similar** information — can drop one | — | L11 |

### Correlation Quick Guide

| r Value | Meaning |
|---------|---------|
| +1 | Perfect positive — bands behave exactly the same |
| -1 | Perfect negative — bands behave exactly opposite |
| 0 | No relationship — completely independent |
| > 0.9 | Very similar → redundant (can drop one) |
| < 0.5 | Different → unique info (keep both) |

---

## P. All Acronyms

| Acronym | Full Form |
|---------|-----------|
| **RS** | Remote Sensing |
| **EMR** | Electromagnetic Radiation |
| **NIR** | Near Infrared |
| **SWIR** | Shortwave Infrared |
| **IFOV** | Instantaneous Field of View |
| **CCD** | Charged Couple Device |
| **UAV** | Unmanned Aerial Vehicle |
| **BIP** | Band Interleaved by Pixel |
| **BIL** | Band Interleaved by Line |
| **BSQ** | Band Sequential |
| **BV** | Brightness Value |
| **DN** | Digital Number |
| **RGB** | Red, Green, Blue |
| **TDRSS** | Tracking and Data Relay Satellite System |
| **MSS** | Multispectral Scanner |
| **TM** | Thematic Mapper |
| **AVHRR** | Advanced Very High Resolution Radiometer |
| **SPOT** | Satellite Pour l'Observation de la Terre |
| **SD** | Standard Deviation |
| **SP** | Sum of Products |

---
