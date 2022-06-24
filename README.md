# Mask-predictor
Technique to find🔎 the mask of an image from a folder of different masks by masking the image and then searching the best fit.

Here Deeplab-V3🚀 is used for object detection and segmentation part

Explanation Cell-wise

Cell-1: Importing 'TORCH' library and pre-trained models

cell-2: Selecting an input image and processing it for masking
        Checking is done whether there is any such object in image to be detected and masked
        
Cell-3: Add mask, plot, save and display the image and just blacken out everything else

Cell-4: Import the saved mask image and whiten out the detected part using 'CV2' library
        Whitening is done here because it was not working in Cell-3
        
Cell-5: Scan for images in the folder, done using 'OS' library
        Check their dimensions and match those with similar dimensions
        Then match those with similar identities using 'Skimage' library
        Print out all the similar ones with similarity more than 90%
