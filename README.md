<p align="center">
  <img src="organic_logo.png" alt="Organic" height="120" />
</p>
<h1 align="center"> ML-Model </h1>

This Repository is used by Machine Learning path cohort to develop object detection models to implement the Organic Vegetable Storage Suggestions Classification
![ML-Timeline-Project](https://github.com/organic-idn/ML-Model/assets/98405455/1ba7e4c1-67d1-4d35-9545-0278ce18b3f0)

<br>
<h3>Machine Learning Project Timeline</h3>
<br>
<p>
1. Google Image Scraping
   <br>
   ![showdatasets](https://github.com/organic-idn/ML-Model/assets/98405455/7b40d69e-447e-4250-aed0-0e4f760522cc)
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

<h1 align="center"> Object Detection API using SSD Mobilenet V2 </h1>
<p align="center">
  <img src="mobilenet.jpeg" alt="MobileNet" height="320" width="840"/>
</p>
<br>
MobileNetV2, developed by Google, is an efficient and compact neural network model designed for mobile and edge devices. Building upon its predecessor, MobileNetV1, it introduces two key features: inverted residuals and linear bottlenecks. These architectural improvements maintain high accuracy while being highly computationally efficient. Inverted residuals help in reusing bottlenecks from previous layers, whereas linear bottlenecks reduce the model's size by reducing the dimensionality inside the network. The result is a balance of performance and size, making MobileNetV2 ideal for resource-constrained devices and applications like real-time image classification and object detection.
<br>
<br>
<h3 align="left"> Reference </h3>
• MobileNetV2 SSD FPN - Edge Impulse Documentation. (2017). Edgeimpulse.com. <a href="https://docs.edgeimpulse.com/docs/edge-impulse-studio/learning-blocks/object-detection/mobilenetv2-ssd-fpn">MobileNetV2 SSD FPN</a>
<br>
• Installation — TensorFlow 2 Object Detection API tutorial documentation. (2023). <a href="https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/install.html">TensorFlow2 Ovject Detection API Tutorial</a>
