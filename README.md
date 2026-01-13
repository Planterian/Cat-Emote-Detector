# Cat-Emote-Detector

A funny simple project that i make using MediaPipe for landmark detection and scikit-learn for machine learning classification for my machine learning assignment

## Some Features

- **Pose Detection**: Full body pose with 33 landmarks
- **Face Detection**: 468 facial landmarks but i hide the landmark and just show some points for the eyes,top nose and mouth
- **Hand Detection**: Left and right hand with 21 landmarks each
- **Pose Classification**: ML model (RandomForest) to classify poses
- **Real-time Processing**: Live webcam feed processing with pose prediction
- **Data Collection**: Tool to collect training data for custom poses
- **Visualization**: Colored landmarks and connections with pose labels
- **Screenshot Capture**: Save detection result

## Installation
You need you download some library in the requirements file that i have put in the folder

## Project usage

## Run the project detector with the pre-trained model

```bash
python.exe main.py
```
## Controls

- **'q'**: Quit the application
- **'s'**: Save a screenshot of the current detection
- **'t'**: Retrain the model with sample data

### To collect your own data

```bash
python.exe data_collector.py
```

## Files and their usage

- `holistic_detector.py`: Core detector class with MediaPipe integration
- `pose_classifier.py`: ML model for pose classification using Random Forest
- `data_collector.py`: Tool for collecting training data and model training
- `main.py`: Main application script with pose classification

## Poses

The model can classify the following poses:

| Emote | Description | Reference |
|-------|-------------|-----------|
| **Absolute Cinema** | Show both of your hands up | <img src="funny-cat-emote-detector-main/images/cat_absolute_cin.jpg" width="100" height="100"> |
| **Crying** | Make your hands like a fist and then put below your eyes a bit | <img src="funny-cat-emote-detector-main/images/cat_crying.jpg" width="100" height="100"> |
| **Laughing** | just simply smile | <img src="funny-cat-emote-detector-main/images/cat_laughing.jpg" width="100" height="100"> |
| **Like** | Just thumbs up or both hands thumbs up at the same time | <img src="funny-cat-emote-detector-main/images/cat_like.png" width="100" height="100"> |
| **Pointing** | Point into the camera with one or both hand works | <img src="funny-cat-emote-detector-main/images/cat_pointing.jpg" width="100" height="100"> |
| **Punching** | Fist into the camera or fist upward | <img src="funny-cat-emote-detector-main/images/saitama.jpg" width="100" height="100"> |

(The punching one was specially make for my lecturer because he like OPM alot 😁)

Quick note: This is a pre-trained model that only classifies the poses above, if you want you add more poses or sounds then feel free to add in by modifying the code. You need to retrain the model also by running the file data_collector.py (Instrucion to use collect data is in the file also).











