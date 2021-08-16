# "PBS" filter
PBS (pansharpening with background subtraction) method for sharpening RGB images

1. Read image, wavelet denoise, and convert to HSV
2. Do 'inverted background subtraction' on the V channel
3. combine with HS, convert to RGB

The effect is to sharpen details of object boundaries/transitions, brighten, and recolour

But without changing the overall distribution of values within the image (i.e. the range), and recolouring in an internally consistent (deterministic) way

![](PBS.jpg)
