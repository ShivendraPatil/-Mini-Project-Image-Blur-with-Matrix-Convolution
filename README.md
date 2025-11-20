# -Mini-Project-Image-Blur-with-Matrix-Convolution
This is a simple introduction to how convolution works in computer vision and deep learning (e.g., CNNs).

This project shows how to represent a small grayscale image as a NumPy matrix and
apply a 3×3 blur kernel using manual convolution. It then visualizes the original
and blurred images with Matplotlib.

**Run:**

python image_blur_convolution.py

Key ideas:
Image = 2D matrix of pixel intensities


Kernel (filter) = small matrix that slides over the image


Convolution = elementwise multiply + sum over each local patch


Average kernel → blur / smoothing
<img width="922" height="439" alt="Screenshot 2025-11-20 125402" src="https://github.com/user-attachments/assets/01de8d92-8771-4af1-ad61-ba284a24ff91" />

