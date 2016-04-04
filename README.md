# canny-edge-detection
Matlab app which identifies the edges of a given image by applying a canny detection algorithm
----------------------
function emap = canny(img,sigma,fsize,tlow,thigh)
Applies canny edge detection algorithm to the given image
 img   - given image matrix
 sigma - the value of sigma for the derivative of gaussian blur
 fsize - given size of the gaussian blur kernal to be applied
 lowt  - given lower threshold, used for hysteresis to avoid streaking
 hight - given upper threshold, anything above which is an edge pixel

Good parameters:
    cameraman.tif :  canny('cameraman.tif',  1, 5, 10, 20)

Note: Marker may need to convert outputs to uint8 to view other functions
working
