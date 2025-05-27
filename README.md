This repo is dedicated to training PocketSphinx for recognizing Singaporean accents when reading out SNELLEN. I am trying to train PocketSphinx for these letters: C, D, E, F, L, O, P, T, and Z.

Here are the instructions to start this application:

type this into your terminal, replace audio_16k.wav with the name of the .wav audio file:

pocketsphinx single \
-hmm /usr/local/share/pocketsphinx/model/en-us/en-us \
-lm stt_training_alphabet_model/alphabet.dmp \
-dict stt_training_alphabet_model/alphabet.dict \
audio_16k.wav > output.txt


