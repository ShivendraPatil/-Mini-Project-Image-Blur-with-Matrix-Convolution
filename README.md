# Mini Project: Image Blur with Matrix Convolution

This mini project is a simple introduction to how convolution works in computer vision and deep learning (e.g., CNNs).

It shows how to:

- Represent a small grayscale image as a NumPy matrix.
- Apply a 3×3 blur kernel using **manual convolution**.
- Visualize the original and blurred images with Matplotlib.

---

## Learning Outcomes

After completing this mini project, you (or your students) will be able to:

1. Represent a grayscale image as a 2D NumPy array (matrix of pixel values).
2. Create and understand a 3×3 blur kernel (average filter) using `np.ones` and division.
3. Implement a **manual 2D convolution**:
   - Extract 3×3 patches using slicing.
   - Do elementwise multiply and sum with `np.sum(patch * kernel)`.
4. Correctly calculate convolution output shape:
   - For image `(H, W)` and kernel `(kH, kW)`, output is `(H - kH + 1, W - kW + 1)` in valid mode (no padding).
5. Visually compare original and blurred images using `matplotlib.pyplot.imshow`.
6. Explain in simple words:
   - What a kernel/filter is.
   - How sliding a kernel over an image relates to **convolutional neural networks (CNNs)**.
7. Build intuition that:
   - Images = matrices  
   - Filters = small matrices  
   - Convolution = local feature extraction (basis of many vision and Gen AI models).

---

## How It Works

- **Image** = 2D matrix of pixel intensities (grayscale values, e.g. 0–255).
- **Kernel (filter)** = small matrix (here 3×3) that slides over the image.
- **Convolution** = for each position:
  - Take a local 3×3 patch from the image.
  - Multiply elementwise with the kernel.
  - Sum all values → one blurred pixel.
- **Average kernel** → smooths out differences between neighboring pixels → blur / smoothing effect.

Key ideas:

- Image = 2D matrix of pixel intensities  
- Kernel (filter) = small matrix that slides over the image  
- Convolution = elementwise multiply + sum over each local patch  
- Average kernel → blur / smoothing  

---

## File

- `image_blur_convolution.py` – main script for this mini project.

---

## How to Run

From the project folder:

python image_blur_convolution.py
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

This will:

- Print the original 5×5 image and the 3×3 blurred output in the terminal.

- Open a Matplotlib window showing:

- Left: original image (5×5)

- Right: blurred image (3×3) after valid convolution.

- 
<img width="922" height="439" alt="Screenshot 2025-11-20 125402" src="https://github.com/user-attachments/assets/01de8d92-8771-4af1-ad61-ba284a24ff91" />

