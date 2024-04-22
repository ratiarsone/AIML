# Music Generation with Chord Accompaniment: A Deep Learning Approach

This repository contains the implementation of a deep learning system designed for generating music with chord accompaniment. Based on recurrent neural networks (RNN) and Long Short-Term Memory (LSTM) units, this code is a demonstration of extending music generation models to include harmonization.

## Overview

The project aims to train a model on piano MIDI files from the Maestro dataset, enabling it to predict the next note in a sequence and generate music with appropriate chord accompaniments. The model learns to understand the intricacies of melody and harmonizes by suggesting chords that fit within the key, enhancing the musical experience.

## Setup

The setup involves installing necessary Python libraries for MIDI file processing, neural network construction, data manipulation, and visualization.

```shell
pip install pretty_midi tensorflow pandas matplotlib seaborn
```

Ensure that these libraries are installed before attempting to run the scripts in this repository.

## Usage

The code is structured as follows:

- MIDI File Processing: Functions to extract melody and chord information from MIDI files, converting them into structured pandas DataFrames.
- Data Preprocessing: Normalizing pitches and generating fixed-length chord sequences for model training.
- Dataset Handling: Script to download the Maestro v2.0.0 dataset automatically.
- Neural Network Model: Setting up and training the LSTM model with TensorFlow, and visualizing the training loss.
- Music Generation: Functions to generate music by predicting chords using the trained model.

## Data

The Maestro dataset (version 2.0.0) used for training is included via a script that downloads and extracts the MIDI files automatically.

## Model

The neural network consists of LSTM layers ending with a dense softmax layer for chord classification. The model is trained on preprocessed sequences derived from the Maestro dataset.

## Visualization

Training progression can be visualized by plotting the training loss over epochs, which is included in the code.

## Contributions

Contributions to this project are welcome. Please feel free to fork the repository, make improvements, and submit a pull request.

## License

This project is open-source and available under the MIT License.

---

*Code authored by Edouard Ratiarson on March 21st, 2024.*
