# Animal-Sound-classification
## Audio Classification with CNN
Developed a CNN-based audio classification model using spectrogram image inputs derived from raw audio signals.

Preprocessing: Applied amplitude normalization, noise reduction, segmentation, and resampling to 16 kHz.

Feature Extraction: Performed Discrete Fourier Transform (DFT) and windowing to generate spectrograms.

Input Preparation: Converted spectrograms into 2D images for CNN input.

Model Architecture: Spatial features learned by the CNN were passed to fully connected layers for final classification.

Result: Achieved 94% test accuracy on the dataset.
