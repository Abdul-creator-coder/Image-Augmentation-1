# Image-Augmentation-1
Firstly, we define a Pipeline object and pass in the directory path of the images you want to augment. In this case, it is "C:\\Users\ghani\Downloads\Image Augmentation\Image". This will create a pipeline that reads all the images in that directory and applies the augmentation operations to them.

Next, we apply various augmentation operations to the images using the methods provided by the Pipeline object. These methods include:

zoom: This method zooms the image by a random factor between min_factor and max_factor. The probability of applying this operation is set to 0.3.

crop_random: This method crops a random area of the image by a percentage area between 0 and 1. The probability of applying this operation is set to 0.9.

flip_left_right: This method flips the image horizontally. The probability of applying this operation is set to 0.9.

flip_top_bottom: This method flips the image vertically. The probability of applying this operation is set to 0.8.

skew_tilt: This method skews the image by a random angle between -magnitude and magnitude. The probability of applying this operation is set to 0.8.

random_color: This method applies a random color transformation to the image. The probability of applying this operation is set to 0.9, and the color transformation is randomly chosen between min_factor and max_factor.

greyscale: This method converts the image from RGB to grayscale. The probability of applying this operation is set to 1.

resize: This method resizes the image to a specified width and height. The probability of applying this operation is set to 1.

random_brightness: This method randomly adjusts the brightness of the image by a factor between min_factor and max_factor. The probability of applying this operation is set to 0.3.

black_and_white: This method converts the image to black and white. The probability of applying this operation is set to 1, and the threshold for converting the image is set to 187. It is setting the probability of applying the black and white operation to 1 (i.e., it will always be applied) and setting the threshold value to 187. This means that any pixel with an intensity value greater than 187 will be set to white, and any pixel with an intensity value less than or equal to 187 will be set to black.

Finally, you use the sample method to generate 5 augmented images from the defined pipeline. This will apply the defined augmentation operations to the images in the directory and save the resulting images in a new directory.

Overall, this code demonstrates how to use the Augmentor library to perform a wide range of image augmentation operations in Python.
