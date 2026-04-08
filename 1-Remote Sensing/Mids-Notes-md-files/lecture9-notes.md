# Lecture 9: Image Display, Subset & Mosaicking

---

## 1. Image Subset (Clipping)

### What is it?
- **Cutting out a smaller portion** from a large image
- You only keep the area you need — the rest is discarded

### Why use it?
| Reason | Explanation |
|--------|-------------|
| **Save storage** | Smaller file = less disk space |
| **Faster processing** | Less data = quicker computer work |
| **Focus on study area** | Work only with the area that matters |

> Think of it as: **Cropping a photo on your phone — keep only what you need**

### How to subset:
- Draw a **rectangle** (bounding box) around your area of interest
- Define by **row/column numbers** or **geographic coordinates**

---

## 2. Image Mosaicking (Stitching)

### What is it?
- **Joining multiple overlapping images** into one seamless large image
- Like putting puzzle pieces together

### Requirements for Mosaicking:
| Requirement | Why |
|-------------|-----|
| **Same map projection** | Images must be on same coordinate system |
| **Same datum** | Same reference surface for coordinates |
| **Same pixel size** | Resolution must match for proper alignment |
| **20–30% overlap** | Need overlap area to stitch properly |
| **Base image** | One image acts as the reference (others adjust to it) |

### Steps:
1. Choose a **base image** (reference)
2. **Align** other images to the base
3. **Blend** overlapping areas so seams are not visible
4. Result: **One large seamless image**

> Think of it as: **Stitching panorama photos on your phone — many shots become one wide image**

---

## 3. Image Display — Band Composites

### How Color Images Are Made:
- Computer monitor uses **3 color guns**: Red (R), Green (G), Blue (B)
- You assign **any spectral band** to each color gun
- Result = a **color composite** image

### True Color Composite (Natural Color):
```
RGB = 3, 2, 1
R → Band 3 (Red band)
G → Band 2 (Green band)
B → Band 1 (Blue band)
```
- Shows the scene as **human eyes would see it**
- Vegetation = green, water = blue, soil = brown

### False Color Composite (Color Infrared):
```
RGB = 4, 3, 2
R → Band 4 (NIR — Near Infrared)
G → Band 3 (Red band)
B → Band 2 (Green band)
```
- **Vegetation appears RED** (because NIR is assigned to Red gun, and vegetation reflects strongly in NIR)
- Used to **detect vegetation health** — healthy vegetation = bright red

### SWIR Composite:
```
RGB = 7, 4, 2
R → Band 7 (SWIR)
G → Band 4 (NIR)
B → Band 2 (Green)
```
- Useful for **geology, soil, moisture** studies

---

## 4. Why Does Vegetation Look RED in False Color?

Simple explanation:
1. **Vegetation reflects a LOT of NIR** (Band 4)
2. In false color, **Band 4 is assigned to the Red gun**
3. So wherever there is vegetation → the Red gun fires strongly
4. Result: **Vegetation appears bright red**

> Memory trick: **NIR loves plants, Red gun shows NIR → plants look red in false color**

---

## 5. Land Cover Appearance in Different Composites

| Land Cover | True Color (3,2,1) | False Color (4,3,2) |
|-----------|--------------------|--------------------|
| **Healthy Vegetation** | Green | **Bright Red** |
| **Stressed Vegetation** | Yellowish-green | **Dark Red / Pink** |
| **Water (clear)** | Blue / Dark blue | **Dark Blue / Black** |
| **Urban / Built-up** | Gray | **Cyan / Light blue** |
| **Bare Soil** | Brown / Tan | **Light brown / Yellow** |
| **Snow / Clouds** | White | **White** |

---

## 6. Key Band Numbers (Landsat)

| Band | Name | Wavelength Range |
|------|------|-----------------|
| Band 1 | Blue | 0.45 – 0.52 μm |
| Band 2 | Green | 0.52 – 0.60 μm |
| Band 3 | Red | 0.63 – 0.69 μm |
| Band 4 | NIR (Near Infrared) | 0.76 – 0.90 μm |
| Band 5 | SWIR-1 | 1.55 – 1.75 μm |
| Band 7 | SWIR-2 | 2.09 – 2.35 μm |

---

## Key Definitions to Remember

| Term | Definition |
|------|------------|
| **Subset** | Cutting out a small area from a large image |
| **Mosaicking** | Stitching multiple overlapping images into one |
| **Band composite** | Assigning spectral bands to RGB color guns to create a color image |
| **True color** | RGB = 3,2,1 — shows natural colors as our eyes see |
| **False color** | RGB = 4,3,2 — shows NIR as red; vegetation appears red |
| **Base image** | Reference image in mosaicking — others align to it |
| **NIR** | Near Infrared — strongly reflected by healthy vegetation |

---
