## Contents from the first class:
1. Learn about RGB, grayscale image
2. Difference between 8-bit and 16-bit image
3. The Spectral Analysis
4. Image Enhancement: Convertion of image( 8bit to 16bit)
5. Infra-layer, hyper-spractal image


The assignment: Layer-wise image print
What i have done:
- Loaded images using both Pillow (PIL) and OpenCV
  -- Used Image.open() and cv2.imread() to read images.
  -- Understood the difference between RGB (Pillow) and BGR (OpenCV).
- Converted images to NumPy arrays
  -- Used np.array(img) to analyze raw pixel data.
- Checked image bit depth (8-bit vs. 16-bit) via dtype.
- Extracted individual RGB channels
- Compared grayscale vs. RGB-colored visualizations of single channels for better understanding.
