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

2. 

create_classesCSV_rename_folders.ipynb

3.full-gt.csv

4. dict_sign_class.ipynb


5. remove_small_data.ipynb


6. model_create_train.ipynb

    изображения были отмечены на фотографиях, их координаты приложены в csv файле. 
    Так как я решил собирать изображения квадратного формата, я выбирал больший параметр из ширины и высоты размеченных знаков, 
    приводил их к матрице 32*32 и сохранял в npz для каждого класса

find reshape save signs in folders
rename files
make csv with numbers and classes
rename folders
make small np files in each folder
join np files in one
 README.md
Create README.md
11 days ago
create_classesCSV_rename_folders.ipynb
Add files via upload
2 days ago
dataset_from_photos_to_class_folders.ipynb
Add files via upload
2 days ago
dict_sign_class.ipynb
Add files via upload
2 days ago
model_create_train.ipynb
Add files via upload
1 minute ago
remove_small_data.ipynb
Add files via upload
2 days ago
rename 



