# FrequencySpatialEnhancement
# Image Restoration and Optical Deciphering

Enhancing Newspaper Photos and Decoding Noisy Number Plates with Frequency Filters and Spatial Techniques

## Introduction

This project focuses on enhancing newspaper photos and decoding noisy number plates using image processing techniques. The main goal is to improve the visibility of license plates in noisy images and extract useful information from them. By applying frequency filters and spatial techniques, we can enhance the quality of the images and make the license plates more readable.

## Project Steps

1. Read the image as a grayscale image: Convert the input image to grayscale to simplify the image processing tasks.

2. Calculate the Discrete Fourier Transform (DFT) of the image: Apply the 2D DFT using the Fast Fourier Transform (FFT) algorithm to decompose the image into its constituent frequencies.

3. Shift the origin of the image domain to the center and calculate the magnitude of the Fourier transform: Shift the Fourier transform so that the center of the frequency domain corresponds to the zero frequency. Calculate the magnitude spectrum of the shifted Fourier transform and apply a logarithmic transformation to make it more visible.

4. Identify periodic noise in the Fourier domain: Locate the white peaks in the magnitude spectrum that capture periodic noise present in the original image.

5. Clean the image in the Fourier domain: Remove the periodic noise by setting the surrounding frequency components to zero, except for a single bright "star" in the center of the magnitude spectrum.

6. Perform inverse Fourier transform: Apply the inverse Fourier transform to obtain the filtered image.

7. Slice the image to extract the number plate region: Focus on the region of interest containing the license plate for further processing.

8. Apply a Gaussian filter: Use a low-pass Gaussian filter to eliminate localized noise in the number plate region.

9. Apply gamma correction to improve contrast: Adjust the intensity values of the image to enhance the visibility of dark and bright areas.

10. Normalize the image: Stretch the contrast of the image to utilize the full dynamic range and improve visual quality.

## Findings

After applying the image processing techniques, the number plate region becomes clearer and more legible. However, further improvements may be required to achieve complete readability.

## Applications

The techniques used in this project have potential applications in various fields, including traffic surveillance, law enforcement, and parking management. By enhancing newspaper photos and improving the visibility of license plates, valuable information can be extracted for identification and analysis purposes.

## Conclusion

The project demonstrates the effectiveness of frequency filters and spatial techniques in enhancing newspaper photos and decoding noisy number plates. By applying these techniques, it becomes possible to improve image quality, extract important information, and make previously unreadable license plates more legible.

Thank you for reading!

If you like my work and want to support me, you can follow me on [Medium](https://patel-prakhar09.medium.com/) and [LinkedIn](https://www.linkedin.com/in/prakhar0927/).

If you want to understand better read my medium blog on [Enhancing Newspaper Photos and Decoding Noisy Number Plates with Frequency Filters and Spatial Techniques](https://patel-prakhar09.medium.com/enhancing-newspaper-photos-and-decoding-noisy-number-plates-with-frequency-filters-and-spatial-47ef9cd9540d)




