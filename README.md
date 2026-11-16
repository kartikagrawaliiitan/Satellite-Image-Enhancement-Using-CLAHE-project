# Satellite Image Enhancement Using CLAHE

## Project Description

This MATLAB project enhances satellite images using Histogram
Equalization (HE) and Contrast Limited Adaptive Histogram Equalization
(CLAHE). It also applies CLAHE to the luminance channel in LAB color
space to produce an enhanced image while preserving its original colors.

## Requirements

-   MATLAB
-   Image Processing Toolbox

## How to Run

1.  Open the MATLAB `.m` project code.
2.  Run the script.
3.  Select an RGB or grayscale satellite image when the file-selection
    window appears.
4.  The program displays the original and enhanced images and their
    histograms.
5.  Results are automatically saved in a new output folder beside the
    selected image.

## Results

The program generates the following image outputs:

  -----------------------------------------------------------------------
  Output file                         Result
  ----------------------------------- -----------------------------------
  `01_Original_Image.png`             Original satellite image

  `02_Grayscale_Image.png`            Grayscale input image

  `03_Histogram_Equalization.png`     Global Histogram Equalization
                                      result

  `04_Grayscale_CLAHE.png`            Grayscale CLAHE result

  `05_Color_CLAHE_Enhanced.png`       Color-preserving CLAHE result using
                                      LAB color space
  -----------------------------------------------------------------------

### Image Results

The following previews are displayed when the generated image files are
stored in the `CLAHE_Results` folder alongside this README.

**1. Original Satellite Image**

![Original satellite image](CLAHE_Results/01_Original_Image.png)

**2. Grayscale Image**

![Grayscale satellite image](CLAHE_Results/02_Grayscale_Image.png)

**3. Histogram Equalization Result**

![Histogram Equalization
result](CLAHE_Results/03_Histogram_Equalization.png)

**4. Grayscale CLAHE Result**

![Grayscale CLAHE result](CLAHE_Results/04_Grayscale_CLAHE.png)

**5. Color CLAHE Enhanced Result**

![Color CLAHE enhanced satellite
image](CLAHE_Results/05_Color_CLAHE_Enhanced.png)

### Histogram Results

**Original Image Histogram**

![Original image histogram](CLAHE_Results/06_Original_Histogram.png)

**Histogram Equalization Histogram**

![Histogram Equalization histogram](CLAHE_Results/07_HE_Histogram.png)

**CLAHE Histogram**

![CLAHE histogram](CLAHE_Results/08_CLAHE_Histogram.png)

## Output Files

The `CLAHE_Results` folder contains the five processed/original images
and three histogram images listed above.

## Evaluation

The script calculates: - **Contrast:** Standard deviation of image
intensity values using `std2`. - **Entropy:** Information content of the
grayscale image using `entropy`.

The contrast and entropy comparison is calculated for the original
grayscale image, Histogram Equalization result, and grayscale CLAHE
result. The color CLAHE output is currently included as a visual result
and is not included in these numerical calculations.

## Notes

-   The color CLAHE method enhances only the L (luminance) channel in
    LAB color space; the A and B color channels are retained.
-   A new results folder is created for each run (for example,
    `CLAHE_Results`, `CLAHE_Results_1`, `CLAHE_Results_2`) so previous
    outputs are not overwritten.
-   The image previews above require the corresponding PNG files to be
    present at the specified relative paths. If a run creates
    `CLAHE_Results_1` or another numbered folder, update the image paths
    to match that folder.
-   Enhancement results depend on the selected input image.
