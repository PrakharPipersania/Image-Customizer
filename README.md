# Image Customizer
Image Customizer can manipulation or altering a photograph using various methods and techniques to achieve desired results. It can be used to adjust the geometry of the image like rotating and cropping, sharpening or softening the image, making color changes or adding special effects to the image.

## Features
* RGB Image to GrayScale Image
* RGB Image to Negative Image
* Brighten & Darken Image
* Flip Image Horizontally & Vertical
* Rotate Image 90 Degree
* Crop Image
* Overlay Images
* Resizeing Image Using Bilinear Interpolation
* Apply Filter on Images 
</br>->Mean Filter
</br>->Gaussian Filter
</br>->Reflect Filter
</br>->Sharpen Filter
</br>->Laplacian Filter
</br>->Sobel Filter (Gx & Gy)
* Custom ( NxN  where N is odd) Filters can also be Applied

## Formulas Used:
* RGB Image to GrayScale Image
</br>
i)Average Method
</br>Grayscale = (R + G + B / 3)
</br>
ii)Weighted Method
</br>Grayscale = ((0.3 * R)+(0.59 * G)+(0.11 * B))
* RGB Image to Negative Image
Negative = (255-R,255-G,255-B)
* RGB Image to Brighten Image
Brighten Image =(R+Brightness,G+Brightness,B+Brightness)
* RGB Image to Darken Image
Darken Image =(R-Darkness,G-Darkness,B-Darkness)
* [Bilinear Interpolation](https://en.wikipedia.org/wiki/Bilinear_interpolation) 
### All Defined Filters are 3x3
* Mean Filter = [[1,1,1],[1,1,1],[1,1,1]]
* Gaussian Filter = [[1,2,1],[2,4,2],[1,2,1]]
* Reflect Filter = [[-1,0,0],[0,1,0],[0,0,1]]
* Sharpen Filter = [[-1,-1,-1],[-1,9,-1],[-1,-1,-1]]
* Laplacian Filter = [[0,-1,0],[-1,4,-1],[0,-1,0]]
* Sobel Gx Filter = [[-1,0,1],[-2,0,2],[-1,0,1]]
* Sobel Gy Filter = [[-1,-2,-1],[0,0,0],[1,2,1]]

## [Implementation & Output](https://github.com/PrakharPipersania/Image-Customizer/blob/main/Image%20Customizer.ipynb)