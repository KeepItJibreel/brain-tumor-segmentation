# Brain Tumor Segmentation — U-Net

A U-Net convolutional neural network trained to perform binary segmentation of brain tumor MRI scans, built with TensorFlow/Keras.

---

## Results (threshold = 0.05)

| Metric | Raw | Cleaned |
|---|---|---|
| Dice | 0.7498 ± 0.2405 | 0.7555 ± 0.2452 |
| IoU | 0.6455 ± 0.2427 | 0.6546 ± 0.2455 |
| Precision | 0.7838 ± 0.2215 | 0.7964 ± 0.2219 |
| Recall | 0.8206 ± 0.2562 | 0.8180 ± 0.2619 |

---

## What's inside

- Custom U-Net architecture built from scratch
- Combined focal + dice loss to handle class imbalance
- Data augmentation pipeline (flips, rotations, zoom, brightness/contrast/saturation)
- Threshold search across multiple values to maximize validation Dice
- Post-processing (mask cleaning) with before/after comparison

## Tech
Python · TensorFlow · Keras · NumPy · Matplotlib