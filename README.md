# Music_genre_classification-DL

- Implemented a CNN-based audio classification system on the GTZAN dataset to identify 10 distinct music genres with 84% validation accuracy
- Engineered audio feature extraction pipeline that converts raw audio to Mel-spectrograms through chunking with strategic overlapping to capture temporal characteristics
- Designed and trained a 7-layer CNN architecture (32→512 filters) with dropout regularization to prevent overfitting on spectral representations
- Developed comprehensive data preprocessing workflow including audio segmentation, feature extraction, and matrix resizing for consistent model input
- Conducted thorough model evaluation using confusion matrices and classification metrics (precision, recall, F1-score) to assess performance across different music genres
- Created visualization tools for audio waveforms, Mel-spectrograms, training history, and model performance metrics to enhance interpretability
- Applied transfer learning techniques with TensorFlow to optimize training on limited audio data while maintaining high classification accuracy

<br>
To run the project, install required libraries using `pip install -r requirements.txt`.
And then, simply run the Music_Genre_App.py file using the cmd `streamlit Music_Genre_App.py`.
