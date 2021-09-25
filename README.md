# Image Steganography
### Steganipraghic attacks are common on systems, networks, and communities
You have an image or any other media, which seems naive and not at all malicious.
However, some other recipient extracted a hidden message from the seemingly innocuous media.

## Method
This jupyter notebook explains how to encode a message in an RGB image file in the LSBs of some pixels.
These pixels are chosen in a way that they belong to a portion of the image where the contrast is high.
Hence, it is very unlikely to locate these changes at pixel level visually.

## How to stay safe
You do not want to forward such media and take part in such malicious activity unknowingly.
We provide a method to detect if an image has any such hidden messages in the LSBs.
