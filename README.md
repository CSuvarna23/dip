**MRI Denoising: Digital Image Processing (DIP)**
 
**Project Description**

This project focuses on the application of **Digital Image Processing (DIP)** techniques for **denoising MRI (Magnetic Resonance Imaging)** scans. The goal is to reduce the effects of noise and improve the quality of MRI images, which is crucial for medical professionals who rely on accurate imaging for diagnoses. We apply various **denoising filters** to the MRI scans and evaluate their effectiveness using standard image quality metrics: **PSNR (Peak Signal-to-Noise Ratio)**, **SSIM (Structural Similarity Index Measure)**, and **MSE (Mean Squared Error)**.

The key aim is to simulate **real-world MRI noise** and apply different image restoration methods to recover a clean version of the image while preserving essential details that are important for medical analysis.

---

## Problem Statement

MRI images are often degraded by noise, either from the scanning process or external interferences. This noise can reduce the accuracy and reliability of medical diagnoses. Specifically, in lower-quality or older scanners, noise becomes more prominent. By applying denoising techniques, we aim to improve the clarity and resolution of these images, ensuring that radiologists and healthcare providers can make better-informed decisions.

---

## 🚀 Real-World Relevance

* 🏥 **Medical Imaging Quality Improvement**: Ensures that MRI scans are clear, allowing better diagnosis of conditions such as brain tumors, spinal cord injuries, etc.
* 🚑 **Enhances Radiology Workflow**: Reduces the time radiologists spend dealing with noisy images, helping them focus on diagnosing.
* 🧑‍⚕️ **Reduces Image Artifacts**: Denoising minimizes the visual artifacts caused by MRI scanners, leading to more reliable results.
* 💡 **Advancement of Medical Research**: By improving MRI imaging, researchers can obtain more precise data for understanding diseases and developing treatments.

---

## 🪨 Dataset Used

The images used in this project are **MRI scans** that have been sourced from publicly available datasets, such as those provided by medical imaging repositories. These images are corrupted with noise (simulating real-world scanning artifacts) to test the effectiveness of the denoising techniques. Various levels of noise are introduced to replicate the types of distortions seen in actual MRI scans.

---

## 🔧 Technologies Used

* **Python 3.x**: The primary programming language used to implement the solution.
* **OpenCV**: For image processing and applying denoising filters.
* **NumPy**: For handling and manipulating image data arrays.
* **scikit-image**: For additional image processing functions, including denoising and quality metrics (PSNR, SSIM).
* **Streamlit**: For building an interactive user interface (UI) to showcase the denoising techniques and results.
* **Pillow**: For image manipulation and saving denoised results.

---

## 🔢 Techniques Implemented

The following denoising techniques were implemented and tested in the project:

* **Gaussian Filter**: A basic filter used to smooth the image and reduce noise.
* **Total Variation (TV) Denoising**: A regularization method aimed at reducing noise while preserving image edges.
* **Non-Local Means (NLM)**: A powerful denoising technique based on the self-similarity of image patches.
* **Bilateral Filter**: A filter that smooths images while preserving edges.
* **Hybrid Filters**: A combination of two denoising techniques applied in succession, such as **Median + NLM** and **Bilateral + Wavelet**.

---

## 📷 Output Preview

### Original and Noisy Images

Below are the original and noisy MRI images that serve as input for the denoising methods:

* **Original Image**:
  ![Original MRI Image](results/original_mri_image.png)

* **Noisy Image**:
  ![Noisy MRI Image](results/noisy_mri_image.png)

### Denoised Images (Grid)

Here is a grid showing the results of various denoising techniques applied to the noisy image:

* **Gaussian Filter**:
  ![Gaussian Filter Result](results/gaussian_denoised.png)

* **Total Variation Denoising**:
  ![TV Denoising Result](results/tv_denoised.png)

* **Non-Local Means (NLM)**:
  ![NLM Denoising Result](results/nlm_denoised.png)

---

## 📊 Evaluation Results

The effectiveness of each denoising technique is evaluated using three common image quality metrics: **MSE (Mean Squared Error)**, **PSNR (Peak Signal-to-Noise Ratio)**, and **SSIM (Structural Similarity Index)**. Below are the results for each technique:

### 📊 Performance Evaluation

| Method                    | MSE    | PSNR (dB) | SSIM   |
| ------------------------- | ------ | --------- | ------ |
| **Gaussian Filter**       | 0.0074 | 21.31     | 0.4180 |
| **Total Variation (TV)**  | 0.0070 | 21.54     | 0.3555 |
| **Non-Local Means (NLM)** | 0.0033 | 24.86     | 0.5740 |

* **MSE (Mean Squared Error)**: Lower values are better. Indicates the overall difference between the original and denoised images.
* **PSNR (Peak Signal-to-Noise Ratio)**: Higher values indicate better denoising performance.
* **SSIM (Structural Similarity Index)**: Closer to 1 means better preservation of the image structure.

From the table above, we can conclude that **Non-Local Means (NLM)** provides the best performance in terms of both PSNR and SSIM.

---

## 📂 Project Structure

```plaintext
MRI-Denoising/
├── images/
│   ├── original_mri_image.jpg
│   └── noisy_mri_image.jpg
├── results/
│   ├── gaussian_denoised.png
│   ├── tv_denoised.png
│   ├── nlm_denoised.png
│   └── evaluation_results.csv
├── app.py
├── denoise.py
├── README.md
└── requirements.txt
```

---

## 🔄 How to Run

To run this project locally, follow these steps:

1. **Clone the repository**:

   ```bash
   git clone https://github.com/your-username/MRI-Denoising.git
   ```

2. **Navigate to the project folder**:

   ```bash
   cd MRI-Denoising
   ```

3. **Install the required dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the app**:

   ```bash
   streamlit run app.py
   ```

   This will open the app in your browser, where you can upload an MRI image, apply denoising filters, and evaluate the results.

---

## 👨‍💼 Team Members

* **Jeswin Lobo (4SO22CD023)**

  * 📧 Email: [22j23.jeswin@sjec.ac.in](mailto:22j23.jeswin@sjec.ac.in)
  * 👤 GitHub: [Jeswin2003lobo](https://github.com/Jeswin2003lobo)

* **Shashank Rao U (4SO22CD046)**

  * 📧 Email: [22j46.shashank@sjec.ac.in](mailto:22j46.shashank@sjec.ac.in)
  * 👤 GitHub: [Shashankraou](https://github.com/Shashankraou)

---

## 📝 License

This project is licensed under the **MIT License**.

---

## 🚧 Acknowledgments

Special thanks to the following libraries and resources:

* [scikit-image](https://scikit-image.org/)
* [OpenCV](https://opencv.org/)
* [Streamlit](https://streamlit.io/)
* [NumPy](https://numpy.org/)
* [Pillow](https://python-pillow.org/)
# dip
