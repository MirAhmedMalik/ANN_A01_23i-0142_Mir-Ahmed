***Neural Style Transfer (ANN Project)***

This project shows how Artificial Neural Networks (ANN) can create artistic images.

It takes:

 .A Content Image (normal photo)
 .A Style Image (painting/art)

 -And combines them to generate a new stylish image.

**How It Works**
We use a pre-trained model called VGG-19.
It helps the system understand:
Content → shapes and objects in the photo
Style → colors and textures of the painting
Then we:
Start with a random image
Slowly improve it using gradient descent
Make it look like the content + style together

**Loss Functions**

The model improves the image using these:

Content Loss → keeps the main structure of the photo
Style Loss → adds artistic textures and colors
Perceptual Loss → makes the image look more realistic and artistic
MSE → basic error (not very good for art)

**How We Check Results**

We use simple measures to check quality:

FID → checks how real the generated art looks
SSIM → checks if shapes are still clear
PSNR → checks image quality and noise
 Key Points
Perceptual Loss gives better artistic results
VGG-19 works very well for this task
FID is best for checking realism
