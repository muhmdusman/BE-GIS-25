# Lecture 11: Image Statistics II — Multivariate Statistics

---

## 1. Recap: Image Notation

```
BV(i, j, k)

i = row
j = column
k = band
```

- **Univariate** = statistics of **one band** at a time (Lecture 10)
- **Multivariate** = statistics of **two or more bands** together (this lecture)

---

## 2. Why Multivariate Statistics?

- To understand **relationships between bands**
- Example: Do Band 3 (Red) and Band 4 (NIR) behave similarly or differently?
- Helps decide: **Which bands to use together?** Which bands carry **unique** vs **redundant** information?

---

## 3. Covariance

### What is it?
- Measures how **two bands change together**
- Do they go up together? Or when one goes up, the other goes down?

### Formula:
```
Covariance (cov_kl) = SP_kl / n

Where:
SP_kl = Σ (BV_ik − mean_k) × (BV_il − mean_l)

k = band k
l = band l
n = number of pixels
```

### Steps to Calculate:
1. Find **mean** of band k and **mean** of band l
2. For each pixel: subtract means from both bands → get deviations
3. **Multiply** the two deviations together (for the same pixel)
4. **Sum** all these products → this gives **SP** (Sum of Products)
5. **Divide** SP by n

### What Covariance Values Mean:

| Covariance | Meaning |
|-----------|---------|
| **Positive (+)** | Both bands increase together (similar behavior) |
| **Negative (−)** | One band goes up while the other goes down (opposite behavior) |
| **Zero (0)** | No relationship between the two bands |

> Note: Covariance of a band **with itself** = **Variance** of that band

---

## 4. Correlation Coefficient

### What is it?
- A **standardized version** of covariance
- Always falls between **-1 and +1** → easier to interpret

### Formula:
```
r_kl = cov_kl / (σ_k × σ_l)

Where:
r_kl = correlation between band k and band l
cov_kl = covariance of bands k and l
σ_k = standard deviation of band k
σ_l = standard deviation of band l
```

### Interpretation:

| r Value | Meaning | Example |
|---------|---------|---------|
| **r = +1** | Perfect positive correlation | Both bands behave exactly the same |
| **r = -1** | Perfect negative correlation | Bands behave exactly opposite |
| **r = 0** | No correlation | Bands are completely independent |
| **r = +0.9** | Strong positive | Bands are very similar → redundant info |
| **r = +0.3** | Weak positive | Bands are somewhat different → unique info |

> **High correlation** between 2 bands = they carry **similar/redundant** information
> **Low correlation** = they carry **different/unique** information → use both!

---

## 5. Variance-Covariance Matrix

- A **table** that shows variance of each band AND covariance between every pair of bands
- **Diagonal** = variance of each band (with itself)
- **Off-diagonal** = covariance between pairs

### Format (for 3 bands):
```
              Band 1      Band 2      Band 3
Band 1    [var₁       cov₁₂      cov₁₃]
Band 2    [cov₂₁      var₂       cov₂₃]
Band 3    [cov₃₁      cov₃₂      var₃ ]
```

| Position | Contains |
|----------|----------|
| **Diagonal** (var₁, var₂, var₃) | Variance of each band |
| **Off-diagonal** (cov₁₂, etc.) | Covariance between band pairs |
| **Symmetric** | cov₁₂ = cov₂₁ (same value) |

---

## 6. Correlation Matrix

- Same layout as variance-covariance matrix, but uses **correlation** values instead
- **Diagonal** = always **1** (a band correlates perfectly with itself)
- **Off-diagonal** = correlation between pairs (between -1 and +1)

### Format (for 3 bands):
```
              Band 1    Band 2    Band 3
Band 1    [  1.00     r₁₂      r₁₃   ]
Band 2    [  r₂₁      1.00     r₂₃   ]
Band 3    [  r₃₁      r₃₂      1.00  ]
```

> **Diagonal is always 1** because every band is perfectly correlated with itself

---

## 7. Practical Use

| Situation | Action |
|-----------|--------|
| Two bands have **high correlation** (r > 0.9) | They give similar info → you can **drop one** |
| Two bands have **low correlation** (r < 0.5) | They give different info → **keep both** for analysis |
| Want to reduce data size | Use correlation matrix to find **redundant bands** |

---

## Key Definitions to Remember

| Term | Definition |
|------|------------|
| **Covariance** | Measures how two bands change together (positive = same direction, negative = opposite) |
| **Correlation** | Standardized covariance, ranges from -1 to +1 |
| **r = +1** | Perfect positive correlation |
| **r = -1** | Perfect negative correlation |
| **r = 0** | No correlation / independent |
| **Variance-covariance matrix** | Table of variances (diagonal) and covariances (off-diagonal) |
| **Correlation matrix** | Table of correlations; diagonal always = 1 |
| **Redundant bands** | Highly correlated bands that carry similar information |
| **SP (Sum of Products)** | Sum of multiplied deviations of two bands |

---
