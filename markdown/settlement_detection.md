#h1 Automatic Dwelling Detection

#h3 1 - Goal
#pg Most westerners underestimate the sheer size of refugee camps and resettlement areas in developing nations in crisis. The number of dwellings, tents, or other structures can be as large as 100 thousand and more. In addition, they are constantly shifting in numbers as people move in and out. 

#h3 2 - Data
#pg Using satellite imagery is the only real way to estimate numbers with some reasonable accuracy. At the United Nations, UNOSAT is the organization for tracking those flows using that imagery. However, their work is highly tedious and time-consuming as images were labeled by hand. My goal was to come up with a solution. 

#im ../assets/settlement_detection/1.png 50 256 Figure 1 - Satellite Image of the Ztari Refugee Camp

#h3 3 - Model
#pg The model I used is a slightly modified version of the deep convolutional neural network architecture called U-net. U-net is a convolutional network architecture for the segmentation of images. For my project, I revised the architecture such that the network takes as input images of real satellite images and outputs a grayscale probability map where the level of white of a pixel indicates the confidence that a particular structure is present within a single pixel. In the second step, I designed a filtering method similar to non-maximum suppression. Non-Maximum Suppression (NMS) is used in numerous computer vision tasks. It is a class of algorithms to select one entity (e.g., bounding boxes) out of many overlapping entities. However, instead of bounding boxes, my filtering method returns a single point which could then easily be counted as a single structure of interest. 

#im ../assets/settlement_detection/2.png 50 256 Figure 2 - Model Architecture

#h3 4 - Impact
#pg The convolutional neural networks were extremely accurate, saving the agency considerable time estimating numbers. Although I cannot show the original results, the image below is a good representation of what the input, output, and final NMS filtering would have looked like. It should also be added that this specific refugee camp is relatively easy, even for traditional computer vision techniques. Other refugee camps, for example, Gendrasa and Doro in South Sudan, are much more irregular, yet the model still performed exceptionally well.

#im ../assets/settlement_detection/3.png 50 256 Figure 3 - Input (left), output (middle) of the model and subsequent filtering operation (right). 

#h3 5 - Technologies Used
#br 
#it ../assets/logos/torch.png 0 96  
#it ../assets/logos/awsec2.png 0 96 
#it ../assets/logos/python.png 0 96
#it ../assets/logos/scipy.png 0 96
#it ../assets/logos/numpy.png 0 96
#it ../assets/logos/cuda.png 0 96
#it ../assets/logos/cuda.png 0 96

