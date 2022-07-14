# Image Processing methods for automatic segmentation and information extraction

### Step-1
Removing noise by thresholding out values less than 30 in the BGR channels

### Step-2
Creation of masks corresponding to the green and blue hues (HSV color space) in the image. 

### Step-3
Applying morphological opening operation to clear overlaps in the images

### Step-4
Using the separation and then dilating images to 

### Step-5
Applying Distance Transform to create a analog map of distance from center to it's edges

### Step-6
Limiting the the distance to max the half distance

### Step-7
Using the connected components algorithms to mark several blobs as individual components for tracking and applied watershed by using the separated components as seeds

### Step-8
Used the regionprops function of skimage to extract information about the components and blobs to store in csv file

