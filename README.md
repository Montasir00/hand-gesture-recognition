# AI Software for Hand Gesture Recognition

## Introduction

Hand gesture recognition is a technology that enables computers to understand human hand signals by combining machine learning and computer vision. This project aims to develop a model that can recognize various hand gestures in real time.

## Main Components

### 1. Data Collection

Data collection is crucial for training the hand gesture recognition model. The process involves:

- **Video Capture:** Initializing video capture with `cv2.VideoCapture(0)` for continuous frame reading.
- **Hand Detection:** Using `cvzone.HandTrackingModule` to detect hands in each frame.
- **Image Processing:** Cropping and resizing hands to a standardized format for improved visualization.
- **User Interaction:** Saving processed images by pressing the 's' key, with a timestamp for easy data collection.

### 2. Data Storage

- All data is organized in a central repository.
- Each labeled folder corresponds to a distinct hand gesture (A-Z).

### 3. Model Training with Teachable Machine

Steps involved in training the model:

- **Data Upload:** Upload labeled hand gesture data to Teachable Machine.
- **Data Preprocessing:** Resize and normalize images for consistency.
- **Data Splitting:** Use an 80-20 split for training and testing.
- **Feature Extraction:** Employ CNNs for feature extraction.
- **Model Training:** Adjust model parameters based on training data.
- **Model Evaluation:** Evaluate with accuracy, precision, recall, and F1 score.
- **Model Refinement:** Adjust hyperparameters or collect more data if needed.

### 4. Testing Script

- **Initialization:** Load the pre-trained model (`keras_model.h5`) and labels (`labels.txt`).
- **Image Processing and Classification:** Process frames in real time and classify hand gestures.
- **User Interaction:** Terminate the script by pressing the 'm' key.

Usage
Data Collection: Use the data collection script to capture hand gesture images.
Model Training: Upload the collected data to Teachable Machine and train the model.
Testing: Use the testing script to evaluate the model in real time.
Conclusion
This project integrates data collection, model training, and testing into a cohesive tool for real-time hand gesture recognition. The combination of OpenCV, cvzone, and Teachable Machine ensures a robust and adaptable solution.

### Future Considerations
Potential applications include:

1.HumanComputerInteraction
2.SignLanguageRecognition
3.GamingControl
4.EducationalTools
