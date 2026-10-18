# GIE-203 Lecture Notes (Lectures 1–20)

Simple, easy-to-read notes covering every concept from the lectures, with diagrams pulled from the slides and memory acronyms for things worth remembering.

## Contents

1. [Lecture 1 — Geometric Corrections (Part I)](Lecture-1-Geometric-Corrections-I.md)
   - Geometric errors, GCPs, rectification vs registration, resampling (NN/Bilinear/Cubic), RMS error.
2. [Lecture 2 — Geometric Corrections (Part II)](Lecture-2-Geometric-Corrections-II.md)
   - Altitude/attitude errors, image skew & deskew, panoramic distortion, Earth curvature, relief displacement.
3. [Lecture 3 — Radiometric / Atmospheric Corrections (Part I)](Lecture-3-Radiometric-Atmospheric-Corrections-I.md)
   - Sensor distortions, vignetting, illumination/view angles, sun-elevation correction, topographic (cosine) correction.
4. [Lecture 4 — Radiometric / Atmospheric Corrections (Part II)](Lecture-4-Radiometric-Atmospheric-Corrections-II.md)
   - Path radiance, adjacency effect, haze removal (HMM/DOS, regression), empirical line method, DN↔radiance↔reflectance calibration.
5. [Lecture 5 — Multi-band Operations & Spectral Transforms](Lecture-5-Multiband-Operations-Spectral-Transforms.md)
   - Add/subtract/multiply/divide operations, band ratioing, spectral ratios, ratio composites.
6. [Lecture 6 — Normalized Difference Vegetation Index (NDVI)](Lecture-6-NDVI.md)
   - Vegetation spectral response, vegetation indices, RVI/DVI/NDVI, NDVI value scale and uses.
7. [Lecture 7 — Soil-Adjusted Vegetation Index (SAVI)](Lecture-7-SAVI.md)
   - Soil line, PVI, SAVI and the L-factor, TSAVI, MSAVI, EVI.
8. [Lecture 8 — Water, Built-Up & Bare Soil Indices](Lecture-8-Water-BUA-BareSoil-Indices.md)
   - VI summary, NDWI, NDMI, NDSI, BSI/MBI, Sentinel-2 index reference table.
9. [Lecture 9 — Tasseled Cap Transformation (TCT)](Lecture-9-Tasseled-Cap-Transformation.md)
   - Kauth-Thomas transform, Brightness/Greenness/Yellowness/Wetness axes, crop sequence, MSS vs TM.
10. [Lecture 10 — Principal Component Analysis (PCA)](Lecture-10-Principal-Component-Analysis-PCA.md)
    - Image/spectral/feature space, spectral redundancy, PCT, PC1/PC2 rotation, scene-specific vs TCT.
11. [Lecture 11 — Spatial Convolution Filtering & Spatial Transforms](Lecture-11-Spatial-Convolution-Filtering.md)
    - Spatial frequency, convolution kernels, low-pass vs high-pass filters, mean/min/max/median neighbourhood operations.
12. [Lecture 12 — Image Classification (Introduction)](Lecture-12-Image-Classification-Introduction.md)
    - RS workflow, spectral vs information classes, supervised/unsupervised, per-pixel vs object-oriented, land use vs land cover, USGS/Anderson system.
13. [Lecture 13 — Ground Reference Data](Lecture-13-Ground-Reference-Data.md)
    - Ground truth vs ground reference, purposes, types of reference data, agricultural data, site suitability, geo-referencing.
14. [Lecture 14 — Visual Image Interpretation](Lecture-14-Visual-Image-Interpretation.md)
    - Elements of interpretation (shape, tone, texture, pattern, shadow, site, association, resolution), direct recognition vs inference.
15. [Lecture 15 — Image Classification: Unsupervised](Lecture-15-Unsupervised-Classification.md)
    - Clustering, K-Means (minimum distance to means), ISODATA (split & merge), software settings, post-classification.

## How to read these
- Each file opens with a one-line "big idea," then explains every concept in plain words.
- **Memory tips** and **acronyms** are highlighted in blockquotes for quick recall.
- Each file ends with a **Quick Revision Cheat-Sheet** for last-minute review.
- Diagrams are stored in `images/lec1` … `images/lec15`.

> Tip: Open these `.md` files in a Markdown preview to see the formatting, tables, and images rendered nicely.
