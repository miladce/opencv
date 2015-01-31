# Color Specification
after equalizing the histogram of the input image and desired histogram,
we must relate this two equalized histograms.
for equalizing histograms we must normalize the cdf of the histograms.
then mapping colors of those.
this links may help you:
http://fourier.eng.hmc.edu/e161/lectures/contrast_transform/node3.html
https://www.scribd.com/doc/106790597/OPENCV-Topic-04-Histogram-Specification#scribd
i write a function to use mapping instead of the mapping part of second link..
my function's  args are the values of the normalized of cdf of histograms and the output is the mapping array that specify a color for the colors of input image.
mappedColorUsedInDesiredImage=outputarray[inputImageColor]
