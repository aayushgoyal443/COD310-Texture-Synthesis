# Dependencies
1. numpy
2. skimage
3. PIL
4. argparse


# How to execute the code :
**Using Command Line :**
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