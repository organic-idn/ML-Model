 <h1 align="center"> ML-Model </h1>

This Repository is used by Machine Learning path cohort to develop object detection models to implement the Organic Vegetable Storage Suggestions Classification
![Bangkit Image](bangkit.png)

<br>
<h3>Architecture</h3>
<br>
<p>
1. Google Image Scraping
  <br>
  <pre>
  he project begins by scraping images from Google to form the dataset. The gathered images are then divided into two categories:
  a. **Training Images:** These images will be used to train our model, allowing it to learn patterns and identify objects of interest.
  b. **Testing Images:** These images will be used to evaluate the trained model's performance and accuracy in identifying objects of interest.
  <br>
2. Labelling Images Using LabelImg
  <br>
  <pre>
  The collected images (both training and testing) are labeled using LabelImg. This involves marking regions of interest in the images and assigning appropriate class labels for the model to learn from. </pre>
  <br>
3. Label Map Creation
  <br>
  <pre>
  A label map is created next. This is a mapping between the class labels and their integer identifiers, which aids in translating the model's numerical output back into understandable class labels. </pre>
  <br>
  <br>
4. Label Map Creation
  <br>
  <pre>
  A CSV record is created for both the training and testing datasets. This record contains the image file paths, object bounding box coordinates, and class labels. </pre>
  <br>
5. TFRecord Creation (Train and Testing)
  <br>
  <pre>
  The CSV files for both training and testing data are then converted into the TFRecord format, which is a common format for storing large amounts of data and metadata in TensorFlow. </pre>
  <br>
6. Fetch MobileNetV2 SSD FPN Pretrained Model
  <br>
  <pre>
  Following the data preparation, we fetch the pre-trained MobileNetV2 SSD FPN model. Using this pretrained model accelerates our training process by leveraging the patterns already learned. </pre>
  <br>
7. Configuring MobileNetV2 SSD FPN Model
  <br>
  <pre>
  The fetched model is then configured according to our project's specific needs. This includes setting model parameters and other configurations suitable for our data and objectives. </pre>
  <br>
8. Training Dataset on MobileNetV2 SSD FPN
  <br>
  <pre>
  With the model configured, we move on to training it with our prepared and labeled dataset. The model learns to identify and classify the objects of interest in our images. </pre>
  <br>
8. Converting to TFLite
  <br>
  <pre>
  After satisfactory training of the model, it's converted into TFLite format. This conversion facilitates the deployment of our model on mobile or edge devices, ensuring efficient execution of our object detection tasks. </pre>
  <br>
</p>
