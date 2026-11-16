# Satellite-Image-Enhancement-Using-CLAHE-project

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

## Output Images

The `CLAHE_Results` folder contains:

  -----------------------------------------------------------------------
  File                                Description
  ----------------------------------- -----------------------------------
  `01_Original_Image.png`             Original input satellite image

  `02_Grayscale_Image.png`            Grayscale version of the input

  `03_Histogram_Equalization.png`     Result after global Histogram
                                      Equalization

  `04_Grayscale_CLAHE.png`            Result after grayscale CLAHE

  `05_Color_CLAHE_Enhanced.png`       Color-preserved CLAHE result using
                                      LAB color space

  `06_Original_Histogram.png`         Histogram of the original grayscale
                                      image

  `07_HE_Histogram.png`               Histogram after Histogram
                                      Equalization

  `08_CLAHE_Histogram.png`            Histogram after grayscale CLAHE
  -----------------------------------------------------------------------

## Evaluation

The script calculates: - **Contrast:** Standard deviation of image
intensity values (`std2`). - **Entropy:** Information content of the
grayscale image (`entropy`).

The contrast and entropy comparison is calculated for the original
grayscale image, Histogram Equalization result, and grayscale CLAHE
result.

## Notes

-   The color CLAHE method enhances only the L (luminance) channel in
    LAB color space; the A and B color channels are retained.
-   A new results folder is created for each run (for example,
    `CLAHE_Results`, `CLAHE_Results_1`, `CLAHE_Results_2`) so previous
    outputs are not overwritten.
-   Enhancement results depend on the selected input image.
