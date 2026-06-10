# ENPM673 Project 4: Panorama Image Stitching
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-blue)
![Feature%20Matching](https://img.shields.io/badge/Feature-Matching-green)
![Homography](https://img.shields.io/badge/Homography-RANSAC-orange)
![Python](https://img.shields.io/badge/Python-3.x-brightgreen)
## 🎯 Project Scope / Overview

This project develops a panorama image stitching system using computer vision techniques. The objective is to combine multiple overlapping images into a single panoramic image by identifying corresponding features, estimating geometric transformations, and aligning images within a common reference frame.

Two approaches are evaluated:

* OpenCV's built-in panorama stitching pipeline.
* A custom image stitching implementation developed from first principles.

The project demonstrates core concepts in feature matching, homography estimation, image warping, and panorama generation.

---

## 📋 Requirements

### Software

* Python 3.x
* Jupyter Notebook

### Libraries

```bash
pip install opencv-python numpy matplotlib
```

### Dataset

Place the input images inside the project image directory:

```text
ENPM673project4_images/
├── image1.jpg
├── image2.jpg
├── image3.jpg
└── ...
```

Images should contain sufficient overlap for successful feature matching and stitching.

---

## ⚙️ Setup

1. Clone or download the project files.
2. Install the required Python packages.
3. Place the dataset images in the designated image folder.
4. Open the notebook:

```bash
jupyter notebook project3_ymihrete.ipynb
```

---

## 🚀 Run / Pipeline

### OpenCV Stitching Pipeline

1. Load input images.
2. Initialize OpenCV's panorama stitcher.
3. Detect and match image features automatically.
4. Estimate image transformations.
5. Warp and blend images.
6. Generate final panorama output.

### Custom Stitching Pipeline

1. Load overlapping images.
2. Detect feature points.
3. Match features between image pairs.
4. Compute homography matrix.
5. Warp images into a common coordinate system.
6. Blend overlapping regions.
7. Generate final stitched panorama.

Output panoramas are displayed and saved for comparison.

---

## 📝 Notes

* Panorama quality depends heavily on image overlap and scene texture.
* Images with significant lighting changes, motion blur, or insufficient overlap may produce poor results.
* OpenCV's implementation generally produces smoother seams and more robust alignment than the custom pipeline.
* The custom implementation is intended to illustrate the underlying computer vision principles involved in panorama generation.

---

## 👤 Author

**Yafeit Mihrete**
ENPM673 – Perception for Autonomous Robots
