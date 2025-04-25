# 🎵 Mood-Based Music Recommendation System 🎭
This project is a real-time emotion detection and music recommendation web application. It captures the user’s mood through a webcam image, classifies it using a deep learning model, and recommends songs tailored to the detected mood using a local dataset.

# 🔍 Features
🎥 Live Webcam Mood Detection using CNN deep learning model.

🧠 Real-Time Emotion Classification into moods like happy, sad, angry, neutral, and more

🎶 Song Recommendations based on user’s mood from a curated local CSV dataset

🔄 Shuffle Button to refresh recommendations for the same mood

🌐 Interactive Web Interface built with Flask

📷 Fast, responsive image capture for smooth user experience

# 🚀 Tech Stack
Python

TensorFlow / Keras (for mood classification using MobileNetV2)

OpenCV (for webcam input)

Flask (for web app backend)

HTML/CSS (for frontend)

Pandas (for handling song data from CSV)

# 📁 Folder Structure
├── app.py                        # Main Flask application
├── mood_classifier_mobilenetv2.h5  # Pre-trained model
├── data_moods.csv               # Dataset with song titles, artists, and mood labels
# 🛠️ How It Works
The webcam captures the user's face in real-time.

The frame is preprocessed and passed into a trained MobileNetV2 CNN model to detect mood.

The system maps the predicted mood to a filtered list of songs from data_moods.csv.

Recommendations are shown in the browser, and users can click Shuffle to refresh songs for the same mood.

# 📷 Supported Moods
happy

sad

angry

neutral

fear

disgust

surprise

# ▶️ Run the App
1. Clone the Repository
git clone https://github.com/your-username/mood-music-recommender.git
cd mood-music-recommender
2. Install Dependencies
pip install -r requirements.txt
3. Run the Web App
python app.py
4. Open in Browser
Visit: http://localhost:5000

# 📦 Dataset
The data_moods.csv file is used for recommending music based on the user's mood.
...
You can customize this dataset to suit your music taste or use an extended dataset from a music API (Spotify, Last.fm, etc.).

# 📌 Future Enhancements
🎧 Integrate with Spotify API for real-time track streaming and metadata

📱 Build a mobile version using Streamlit or Flutter

💾 Save user mood history and recommendations

🔊 Add audio playback to preview tracks directly in the app

# 🙌 Acknowledgements
TensorFlow

Keras Applications

OpenCV

Flask
