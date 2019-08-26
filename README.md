# image_transform_cpp

The purpose of this project is to use cpp to perform basic image transformation actions.
Utilizing AWS Cloud9 IDE, we do not need to worry about local environment setup.

This program takes an image as input, in this case the image is named alma.png.
We then perform below actions:

1. Grayscale
   Set saturation for each pixel to be 0% will result in a gray pixel.
   
2. "Fall filter"
   Apply a fall filter to the image, transform hue of each pixel to Illini Orange(11) or Illini Blue(216).
   The hue of each pixel should be set to one or the other of these two hue values, based on the closeness to these two values.
   
3. Spotlight
   To spotlight an image is the create a spotlight pattern centered at a given point.
   The spotlight adjusts the illumimance of the pixel based on its distance to the given point. The illuminance is decreased by 0.5% per 1 pixel unit of Euclidean distance, up to an 80% decrease in luminance at most.
   
4. Add on watermark
  To watermark an image is to lighten a region of it based on the content of another image that acts as a stencil.
  Assume that the images are positioned in such way that their upper-left corners overlapping at the same coordinates.
  For every pixel that exists within the bounds of both base and stencil images, the luminance of the base image should be increased by 0.2 but not exceeding 1.0.


Backgrounds:
  Understanding color spaces and HSLAPixel
