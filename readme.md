# Computer Vision Mini Project

## 📌 Project Overview
This mini project explores key computer vision techniques for feature detection, matching, and corner detection. Implementations include:
- **SIFT (Scale-Invariant Feature Transform)**
- **RANSAC (Random Sample Consensus)**
- **Shi-Tomasi Corner Detection**

---

## 📸 Algorithms Implemented

### 1. 🔍 SIFT Algorithm
**Aim:** Detect and match keypoints between two images using the SIFT algorithm.

#### 🔎 Observations:
- **Limited Features & High Contrast Threshold:** Reduced the number of detected keypoints, especially in low-contrast areas, but prioritized more prominent features and improved performance.
- **Higher Edge Threshold:** Reduced false keypoints near textured borders, improving match robustness.
- **Increased Sigma:** Allowed detection of more scale-invariant features but missed finer texture-level details.

---

### 2. 🔧 RANSAC
**Aim:** Filter out outliers from keypoint matches and fit a transformation model.

#### 🔎 Observations:
- **Threshold = 2.0:** Strict matching, fewer inliers but reduced outliers effectively.
- **Threshold = 10.0:** Lenient matching, included more false matches.
- **Threshold = 5.0:** Balanced result with good accuracy and adequate match count.

---

### 3. 🟨 Shi-Tomasi Corner Detector
**Aim:** Identify and mark corner points in the image.

#### 🔎 Observations:
- **Default Parameters:** Detected a well-distributed set of corners with good balance.
- **Lower Distance, Higher Cap:** Detected more fine details, but increased chances of unstable keypoints.
- **High Quality Level:** Only strong corners retained, resulting in more reliable and distinct feature tracking.

---

## 🧪 Conclusion
This project demonstrates the effectiveness of feature detection and matching algorithms in computer vision. By tuning parameters:
- **SIFT** helps in detecting scale- and rotation-invariant keypoints.
- **RANSAC** effectively refines matches by removing outliers and improving geometric accuracy.
- **Shi-Tomasi** is excellent for corner detection and can be adjusted to balance between clarity and detail.

Each method has trade-offs between accuracy, speed, and robustness. Understanding these techniques and their parameters is critical for designing reliable CV systems in real-world applications.

---

## 🖼️ Sample Output Screenshots
*(Please refer to the notebook or PDF for actual visual outputs.)*

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/Prathmesh2011/Computer-Vision-Assignment.git
