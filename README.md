# Color Specification
color specification in opencv:</br>
after equalizing the histogram of the input image and desired histogram,</br>
we must relate this two equalized histograms.</br>
for equalizing histograms we must normalize the cdf of the histograms. and then map their colors.</br>
these links may help you:</br>
http://fourier.eng.hmc.edu/e161/lectures/contrast_transform/node3.html</br>
https://www.scribd.com/doc/106790597/OPENCV-Topic-04-Histogram-Specification#scribd</br>
I wrote a function to use mapping instead of the mapping part of the second link..</br>
my function's  args are the values of the normalized of cdf of histograms and the output is the mapping array that specifies a color for the colors of input image.</br>
<code>
mappedColorUsedInDesiredImage=outputarray[inputImageColor]</br>
</code>
