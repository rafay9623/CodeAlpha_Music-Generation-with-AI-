# CodeAlpha_Music-Generation-with-AI-
This project generates music using a Long Short-Term Memory (LSTM) neural network trained on MIDI files. It processes MIDI data, trains a model, and generates new music sequences saved as MIDI files.

Features
Extracts notes and chords from MIDI files using music21.
Trains an LSTM model to predict note sequences.
Generates new music sequences and saves them as MIDI files.

Prerequisites
Python 3.8+
Install: music21, tensorflow, numpy, keras
pip install music21 tensorflow numpy keras
MIDI files (e.g., lbtheme.mid, lbvar1.mid, lbvar2.mid, lbvar6ep.mid)

Installation
Clone the repository:
git clone <repository-url>
cd music-generation-ai

Install dependencies:
pip install -r requirements.txt
Place MIDI files in the project directory.

Usage
Preprocess MIDI files: Run Music Generation with AI.py to extract notes from MIDI files and save them to data/notes.pkl.
python "Music Generation with AI.py"
Train the model: The script trains an LSTM model on the extracted notes and saves it to models/music_model.h5.
Generate music: The script generates a new music sequence and saves it as output/generated_music.mid.

Files
Music Generation with AI.py: Main script for preprocessing, training, and music generation.
data/notes.pkl: Stores extracted notes.
models/music_model.h5: Trained LSTM model.
models/mapping.pkl: Note-to-integer mapping.
output/generated_music.mid: Generated MIDI file.
