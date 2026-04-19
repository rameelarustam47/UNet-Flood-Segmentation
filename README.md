# Flood Segmentation in Swat Valley using U-Net (Deep Learning)

## 🌊 Problem Statement

This study focuses on pixel-level flood inundation mapping using deep learning to detect flood-affected areas under extreme class imbalance conditions.

---

## 📍 Study Area

Swat Valley

---

## 📡 Data Sources

* Sentinel-1 SAR (pre-flood)
* Sentinel-1 SAR (during flood)
* SRTM DEM (30m)
* Slope derived from DEM
* CHIRPS rainfall data

---

## 🧠 Model Architecture (U-Net)

A U-Net encoder–decoder architecture was used for flood segmentation:

* 3 encoder blocks for feature extraction
* Bottleneck layer with 128 filters
* 3 decoder blocks for reconstruction
* Skip connections for spatial detail preservation
* Weighted loss function to handle class imbalance

---

## 🌍 Physically-Informed Component

Terrain variables (DEM, slope) and rainfall data were incorporated to guide spatial consistency, allowing the model to learn hydrologically meaningful flood patterns.

---

## 📊 Results

* Overall Accuracy: **99.70%**
* Flood Recall: **76.94%**
* Flood Precision: **34.62%**
* Flood F1 Score: **0.48**

---

## 🔍 Key Insight

Despite extreme class imbalance (179 flood pixels vs 261,965 non-flood pixels), the model successfully detected ~77% of flood pixels, demonstrating strong sensitivity to rare flood events.

However, precision remains low, indicating false positives in boundary regions—common in SAR-based flood mapping.

---

## 🛠️ Tools & Technologies

* TensorFlow (Keras)
* Google Earth Engine
* Rasterio
* Python

---

## 🎯 Future Improvements

* Incorporate attention mechanisms (Attention U-Net)
* Improve class imbalance handling
* Integrate hydrological constraints for physically-consistent predictions
