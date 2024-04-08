# LeafDetection

Place PNG images in the directory: Put the images you want to process (e.g., plant001.png, plant002.png, etc.) in the same directory as the code file.

Run the code: Execute the MATLAB script. It will process all PNG images in the directory and create corresponding output images.

1. Image Preprocessing:
- Sharpens the image.
- Applies Gaussian filtering.
- Converts the image to HSV color space.
- Extracts greenness information.
2. Thresholding and Binarization:
- Thresholds the Value (V) channel based on greeness.
- Performs Otsu's binarization.
- Retains the largest connected component.
3. Segmentation:
- Applies Canny edge detection.
- Integrates edges into the binary image.
- Uses morphological opening to remove noise.
- Performs watershed segmentation to separate overlapping leaves.
4. Labeling and Colorization:
- Labels individual leaves using bwlabel.
- Segments each leaf and assigns a random color.
5. Output:
- Displays intermediate results as subplots.
- Saves the final colorized image with highlighted leaves.
