# TIPS

Welcome to the *Tassel Image-based Phenotyping System*, aka *Tassel Image Processing Software*, aka *TIPS*!  See below for relevant information and help.

## Downloading and testing TIPS

I recommend you use `git` to obtain the latest version of this software.  You can clone the repository to your computer with `git` by entering the following in the command line:
> `git clone https://github.com/joeshmoe5409/TIPS.git`

To verify that you have all the components, run TIPS on the test images included with the software:
> `matlab -nodesktop -nosplash -r "TIPS('testImg_foreground', 'testImg_background', './testOut/testImg'); quit()"`
