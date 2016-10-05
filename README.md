# TIPS

Welcome to the *Tassel Image-based Phenotyping System*, aka *Tassel Image Processing Software*, aka *TIPS*!  See below for relevant information and help.

## Downloading and testing TIPS

I recommend you use `git` to obtain the latest version of this software.  You can clone the repository to your computer with `git` by entering the following in the command line:
> `git clone https://github.com/joeshmoe5409/TIPS.git`

You will also need to have MATLAB on your computer.

To verify that you have all the components, run TIPS on the test images included with the software:
> `matlab -nodesktop -nosplash -r "TIPS('testImg_foreground.jpg', 'testImg_background.jpg', './testOut/testImg'); quit()"`

If TIPS runs successfully, you should now have a folder in your working directory called 'testOut' containing two files: 'testImg_processed.png' and 'testImg_out.txt'.

## Running TIPS on your own images
### Inputs
TIPS was written to process tassels photographed in front of a white background.  The algorithm expects to be passed two images: one with the tassel in it (foreground), and one without the tassel (background), as well as an output path and prefix.  Formally, the arguments required by TIPS are:

* **foreground**: path to the image with the tassel in it. *e.g., './myTasselImages/tassel1_foreground.jpg'*
* **background**: path to the image without the tassel in it. *e.g., './myTasselImages/tassel1_background.jpg'*
* **out**: path and prefix for output.  Suffixes will be appended to this input by TIPS. *e.g., './output/tassel1'* will produce *'./output/tassel1_processed.png' and './output/tassel1_out.txt'*

This helps isolate the tassel faithfully.  Depending on the amount of noise in your imaging setup, you may be able 
