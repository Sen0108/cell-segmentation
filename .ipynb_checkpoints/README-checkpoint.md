# Image Processing methods for automatic segmentation and information extraction
### Step-1
Extraction of the green channel of image. To achieve more precious results, we use mask based on the HSV color space. Thresholding is done based on the hue of the green colors found in the image

### Step-2
Applying morphological opening operation to clear overlaps in the images

### Step-3
Using the separation and then dilating images to 

### Step-4
Applying Distance Transform to create a analog map of distance from center to it's edges

### Step-5
Limiting the the distance to max the half distance

### Step-6
Using the connected components algorithms to mark several blobs as individual components for tracking and applied watershed by using the separated components as seeds

### Step-7
Used the regionprops function of skimage to extract information about the components and blobs to store in csv file

