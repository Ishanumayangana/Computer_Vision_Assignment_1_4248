# 🧠 Computer Vision and Image Processing - Assignment_1

This project explores **grayscale transformations**, **blurring**, **rotations**, and **block-wise resolution reduction**, using Python, OpenCV, and Google Colab.

---

## 📌 Project Objectives

Implement the following four key image processing tasks:

1. **Intensity Level Reduction**  
2. **Spatial Averaging (Blurring)**  
3. **Image Rotation**  
4. **Block-wise Spatial Resolution Reduction**

All outputs are visually compared side-by-side with the original grayscale image.

---

## 🧪 Technologies Used

- **Python 3** (Colab Notebook)
- **OpenCV (cv2)** – Core image operations
- **NumPy** – Numerical computing
- **Matplotlib** – Image visualization
- **ipywidgets** – Interactive UI (e.g., sliders, dropdowns)
- **PIL (Pillow)** – Image saving
- **Google Colab** – Platform for execution

---

## 🔍 Task Details and Outputs

### 🎯 Task 1: Intensity Level Reduction

**Goal**: Reduce grayscale intensity levels from 256 to a power of 2 (e.g., 2, 4, 8, ..., 256).

**How**:
- Pixel values are quantized based on the selected level.
- An interactive **dropdown widget** allows choose the desired intensity level.
  
**Output**:
- Side-by-side visualization (original vs reduced).

---

### 🎯 Task 2: Spatial Averaging (Blurring)

**Goal**: Apply spatial averaging (mean filtering) to smooth images.

**How**:
- Uses OpenCV’s `cv2.blur()` with different kernel sizes:
  - 3×3
  - 10×10
  - 20×20

**Output**:
- Visual comparison of original and blurred versions.
- Output files:
  - `gray_avg_3x3.png`
  - `gray_avg_10x10.png`
  - `gray_avg_20x20.png`

---

### 🎯 Task 3: Image Rotation

**Goal**: Rotate the image by specific angles: **45° and 90°**.

**How**:
- OpenCV’s `getRotationMatrix2D()` creates the transformation matrix.
- `cv2.warpAffine()` applies rotation around the image center.

**Output**:
- Side-by-side view of original and rotated versions.
- Output files:
  - `gray_rotated_45.png`
  - `gray_rotated_90.png`

---

### 🎯 Task 4: Block-wise Spatial Resolution Reduction

**Goal**: Simulate lower spatial resolution by averaging blocks of pixels.

**How**:
- Each non-overlapping block (3×3, 5×5, 7×7) is averaged.
- The block's average replaces all pixels in the block.

**Output**:
- Pixelated-style comparison (original vs block-averaged).
- Output files:
  - `gray_block_avg_3x3.png`
  - `gray_block_avg_5x5.png`
  - `gray_block_avg_7x7.png`

---

## ⚙️ Instructions for Use (Colab)

1. **Open the Notebook** in Google Colab.
2. **Upload an Image** when prompted.
3. Each section is **independent and interactive**.
4. Adjust values using sliders or dropdowns (e.g., intensity levels).

