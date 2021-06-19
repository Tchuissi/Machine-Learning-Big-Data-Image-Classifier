This application was developed in Google Colab and will work best there. If you want to run the notebooks as is, without having to change the code to point to local storage, please send us a message so we can add you to the Google Drive directory.
Data Processing
1.	Begin in the “Get_Flickr_Pics/Store_in_MongoDB” notebook located in Google Colab.
a.	Get the ip address of the Colab instance and save to MongoDB Atlas
b.	Run the notebook to get 500 image datasets, validate the descriptions and upload the subset with valid English descriptions to MongoDB Atlas
c.	Repeat to get the desired number of training photos
2.	Go to the “Download_Images_To_Google_Drive” notebook located in Google Colab.
a.	Get the ip address of the Colab instance and save to MongoDB
Model Training
After the training data has been downloaded to a local disk, do the following:
1.	Run the 03_model_training_prep.ipynb notebook to create the files to be used to train the model
2.	Run the 04_model_training.ipynb notebook to train the model - this will take about 2 hours
3.	Run the 05_predict.ipynb notebook to make predictions
