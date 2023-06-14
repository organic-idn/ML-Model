 <h1 align="center"> Organic ML </h1>

![Bangkit Image](organic_logo.png)

<h1 align="center"> ML-Model </h1>

This Repository is used by Machine Learning path cohort to develop object detection models to implement the Organic Vegetable Storage Suggestions Classification
![Bangkit Image](bangkit.png)

<br>
<h3>Machine Learning Project Timeline</h3>
<br>
<p>
1. Google Image Scraping
   <br>
   <pre>
   - Training Images: These images are used for training the model.
   - Testing Images: These images are used for evaluating the trained model's performance.</pre>
   <br>
2. Labelling Images Using LabelImg
   <br>
   <pre>
   - This involves marking regions of interest in the images and assigning appropriate class labels.</pre>
   <br>
3. Label Map Creation
   <br>
   <pre>
   - A mapping between the class labels and their integer identifiers is created.</pre>
   <br>
4. CSV Record Creation (Train/Testing)
   <br>
   <pre>
   - A CSV record is created for both the training and testing datasets. This record contains image file paths, object bounding box coordinates, and class labels.</pre>
   <br>
5. TFRecord Creation (Train and Testing)
   <br>
   <pre>
   - The CSV files for both training and testing data are converted into the TFRecord format.</pre>
   <br>
6. Fetch MobileNetV2 SSD FPN Pretrained Model
   <br>
   <pre>
   - We fetch the pre-trained MobileNetV2 SSD FPN model to accelerate our training process.</pre>
   <br>
7. Configuring MobileNetV2 SSD FPN Model
   <br>
   <pre>
   - The fetched model is configured according to our project's specific needs.</pre>
   <br>
8. Training Dataset on MobileNetV2 SSD FPN
   <br>
   <pre>
   - The model is trained with our prepared and labeled dataset.</pre>
   <br>
9. Converting to TFLite
   <br>
   <pre>
   - The trained model is converted into TFLite format for efficient deployment on mobile or edge devices.</pre>
   <br>
</p>
