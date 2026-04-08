# Lecture 7: Remote Sensing Data Formats

---

## 1. What is a Digital Image?

- A **numerical record** of the radiance (brightness) leaving each pixel in each spectral band
- Values are represented in terms of **radiometric resolution** (usually 8-bit = 0–255)

---

## 2. Why Digital Images? (Advantages Over Analog)

| Advantage | Explanation |
|-----------|------------|
| **No digitization needed** | Data is already digital — user doesn't have to convert it |
| **No info lost** | No information missing or changed from provider to user |
| **Easier storage** | Digital files easier to store and manage than physical photos |
| **No color loss** | Colors don't fade or degrade during storage |
| **More info (> 3 bands)** | Can contain many more bands than a simple RGB photo |
| **Flexible output** | Can create many different band combinations for viewing |

> Simple way to remember: Digital = **no loss, more bands, easier to store and share**

---

## 3. Digital Image Data Storage Schemes

There are **three main ways** to organize multi-band image data in a file:

### 3.1 Band Interleaved by Pixel (BIP)

**How it works:** For each pixel, store **all its band values together** before moving to next pixel.

```
Pixel(1,1)-Band1, Pixel(1,1)-Band2, Pixel(1,1)-Band3
Pixel(1,2)-Band1, Pixel(1,2)-Band2, Pixel(1,2)-Band3
Pixel(1,3)-Band1, Pixel(1,3)-Band2, Pixel(1,3)-Band3
...
```

> Think of it as: **"All colors of one pixel, then all colors of next pixel"**

### 3.2 Band Interleaved by Line (BIL)

**How it works:** Store **one full line** of band 1, then same line of band 2, then band 3... then move to line 2.

```
Line1-Band1, Line1-Band2, Line1-Band3
Line2-Band1, Line2-Band2, Line2-Band3
...
```

> Think of it as: **"All bands of line 1, then all bands of line 2"**

### 3.3 Band Sequential (BSQ)

**How it works:** Store the **entire image for band 1** first, then entire image for band 2, etc. Each band is a separate file.

```
Band 1: Line1, Line2, Line3... (entire image)
Band 2: Line1, Line2, Line3... (entire image)
Band 3: Line1, Line2, Line3... (entire image)
```

> Think of it as: **"Complete picture of band 1, then complete picture of band 2"**

### Quick Comparison:

| Format | Organizes By | Simple Memory Trick |
|--------|-------------|-------------------|
| **BIP** | Pixel by pixel | All bands of **one pixel** together |
| **BIL** | Line by line | All bands of **one line** together |
| **BSQ** | Band by band | **One whole band** at a time |

---

## 4. How 3 Bands Are Stored in BIP (Diagram)

For a 3×3 image with 3 bands:

```
BIP Order:
┌─────────────────────────────────────────────────┐
│ P(1,1)B1 │ P(1,1)B2 │ P(1,1)B3 │ → pixel 1   │
│ P(1,2)B1 │ P(1,2)B2 │ P(1,2)B3 │ → pixel 2   │
│ P(1,3)B1 │ P(1,3)B2 │ P(1,3)B3 │ → pixel 3   │
│ P(2,1)B1 │ P(2,1)B2 │ P(2,1)B3 │ → pixel 4   │
│ ...      │ ...      │ ...      │              │
└─────────────────────────────────────────────────┘
  Band1      Band2      Band3

For a given pixel → values for ALL bands are side by side
```

---

## 5. Raster Data — Multi-Band Structure

- Each band is a **separate layer** (like stacked transparent sheets)
- All bands are **registered** — pixel in band 1 aligns exactly with same pixel in other bands
- Think of it as **superimposed images** on top of each other

---

## 6. Raster Data Storage Types

| Storage Type | Range | Use |
|-------------|-------|-----|
| **Unsigned 8-bit integer** | 0 to 255 | Most common for images |
| **Unsigned 16-bit integer** | 0 to 65,535 | Higher radiometric data |
| **Signed 8-bit integer** | -128 to 127 | Can store negative values |
| **Signed 16-bit integer** | -32,768 to 32,767 | Can store negative values |
| **Floating point** | Very wide range | Continuous data (e.g., elevation) |

### Unassigned Bit Range in 8-bit:
- 8-bit **unsigned** = 0 to 255 (all 256 values used for brightness)
- 8-bit **signed** = -128 to 127 (negative values not used for brightness)
- **Unassigned range** in signed 8-bit = the negative values (-128 to -1) are not used for brightness

---

## 7. Image Representations

| Type | Bands | Bits | What It Shows |
|------|-------|------|---------------|
| **Black & White** | 1 band | 2 bits | Only black and white (2 tones) |
| **Gray Scale** | 1 band | 8 bits | 256 shades of gray |
| **Color Image** | 3 bands | 8 bits each | Full color (RGB) |

---

## Key Definitions to Remember

| Term | Definition |
|------|------------|
| **BIP** | Band Interleaved by Pixel — all bands of one pixel stored together |
| **BIL** | Band Interleaved by Line — all bands of one line stored together |
| **BSQ** | Band Sequential — one entire band stored as a complete file |
| **Raster** | Grid/matrix of pixels — how RS images are stored |
| **Unsigned integer** | Only positive values (0 and up) |
| **Signed integer** | Positive and negative values |

---
