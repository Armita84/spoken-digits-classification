# spoken-digits-classification
Classification Methods for Audio MNIST Dataset

Dataset consists of recordings of spoken digits in wav files at 8kHz. The recordings are trimmed so that they have near minimal silence at the beginnings and ends.

The Samples recorded by 4 speakers with English pronunciations and there are totally 2,000 recordings (50 of each digit per speaker) in the dataset.

Files are named in the following format: {digitLabel}_{speakerName}_{index}.wav Example: 7_jackson_32.wav

If you want to know more about how dataset is created and contribute to creating more data, please check the below repository:

https://github.com/Jakobovski/free-spoken-digit-dataset

# Files/Folders Information
recordings: all audio samples are stored in this folder – 2000 wav files

spectrograms: audio images (audio spectrograms)

acquire_data/say_numbers_promp.py: File saying how record the spoken digits

acquire_data/split_and_label_numbers.py: File for splitting the original file and labeling the sample files

utils/trimmer.py: trim the silence in each file.

utils/spectogrammer.py: convert the audio files to spectrogram images (the sample file)

utils/fsdd.py: prepare audios for converting to spectrograms

metadata.py: contains information of the speaker

audio_plot.ipynb: Plot audio signal and spectrogram using Librosa

audio_to_spectrograms.ipynb: convert audios to images and store them to spectrograms directory.

data_preprocessing.ipynb: convert images to numpy arrays

xtrain_file.npy, ytrain_file.npy: train dataset in numpy files

xtest_file.npy, ytest_file.npy: test dataset in numpy files

model.ipynb: classification task based on different cnn architectures.

result_images: contains models graphs and plots

# Classification methods:
I used three CNN models and a LSTM model for classification. You can find the models and the results in model.ipynb


