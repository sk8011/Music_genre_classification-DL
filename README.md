# 🎵 Music Genre Classification Using Deep Learning

This project implements a Convolutional Neural Network (CNN) to classify music tracks into 10 distinct genres using the GTZAN dataset.
By converting audio signals into Mel-spectrograms, the model captures both spectral and temporal features, achieving high classification accuracy.

## 📌 Features

- **CNN Architecture**: A 7-layer CNN with filter sizes ranging from 32 to 512, incorporating dropout layers to mitigate overfitting.
- **Audio Preprocessing**: Segmentation of audio files into overlapping chunks, conversion to Mel-spectrograms, and resizing to ensure uniform input dimensions.
- **Model Evaluation**: Utilization of confusion matrices and classification metrics (precision, recall, F1-score) to assess performance.
- **Streamlit Integration**: An interactive web application built with Streamlit for real-time genre prediction.

## 📂 Project Structure

```
├── Train_Music_Genre_Classifier.ipynb   # Notebook for training the CNN model
├── Test_Music_Genre.ipynb               # Notebook for testing and evaluation
├── streamlit_app.py                     # Streamlit app for genre prediction
├── Trained_model.h5                     # Saved trained model
├── requirements.txt                     # List of dependencies
├── music_genre_home.png                 # Image used in the Streamlit app
└── README.md                            # Project documentation
```

## 🛠️ Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/sk8011/Music_genre_classification-DL.git
   cd Music_genre_classification-DL
   ```

2. **Create a virtual environment (optional but recommended)**:

   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install the required packages**:

   ```bash
   pip install -r requirements.txt
   ```

## 🚀 Usage

### Training the Model

Open the `Train_Music_Genre_Classifier.ipynb` notebook to train the CNN model on the GTZAN dataset. Ensure that the dataset is properly loaded and preprocessed as per the instructions in the notebook.

### Testing and Evaluation

Use the `Test_Music_Genre.ipynb` notebook to evaluate the trained model's performance. This includes generating confusion matrices and calculating classification metrics.

### Running the Streamlit App

To launch the interactive web application for genre prediction:

```bash
streamlit run streamlit_app.py
```

This will open a web interface where you can upload audio files and receive genre predictions in real-time.

## 🎧 Dataset

The project utilizes the [GTZAN dataset](http://marsyas.info/downloads/datasets.html), which comprises 1,000 audio tracks each 30 seconds long, categorized into 10 genres: blues, classical, country, disco, hiphop, jazz, metal, pop, reggae, and rock.

## 📈 Results

- **Validation Accuracy**: Achieved 84% accuracy on the validation set.
- **Model Performance**: Demonstrated strong generalization capabilities across diverse genres, as evidenced by evaluation metrics.

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 🤝 Acknowledgments

Special thanks to the creators of the GTZAN dataset and the open-source community for providing tools and resources that made this project possible.
