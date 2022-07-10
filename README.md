# Dependencies
1. numpy
2. skimage
3. PIL
4. argparse


# How to execute the code :

1. You will first have to download the repository and then extract the contents into a folder.
2. Make sure you have the correct version of Python installed on your machine. This code runs on Python 3.6 above.
3. Install all dependencies mentioned above.
4. You can open the folder and run texture_synthesis.py on command prompt.
> `python texture_synthesis.py --image_path <image_path> --block_size <int_value> --num_block <int_value>


**Note :**
1. image_path is the addresss of the input image.
2. block_size is size of the patch (block) to be used for texture synthesis. Choose it wisely.
3. num_block is the number of patches to be synthesized. The more the number of blocks, the bigger the output image.
4. Side length of square output image (in pixels) will be:$$(num\_block*block\_size) - (num\_block-1)*(block\_size/6)$$
5. The output will be saved in the output folder. The format of the output image name will be:  
<input_image_name>\_<block_size>\_<num_block>.png


# References :

## Code References :

Code has been referred from the following sources:

[1] Image-Quilting: https://github.com/lschlessinger1/image-quilting  
[2] Texture Synthesis: https://github.com/Devashi-Choudhary/Texture-Synthesis

## Input Images :

The input images can be found in the "resources/input/" directory. These images have been used to generate outputs. Sources for the images: 

[1] blood\_vessels.png: https://in.pinterest.com/pin/524317581592002674/
[2] brain.jpeg: https://www.brainline.org/tbi-basics/interactive-brain
[3] rbc.png: https://www.medicalnewstoday.com/articles/red-blood-cell-disorders-types-causes-and-symptoms