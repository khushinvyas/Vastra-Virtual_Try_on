# Vastra-Virtual_Try_on

## Overview
This project presents a novel **Virtual Try-on System** using **Generative Adversarial Networks (GANs)** to enable users to try on clothing digitally before purchasing. The model ensures a realistic and natural fit, preserving garment textures and user body alignment to improve the online shopping experience and reduce product return rates.

## Authors
```yaml
- Khushi Arora (22070126054)
- Khushin Vyas (22070126056)
- Paarth Chauhan (22070126069)
- Yashita Ughade (22070126135)
```

### Institution
```yaml
Symbiosis Institute of Technology
```

## Motivation
The rise of **e-commerce** in the fashion industry has provided convenience but lacks a real-world trial experience. Traditional size charts and static images fail to offer personalization, leading to uncertainty in fit and style. Virtual try-on solutions powered by **AI and GANs** provide an interactive and immersive shopping experience.

## Features
```yaml
- Realistic clothing visualization on user images
- Texture preservation for detailed garment appearance
- Pose estimation for accurate alignment
- GAN-based synthesis for high-resolution, photorealistic outputs
- User-friendly deployment via web applications (Flask, Gradio, Hugging Face Spaces)
```

## Dataset
The **VITON-HD dataset** (Kaggle) is used, comprising:
```yaml
- 13,679 frontal-view images of women in different outfits
- Pose annotations to help in accurate garment alignment
```

## Implementation
### 1. Data Pre-processing
```yaml
- Pose Estimation: Uses MoveNet to extract body keypoints (shoulders, elbows, waist, etc.)
- Background Removal: Gray-scaling and thresholding techniques eliminate unnecessary elements
- Cloth Masking: Morphological operations to extract garment shape
- Keypoint Extraction: Helps in warping and alignment for a natural fit
```

### 2. Alignment and Warping
```yaml
- Thin Plate Spline (TPS) Warping: Warps apparel images to align with body keypoints
```

### 3. GAN Model Training
```yaml
- Garment Warping & Refinement
- Texture & Detail Preservation
- GAN-Based Synthesis
- High-Resolution Output Generation
```

### 4. Try-On Condition Generator (HR-VITON)
```yaml
- Human Parsing & Pose Estimation
- Garment Warping Guidance
- Condition Map Creation
```

### 5. Visual Quality Enhancement
```yaml
- Super-Resolution GANs (SRGAN) for improved lighting and texture
- Edge enhancement & smoothing for seamless overlays
```

### 6. Deployment
```yaml
- Web Application using Flask/Gradio/Hugging Face Spaces
- User Interface: Allows users to upload images and select garments for try-on
- Performance Optimization for real-time inference
```

## Methodology Flowchart
![Vastra Screenshot](https://raw.githubusercontent.com/khushinvyas/Vastra-Virtual_Try_on/main/Screenshot%202025-03-26%20125643.png)


## Results
The system effectively generates **realistic virtual try-on experiences**, improving user engagement and online shopping efficiency. Experimental validation demonstrates its ability to align garments naturally while preserving textures and details.

## Future Work
```yaml
- Support for more garment types and accessories
- Real-time virtual try-on video implementation
- Better occlusion handling for complex poses
- Lower computational cost for faster inference
```

## References
A comprehensive list of references and related works is included in the full report.

---
For any questions or contributions, feel free to reach out!

