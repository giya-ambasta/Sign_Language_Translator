# Sign Language Translator

A real-time Sign Language Translation system using Computer Vision and Machine Learning. This project can recognize American Sign Language (ASL) gestures and translate them into text.

## Features

- Real-time hand gesture recognition
- Support for ASL alphabet (A-Z, excluding J and Z)
- Interactive web interface using Streamlit
- Live webcam feed processing
- Word and sentence formation capabilities

## Technical Stack

- Python
- OpenCV (cv2) for image processing
- MediaPipe for hand tracking
- Streamlit for the web interface
- Scikit-learn for machine learning (Random Forest Classifier)

## Project Structure

- `app.py`: Main application with Streamlit interface
- `trainer.py`: Model training script
- `inference.py`: Real-time inference script
- `collect_img.py`: Data collection script
- `create_dataset.py`: Dataset creation and preprocessing
- `accuracy.py`: Model accuracy evaluation

## Setup and Installation

1. Clone the repository:
```bash
git clone https://github.com/giya-ambasta/Sign_Language_Translator.git
cd Sign_Language_Translator
```

2. Install required packages:
```bash
pip install opencv-python mediapipe streamlit scikit-learn numpy
```

## Usage

1. To run the main application:
```bash
streamlit run app.py
```

2. To collect new training data:
```bash
python collect_img.py
```

3. To create and process the dataset:
```bash
python create_dataset.py
```

4. To train the model:
```bash
python trainer.py
```

5. To test the model accuracy:
```bash
python accuracy.py
```

## Features in Detail

- **Home Page**: Introduction to the application and its purpose
- **What is Sign Language**: Educational content about ASL
- **How Does the Code Work**: Technical explanation of the system
- **Translate**: Real-time translation interface

## Model Information

The system uses a Random Forest Classifier trained on hand landmark features extracted using MediaPipe. The model processes the following:
- Hand landmark positions
- Relative distances between landmarks
- Hand gesture patterns

## Contributing

Feel free to contribute to this project by:
1. Forking the repository
2. Creating your feature branch
3. Committing your changes
4. Pushing to the branch
5. Creating a new Pull Request

## License

This project is open source and available under the MIT License.
