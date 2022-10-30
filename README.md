# CheckBoxDetection

Due to the confidentiality of the data, the code is not uploaded yet on GitHub.

Project Involves detecting checkboxes in a scanned image using Image Processing and Computer Vision Techniques. 

Initial detection of checkboxes was done using Image Processing techniques such as Canny Edge Detector was used. Performance was good it showed a lot of distortion due to noise.

As a result, the same method was tried after removing text from the image usng a tool known as keras_ocr. While results improved, noise due to handwritten data in the image caused distortion. Hence a deep learning approach was used.

Due to lack of dataset for this project, custom dataset was created using MakeSenseAI. The dataset consisted of 57 images with coordinates of marked and unmarked checkboxes stores in a XML file for each image. It is split into training and testing data with 45 and 12 images respectively. This custom dataset was trained using a model from a package called Detecto. Detecto is a very effective package as it can load data in both image files and xml format and also model the data using its own inbuilt model. It can also be used for visualisation, plotting and also showing labels for detected objects.

After running the model, it is tested using test data and is shown to effectively detect marked and unmarked checkboxes with the respective labels.
