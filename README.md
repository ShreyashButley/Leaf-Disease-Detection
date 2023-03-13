# Abstract:
Identification of the plant diseases is the key to prevent the losses in the yield and 
quantity of the agricultural product. The studies of the plant diseases mean the 
studies of visually observable patterns seen on the plant. Health monitoring and 
disease detection on plants is very critical for sustainable agriculture. It is very 
difficult to monitor the plant diseases manually. 

Step 1: Image acquisition is the very first step that requires capturing an image 
with the help of a digital camera. <br />
Step 2: Pre-processing of input image to improve the quality of image and to 
remove the undesired distortion from the image. Clipping of the leaf image is 
performed to get the interested image region and then image smoothing is 
done using the smoothing filter. To increase the contrast, Image enhancement 
is also done. <br />
Step 3: Mostly green colored pixels, in this step, are masked. In this, we 
computed a threshold value that is used for these pixels. Then in the following 
way mostly green pixels are masked: if pixel intensity of the green component
is less than the pre-computed threshold value, then zero value is assigned to 
the red, green, and blue components of this pixel. <br />
Step 4: In the infected clusters, inside the boundaries, remove the masked 
cells. <br />
Step 5: Obtain the useful segments to classify the leaf diseases. Segment the 
components using the ML algorithm <br />

# output 
<img width="533" alt="image" src="https://user-images.githubusercontent.com/95575935/224718200-66f9d439-f5ee-430e-9963-71835186f073.png">


# link to dataset 
https://www.kaggle.com/datasets/emmarex/plantdisease

