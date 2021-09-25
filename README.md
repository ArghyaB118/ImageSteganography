# Image Steganography
### Steganipraghic attacks are common on systems, networks, and communities
You have an image or any other media, which seems naive and not at all malicious.
However, some other recipient extracted a hidden message from the seemingly innocuous media.

## Inspiration

With the boom of online education and business in the post-pandemic era, a huge amont of data transfer is happening among students and professionals.
Media files are being transferred among large networks with millions of users and it hard to monitor all the large media contents.
With the onset of serious security issues faced in the last few decades, media abuse has been one of the severe concerns.
Hidden messages are transferred Hidden messages are transferred through media using steganography. It's difficult, almost impossible to trace back to the origin of a viral image that is seemingly innocuous but may contain a hidden malicious message parsed inside.media using steganography. 
Steganography has been in use for the last two decades in major terrorist attacks such as 9/11 or Paris attack.
It's difficult, in fact, almost impossible to trace back to the origin of a viral image that is seemingly innocuous but may contain a hidden malicious message parsed inside.
Hence, students and professionals are acting as a carrier of malicious messages unknowingly.
It's important to read any such message hidden in media contents locally and at a network administrator level.

## What it does

We contribute in two levels.
We show how malicious media contents (such as images) can be generated that has hidden message inside.
We provide a solution to decode such hidden messages.

## How we built it

We created a malicious image encoding (hiding) a text message inside an RGB image.
We only use the LSBs of certain pixels of the image. 
These pixels are chosen in a way that they belong to a portion of the image where the pixels are highly dissimilar.
Hence, it is very unlikely to locate these changes at pixel level visually.


## Challenges we ran into

The main challenges were two fold. One was mathematical in the sense that encoding has to be in the pixel level. 
That too, in such granularity that it is impossible to understand visually that the image is morphed.
We solved it by only altering the least significant bits (LSBs) of the binary values of the pixels.
The second challenge was coding wise.
We wanted to implement both the encoding and the decoding processes. 
Although, the decoder does not know any details about the particular pixels where the message is hidden.
We used a dissimilarity measure based encoding: only the central pixel of a highly dissimilar box is contains an encoded message.

## Accomplishments that we're proud of

The implementation has a cool way to alter only the LSBs.
It ensures that the encoded image is visually absolutely similar to the original image.

## What we learned

Security is a very serious issue, be it in a system or a network, a community etc.
We need customized softwares to find any hidden encoded message in any media content.

## What's next for Steganography Attack

1. High hiding capacity
2. Better encryption
3. Using diverse filesystems to hide the message in
