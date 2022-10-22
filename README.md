https://github.com/vilgub/signs/

Here is my notebooks.

Dataset from kaggle: https://www.kaggle.com/code/watchman/russian-traffic-signs/data
                     (folder 'rtsd-frames' with photos and 'full-gt.csv')

All photos are taken from the car. Some of the photos have multiple road signs. 
CSV file contains the coordinates of the upper left corner, the height and width of the road sign.

1. I decided to collect all road signs in different folders according to the class. 
Images will be stored at a size of 32 by 32 pixels, so when cutting out a fragment, 
I took a larger size from the width and height of the sign and resized it to the desired size.

    dataset_from_photos_to_class_folders.ipynb

2. The dataset does not contain data indicating the name of road signs. 
Therefore, I created a csv file with this information, renaming the folder names along the way 
to a convenient list of integers. (in order not to deal with the routine of copying and pasting data, you can use the attached csv)

    create_classesCSV_rename_folders.ipynb
    labels.csv

3. Some classes have very few images for model training, I removed folders with less than 100 images

    remove_small_data.ipynb

4.  The most interesting part is where you can enjoy the results. Preparing data for training and validation. Sequential model training. Visualization of results. Saving the Trained Model
    
    model_create_train.ipynb



"Time you enjoy wasting was not wasted."
  John Lennon
