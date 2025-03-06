Grocery Detection
This project provides a solution for detecting groceries displayed on shelves using a YOLOv4 model trained on the Grocery Dataset. The model checkpoints utilized in this project are sourced from the Grocery Object Detector for FMCG using Scaled YOLOv4-P5 repository.

How to Use the Model
1. Extract Files
Unzip the grocery_detect_submission.zip file to access the necessary files.

2. Contents of the Archive
grocery_detection_server.ipynb: Contains the inference code and the implementation of a Flask server.
grocery_detect_client.ipynb: Contains the client code for sending requests to the Flask server.
last_yolov4-p5-results_strip.pt: Pre-trained model weights.
C1_P06_N1_S3_1.jpg: Sample test image for running inference.

3. Setting Up the Flask Server
Since the Flask server runs on Google Colab's localhost (port 8000), an ngrok tunnel is required to enable internet access to the server.
Add your ngrok authentication key to Google Colab's secrets.

4. Running the Server
Start the Flask server and copy the ngrok public URL generated as the output.
Use this URL in the client script to send requests to the server.

5. Inference via Client Code
Once the server is running, execute the client code to send an inference request and receive the response.
This setup allows for easy deployment and testing of grocery detection on shelf images.