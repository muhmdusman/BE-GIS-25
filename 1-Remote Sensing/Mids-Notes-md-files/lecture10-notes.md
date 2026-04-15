# Lecture 10: Image Statistics I — Univariate Statistics

---

## 1. Why Do We Need Image Statistics?

- To **assess image quality** — is the data good enough to use?
- To **detect errors or noise** in the image
- To **understand** the distribution of brightness values
- To **compare** different bands or images

---

## 2. Errors and Noise in Images

| Source | Example |
|--------|---------|
| **Sensor malfunction** | Broken detector → striping in image |
| **Atmospheric interference** | Haze, clouds reduce clarity |
| **Transmission errors** | Data corrupted during satellite-to-ground transfer |
| **Calibration errors** | Sensor not properly calibrated |

> Images must be checked for errors **before** any analysis

---

## 3. Sampling Theory Basics

| Term | Definition |
|------|------------|
| **Population** | The **complete set** of all data values (entire image) |
| **Sample** | A **subset** of the population used for analysis |
| **Biased sample** | Sample that does NOT fairly represent the whole population |
| **Sampling error** | The difference between sample result and true population value |
| **Normal distribution** | Bell-shaped curve — most values near the center (mean), fewer at extremes |

> Simple rule: A **good sample** is one that **represents the whole population fairly**

---

## 4. Histogram

### What is it?
- A **bar chart** showing how many pixels have each brightness value
- X-axis = brightness values (0 to 255 for 8-bit)
- Y-axis = number of pixels (frequency)
Prcatice Question : Practice 3*3 table values histogram

```
Frequency
  │   ░░
  │   ░░░░
  │  ░░░░░░░
  │ ░░░░░░░░░░
  │░░░░░░░░░░░░░
  └──────────────→ Brightness Value
  0    50  100  150  200  255
```

### What it tells us:
| Histogram Shape | Meaning |
|----------------|---------|
| **Narrow, clustered** | Low contrast (image looks dull/flat) |
| **Wide, spread out** | High contrast (image looks sharp) |
| **Skewed left** | Most pixels are dark |
| **Skewed right** | Most pixels are bright |
| **Bell-shaped** | Normal distribution — balanced |

---

## 5. Univariate Statistics (One Variable/Band at a Time)

### 5.1 Mean (Average)
- **Sum of all values ÷ number of values**
- Formula: **Mean = Σx / n**
- Tells the **central/typical brightness** of the image

### 5.2 Median
- **Middle value** when all values are arranged in order
- If n is odd: middle number
- If n is even: average of two middle numbers
- **Not affected by extreme values** (outliers)

### 5.3 Mode
- The **most frequent value** — appears the most times
- A dataset can have **multiple modes** or **no mode**

### Quick Comparison:

| Statistic | What It Is | When to Use |
|----------|-----------|-------------|
| **Mean** | Average of all values | General center |
| **Median** | Middle value | When outliers exist |
| **Mode** | Most common value | Most typical pixel value |

---

### 5.4 Range
- **Largest value − Smallest value**
- Shows the **spread** of data
- Formula: **Range = Max − Min**

### 5.5 Variance
- Measures **how spread out** the values are from the mean
- **Large variance** = values are widely spread
- **Small variance** = values are close to the mean

**Formula:**
```
Variance (σ²) = Σ(xi − mean)² / n
```

**Steps to calculate:**
1. Find the mean
2. Subtract mean from each value → get deviations
3. Square each deviation
4. Sum all squared deviations
5. Divide by n (number of values)

### 5.6 Standard Deviation (SD)
- **Square root of variance**
- Easier to understand because it's in **same units** as the data
- Formula: **SD (σ) = √variance**

| SD Value | Meaning |
|----------|---------|
| **Small SD** | Values are close to mean → low spread |
| **Large SD** | Values are far from mean → high spread |

---

## 6. Worked Example

Dataset: **2, 4, 6, 8, 10**

| Step | Calculation | Result |
|------|------------|--------|
| **Mean** | (2+4+6+8+10) / 5 | **6** |
| **Median** | Middle of sorted list: 2,4,**6**,8,10 | **6** |
| **Mode** | No repeated values | **No mode** |
| **Range** | 10 − 2 | **8** |
| **Variance** | [(2-6)²+(4-6)²+(6-6)²+(8-6)²+(10-6)²] / 5 = [16+4+0+4+16]/5 | **8** |
| **SD** | √8 | **2.83** |

---

## Key Definitions to Remember

| Term | Definition |
|------|------------|
| **Histogram** | Bar chart showing frequency of each brightness value |
| **Mean** | Average value = sum ÷ count |
| **Median** | Middle value when sorted |
| **Mode** | Most frequent value |
| **Range** | Max − Min |
| **Variance** | Average of squared deviations from mean |
| **Standard Deviation** | Square root of variance — spread of values |
| **Normal distribution** | Bell curve — most values near the mean |
| **Population** | Complete set of all values |
| **Sample** | Subset taken from population |

---
