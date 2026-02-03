**Image Blurring: Spatial vs Frequency Domain**

**Overview**

This project demonstrates that image blurring using spatial convolution produces the same result as applying the equivalent filter in the Fourier domain, confirming the Convolution Theorem.

**Method**

A Gaussian kernel is used for blurring.

Spatial filtering is performed using cv2.filter2D.

Frequency filtering is performed by:

Zero-padding the image and kernel

Flipping the kernel to perform convolution

Applying FFT, multiplying spectra, and using inverse FFT

Cropping to the original image size

**Key Idea**
F(f * h) = F(f) * F(h)

Convolution in the spatial domain is equivalent to multiplication in the frequency domain.

**Result**

The spatial and frequency-domain outputs are visually identical.
The maximum difference is very small

Run the code:
1. Download the code into notebook.
2. Input the image into the same folder. 

**Conclusion**

This confirms that spatial convolution and frequency-domain multiplication are equivalent ways to perform image blurring.
