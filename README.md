# UNet-Flood-Segmentation
# Swat KPK Flood Segmentation 2025
## Using U-Net Deep Learning

## Study Area
Swat Valley KPK Pakistan 2025

## Data Used
- Sentinel-1 SAR Before Flood
- Sentinel-1 SAR During Flood
- SRTM DEM
- Slope
- CHIRPS Rainfall

## Model Architecture
U-Net Encoder Decoder
- 3 encoder blocks
- Bottleneck 128 filters
- 3 decoder blocks
- Skip connections
- Weighted loss for flood pixels

## Results
- Test Accuracy: 99.70%
- Flood Recall: 76.94%
- Flood Precision: 34.62%
- Flood F1 Score: 0.48

## Key Achievement
Model successfully detected 77% of
actual flood pixels despite extreme
class imbalance (179 flood pixels
vs 261,965 no flood pixels)

## Tools
- TensorFlow Keras
- Google Earth Engine
- Rasterio
- Python
