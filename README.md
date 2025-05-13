# Sound Classification Using CNN

## Overview

This project focuses on classifying sound data using a Convolutional Neural Network (CNN). The process involves several preprocessing steps, including amplitude normalization, noise reduction, segmentation, and resampling to 16kHz. The audio data is then converted into spectrograms and fed into a CNN for classification. The model achieves 94% accuracy on the test dataset.

## Preprocessing Steps

1. **Amplitude Normalization**: Normalize the audio signal to ensure consistent volume levels across all audio samples.

2. **Noise Reduction**: Apply noise reduction techniques to remove background noise and enhance the quality of the audio signal.

3. **Segmentation**: Split the audio into smaller chunks (e.g., 1-second segments) to allow for better feature extraction.

4. **Resampling to 16kHz**: Resample the audio to 16kHz to ensure uniformity across all input data.

## Spectrogram Generation

5. **DFT (Discrete Fourier Transform) and Windowing**: Perform a Discrete Fourier Transform to convert the audio signal from the time domain to the frequency domain. Apply windowing to minimize spectral leakage.

6. **Convert Spectrogram to 2D Images**: Convert the spectrogram data into 2D images, which will serve as input to the CNN.

## Model Architecture

- **Convolutional Neural Network (CNN)**: A CNN is used to learn spatial features from the 2D spectrogram images.
  
- **Fully Connected (FC) Layer**: The features learned by the CNN are passed to a Fully Connected layer for classification.

## Results

- **Test Accuracy**: The model achieves an impressive test accuracy of 94%.

## Conclusion

This project demonstrates the effectiveness of CNNs for sound classification tasks. The preprocessing steps, combined with the CNN architecture, allow the model to learn spatial features from audio spectrograms and make accurate predictions.

## Requirements

- Python 3.x
- Libraries: librosa, noisereduce, numpy, tensorflow/keras (for CNN), matplotlib
