# blindness_detection
Blindness Detection
The data was downloaded from Kaggle. The data when extracted gave a warning that the file is corrupt. There were images missing in the folder. I made a new dataframe when contained only the images available and only for those images the labels were available.

Diabetic eye disease comprises a group of eye conditions that affect people with diabetes. These conditions include diabetic retinopathy, diabetic macular edema (DME), cataract, and glaucoma. All forms of diabetic eye disease have the potential to cause severe vision loss and blindness. Diabetic retinopathy involves changes to retinal blood vessels that can cause them to bleed or leak fluid, distorting vision. Diabetic retinopathy is the most common cause of vision loss among people with diabetes and a leading cause of blindness among working-age adults. DME is a consequence of diabetic retinopathy that causes swelling in the area of the retina called the macula. Because diabetic retinopathy often goes unnoticed until vision loss occurs.

Diabetic retinopathy affects blood vessels in the light-sensitive tissue called the retina that lines the back of the eye. It is the most common cause of vision loss among people with diabetes and the leading cause of vision impairment and blindness among working-age adults. For building a machine learning model, I have downloaded the data from an open source website Kaggle.com.

The model building would help speed up disease detection and this would help to prevent lifelong blindness.

There are two types of files, one being the CSV file for storing the labels of the images and another folder containing the images. The data size is of 929 images and the images are labeled into 5 categories. 

1) Class 0 : No Diabetic retinopathy

2) Class 1 : Mild

3) Class 2 : Moderate

4) Class 3 : Moderate

5) Class 4 : Severe

I experimented with various changes to the dataset to build a robust model. I tried different pre-trained weights (Transfer learning). Different image size(150, 250, 256, 500,etc) , simple and complex data augmentation. 
I also found some extra data on Internet and tried using it to improve the model's performance but the model did not perform well with the additional data.

The best performing model gave a Kappa Score of 73.5

In the model, the image size was 250*250, DenseNet 201 as the pre-trained weights, used early stopping and ReduceLearningRateOn Plateau to avoid overfitting of data.
