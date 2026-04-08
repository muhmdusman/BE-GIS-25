# Lecture 8: Digital Image — From Analog to Digital

---

## 1. Analog vs Digital Image

| Feature | Analog Image | Digital Image |
|---------|-------------|---------------|
| **Form** | Physical (film, photo print) | Electronic (numbers/pixels) |
| **Storage** | Physical — fades over time | Digital — no degradation |
| **Processing** | Manual darkroom | Computer software |
| **Copying** | Each copy loses quality | Perfect copies every time |
| **Sharing** | Physical delivery needed | Instant digital transfer |
| **Example** | Old film camera photo | Satellite image, phone photo |

> **Key advantage of digital:** No information loss, easy to process by computer, can store many spectral bands

---

## 2. Digitization — Converting Analog to Digital

To convert an analog (continuous) signal into digital, you need **2 steps**:

### Step 1: Sampling
- **What:** Dividing the continuous image into a **grid of small boxes** (pixels)
- Each box becomes one **pixel** (picture element)
- The **more samples** you take → **higher spatial resolution** → more detail

> Think of it as: **Placing a grid on a photo — each grid cell becomes one pixel**

### Step 2: Quantization
- **What:** Assigning a **numeric value** (brightness number) to each pixel
- Each pixel gets a value based on how bright/dark it is
- The **number of levels** depends on **radiometric resolution** (bits)
  - 2 bits → 4 levels
  - 4 bits → 16 levels
  - 8 bits → 256 levels (most common)

> Think of it as: **Measuring the brightness of each grid cell and writing down a number**

### Complete Process:
```
Analog Image → Sampling (grid it) → Quantization (number it) → Digital Image
```

---

## 3. Image Notation — How Pixels Are Referenced

- **Row (r)** = horizontal line (goes across, left to right)
- **Column (c)** = vertical line (goes up-down)
- **Band (k)** = spectral layer

### Pixel Reference System:
```
BV(i, j, k)

i = row number
j = column number
k = band number
```

**Example:** BV(3, 5, 2) = brightness value at row 3, column 5, band 2

### Image as a Matrix:
```
An image with R rows, C columns, K bands:

     Col 1  Col 2  Col 3  ... Col C
Row 1  [45]   [67]   [23]  ...  [89]
Row 2  [12]   [55]   [78]  ...  [34]
Row 3  [90]   [31]   [66]  ...  [47]
...
Row R  [22]   [81]   [43]  ...  [56]

↑ This is ONE band. Stack K such matrices for a multi-band image.
```

---

## 4. Pixel Neighborhood

A pixel has **4 direct neighbors** (up, down, left, right) and **4 diagonal neighbors**:

```
    ┌─────┬─────┬─────┐
    │ NW  │  N  │ NE  │  ← diagonal + direct
    ├─────┼─────┼─────┤
    │  W  │  P  │  E  │  ← P = center pixel
    ├─────┼─────┼─────┤
    │ SW  │  S  │ SE  │
    └─────┴─────┴─────┘

4-connected = N, S, E, W (direct neighbors)
8-connected = all 8 surrounding pixels
```

---

## 5. Metadata — Data About the Data

Metadata is the **information that describes the image file**. It tells you everything about the image WITHOUT opening it.

| Metadata Item | What It Tells You |
|--------------|-------------------|
| **File name** | Name of the image file |
| **Date of acquisition** | When the image was captured |
| **Quantization** | How many bits per pixel (e.g., 8-bit) |
| **Number of rows** | How many horizontal lines |
| **Number of columns** | How many vertical lines |
| **Number of bands** | How many spectral layers |
| **Statistics** | Min, max, mean values per band |
| **Georeferencing** | Map coordinates (where it is located on Earth) |
| **Pixel size** | Ground area each pixel covers (e.g., 30m × 30m) |

> Simple way to remember: Metadata = **"identity card of the image"**

---

## 6. Auxiliary Data

- Additional information stored **alongside** the image
- Examples: map projection, sensor type, sun elevation angle, cloud cover %
- Helps in **proper interpretation** and **processing** of the image

---

## Key Definitions to Remember

| Term | Definition |
|------|------------|
| **Sampling** | Dividing continuous scene into grid of pixels |
| **Quantization** | Assigning a brightness number to each pixel |
| **BV(i,j,k)** | Brightness Value at row i, column j, band k |
| **Metadata** | Descriptive information about the image (rows, cols, bands, date, etc.) |
| **Pixel neighborhood** | The 4 or 8 pixels surrounding a given pixel |
| **Digitization** | Process of converting analog to digital (sampling + quantization) |

---
