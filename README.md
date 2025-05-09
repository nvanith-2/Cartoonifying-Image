# 🖼️ Cartoonizer with OpenCV and KMeans

**By Nagapuri Vanitha**

---

## 🎯 Motivation

I chose the task of cartoonizing images because it lies at the intersection of artistic creativity and computational efficiency. The idea of transforming realistic images into cartoon-style visuals using simple yet powerful image processing techniques is fascinating — especially given how this can be done without deep learning. It serves as a great introduction to computer vision and unsupervised learning, making it approachable for learners and still useful in practical applications like stylized filters and AR effects.

---

## 🧠 Multimodal Learning: Historical Context

Multimodal learning integrates data from multiple sources or modalities — such as images, text, and audio — to create more holistic models. While cartoonization itself is single-modality (vision), the evolution of image understanding plays a key role in multimodal applications. Traditional image processing techniques like edge detection and color clustering formed the foundation before the deep learning wave.

Recently, deep learning models like **StyleGAN**, **CycleGAN**, and **DALL·E** have pushed the boundaries of image transformation and generation. However, lightweight techniques like the one used here remain valuable for:

* Real-time applications on constrained devices.
* Explainability in educational tools.
* Preprocessing for multimodal pipelines.

This work connects with the roots of image stylization and serves as a bridge toward more advanced multimodal creativity.

---

## 📘 Learnings

From this project, I learned:

* How to combine classical computer vision techniques (edge detection, bilateral filtering) with clustering (KMeans) to simulate cartoon-like effects.
* The importance of color space conversions in OpenCV and how RGB/BGR inconsistencies can affect output.
* That effective visual output doesn't always require deep neural networks — sometimes, simple pipelines produce surprisingly good results.

---

## 💻 Code and Visuals

Here's a high-level overview of the process used in the code:

### 📟 Steps:

1. **Read and preprocess the image** (`rock3.png`).
2. **Edge Detection** using grayscale conversion, median blur, and adaptive threshold.
3. **Color Quantization** via KMeans clustering to reduce the number of colors.
4. **Smoothing** using bilateral filtering.
5. **Combining** edges with the smoothed image to get a cartoon effect.

### 📊 Sample Outputs:

| Original Image | Cartoonized Output |
| -------------- | ------------------ |
|                |                    |

> Note: Outputs are saved automatically in the script as `cartoon.png`.

### 📁 How to Run

1. Clone the repository and install dependencies:

```bash
pip install -r requirements.txt
```

2. Run the script:

```bash
python cartoonizer.py
```

---

## 🤔 Reflections

### (a) What surprised me?

* The effectiveness of classical techniques — especially how edge masks and color quantization alone can produce stylized results.
* The simplicity and speed of KMeans color clustering for image segmentation.

### (b) Scope for Improvement

* Add GUI slider controls to let users adjust parameters in real-time.
* Extend the pipeline to video input.
* Use histogram-based clustering for more perceptually aware color grouping.
* Add deep learning alternatives for comparison.

---

Thank you for checking out this project!
If you enjoyed it or have suggestions, feel free to open an issue or contribute.
