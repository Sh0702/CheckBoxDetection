# CheckBoxDetection
Project Involves detecting checkboxes in a scanned image using Image Processing and Computer Vision Techniques.

Initial detection of checkboxes was done using Image Processing techniques such as horizontal and vertical line detection.
Due to poor results, a more effective inbuilt edge detector known as Canny Edge Detector was used. While the performance imporved, it was still ineffective as it detected a lot of unneseccary parts such as gap between text characters. 
As a result, the same methods were tried after removing text from the image usng a tool known as keras_ocr. The results did improve especially using Canny Edge Detector.

While these results using Image Processing was effective for a small amount of data, the same methods can't be used for large volumes of data. In addition to this, text removal using keras_ocr resulted in distortions especially in the presence of handwritten data which could not be properly removed by the keras_ocr tool. Hence a deep learning approach was used.

Due to lack of dataset for this project, custom dataset was created with 57 images with coordinates of marked and unmarked checkboxes stores in a XML file for each image. It is split into training and testing data with 45 and 12 images respectively. This custom dataset was trained using a model from a package called Detecto. Detecto is a very effective package as it can load data in both image files and xml format and also model the data using its own inbuilt model. It can also be used for visualisation, plotting and also showing labels for detected objects.

After running the model, it is tested using test data and is shown to effectively detect marked and unmarked checkboxes with the respective labels.
