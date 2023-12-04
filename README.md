# Computer Vision

## Image Processing (TL;DR)

- Filters
  - Low pass Filters: 
    - Smoothing effect
    - `Averaging, median, gaussian blur`
  
  - High Pass:

- Thresholding:
  - Binarization of grayscale images.
  - `Simple Thresholding`: threshold manually set
  - `OSTU Thresholding`: thershold computed assuming image has bi-modal histogram such that the threshold value has minimum variance for the 2 peaks in histogram.
  - `Adaptive Thresholding`:
  
- Morphology:
  - close/open gaps betweem objects, mostly applied to binary images.
  
  - `erosion`: emoving small blobs in an image or disconnecting two connected objects. A foreground pixel in the input image will be kept only if all pixels inside the structuring element are > 0. Otherwise, the pixels are set to 0.

  - `dilation`: joining broken parts of an image together. Sets to white if ANY pixel in the structuring element is > 0.

  - `opening`: An opening is an erosion followed by a dilation. Allows us to remove small blobs from an image.
  - `closing`: The exact opposite to an opening would be a closing. A closing is a dilation followed by an erosion. 
  - `gradient`: A morphological gradient is the difference between a dilation and erosion. It is useful for determining the outline of a particular object of an image.
  - `white hat and black hat`: In ref.

## References:

- [Morphology](https://pyimagesearch.com/2021/04/28/opencv-morphological-operations/)
- [Convolutional neural networks for artistic style transfer](https://harishnarayanan.org/writing/artistic-style-transfer/)
