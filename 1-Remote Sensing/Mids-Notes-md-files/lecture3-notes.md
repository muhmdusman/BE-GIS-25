# Lecture 3: Digital Image and Resolutions

---

## 1. Digital Image Basics

- Digital images are made up of discrete elements called **PIXELS**
- Each pixel stores a **number (DN — Digital Number)** representing brightness
- The image is essentially a **matrix of numbers**
- As **pixel size decreases** → more scene detail is preserved

---

## 2. Pixel Properties

A pixel has **two** properties:

| Property | Meaning |
|----------|---------|
| **Spatial** | Defines the dimensions of the corresponding ground area (pixel size on ground) |
| **Spectral** | Defines the intensity of spectral response for a pixel in a particular band |

- **Aspect Ratio** = 1 (pixel is square)

---

## 3. Resolution — Overview

- **Resolution** = The ability of a remote sensing system to render a sharply defined image
- It indicates the **smallest observable/measurable difference**

### Four Types of Resolution:

| Type | Property Of | What It Measures |
|------|------------|-----------------|
| **Spatial** | Sensor/Instrument | Size of smallest detectable object |
| **Spectral** | Sensor/Instrument | Number and width of wavelength bands |
| **Radiometric** | Sensor/Instrument | Number of brightness levels recorded |
| **Temporal** | Platform | How often an area is revisited |

---

## 4. Spatial Resolution

- Measures the **smallest object** a sensor can detect
- Also refers to the **size of ground area represented by each pixel**
- Smaller pixel = **higher resolution** = more ground detail = **larger file size**

### Detection Rule:
- An object must be **equal to or larger** than the resolution cell
- To detect an object → spatial resolution should be **less than half** the object's smaller dimension
- Example: To identify a 4 m wide home → need **minimum 2 m** spatial resolution

### Spatial Resolution Classes:

| Class | Pixel Size |
|-------|-----------|
| **Coarse/Low** | > 30 m to > 1000 m |
| **Medium** | > 4 m to 30 m |
| **High/Fine** | 1 m to 4 m |
| **Very High** | Sub-meter (< 1 m) |

---

## 5. Map Scale

- **Map Scale** = Ratio of distance on map to actual ground distance
- **Small scale** = small map-to-ground ratio → e.g., 1:100,000 (covers large area, less detail)
- **Large scale** = larger ratio → e.g., 1:5,000 (covers small area, more detail)

### Scale vs Pixel Size (Examples):

| Scale | Approx Pixel Size | Sensor |
|-------|--------------------|--------|
| 1:50,000 | 4 m | Aircraft, IKONOS |
| 1:250,000 | 20–30 m | SPOT, Landsat TM |
| 1:500,000 | 50 m | Landsat MSS |
| 1:10,000,000 | 1000 m | NOAA AVHRR |

---

## 6. Spectral Resolution

- Refers to the **specific wavelength intervals** a sensor can record
- Each wavelength interval = a **band**
- **High spectral resolution** = **narrow bandwidth** (finer divisions of the spectrum)
- In general: the **number of bands** of a sensor system

### Image Types by Spectral Resolution:

| Type | Bands | Result |
|------|-------|--------|
| **Panchromatic** | 1 band | Gray scale image |
| **Multispectral** | 3+ bands | Color image (e.g., RGB) |

- Gray scale image = single band, intensity is sum of all visible wavelengths
- Color image needs **at least 3 bands** (Red, Green, Blue) for full color

> For **urban land cover**, spatial resolution is considered **more important** than spectral resolution.

---

## 7. Radiometric Resolution

- The ability of a sensor to record **many levels of brightness**
- **Coarse** radiometric resolution = few brightness levels
- **Fine** radiometric resolution = many brightness levels
- The finer the radiometric resolution → more sensitive to **small energy differences**

### Brightness Value Ranges (by bit depth):

| Bit Depth | Number of Tones | Range (Black to White) |
|-----------|----------------|----------------------|
| 1 bit | 2 | 0 – 1 |
| 2 bit | 4 | 0 – 3 |
| 4 bit | 16 | 0 – 15 |
| 5 bit | 32 | 0 – 31 |
| 6 bit | 64 | 0 – 63 |
| 7 bit | 128 | 0 – 127 |
| **8 bit** | **256** | **0 – 255** |
| 11 bit | 2048 | 0 – 2047 |

> **Formula**: Number of tones = $2^n$ where n = number of bits

---

## 8. Temporal Resolution

- How often a given place on Earth is **revisited** (imaged) by a RS system
- Fixed depending on **orbital parameters** of the satellite
- Each satellite has its own **unique revisit schedule**
- Example: If a satellite images the same area every 16 days → temporal resolution = **16 days**

### Factors Affecting Temporal Resolution:
1. **Satellite/sensor capabilities**
2. **Swath overlap**
3. **Latitude**

- Important for **change detection** studies
- **Aerial imaging** → temporal resolution is **flexible** (weather dependent)
- **Moving sensors** can have revisit time of **1–5 days**

---

## Key Definitions to Remember

| Term | Definition |
|------|------------|
| **Pixel** | Smallest element of a digital image; has spatial and spectral properties |
| **Spatial Resolution** | Size of the ground area represented by one pixel |
| **Spectral Resolution** | Number and width of wavelength bands a sensor records |
| **Radiometric Resolution** | Number of brightness levels a sensor can distinguish |
| **Temporal Resolution** | How often a sensor revisits and images the same area |
| **DN (Digital Number)** | The brightness value stored in a pixel |
| **Map Scale** | Ratio of map distance to actual ground distance |

---
