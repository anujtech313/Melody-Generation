# Generating Melodies with RNN-LSTM

Technology used -  High Level API - Keras/Tensorflow, Music21 - Python Library For processing Symbolic Music Data, MuseScore - Software for music notation.

Time melody act as a time series data and hence time- series prediction problem. Musical Notes were trained in neural network architecture using RNN-LSTM to predict next note in the melody.

Melodies have a long-term structural patterns and LSTMs capture long-term temporal dependencies.

ESAC dataset was used for training purpose which consists of 5k+ songs from all over the world.

Note = Pitch + Duration, Pitch indicates how high/low a note is.

Music representation: 1) Sequence, Pitch/duration info for each note. 
                       2) Time series, Sample melody at each 16th note, Each step = 16th note, Log MIDI note when note occurs, use"_" symbol for held notes, Use "r" symbol for rest.
                       
Preparation of Melodies for LSTM ingestion - Time series representation - Map time series representation to integers - One-hot encoding.

![LSTM](https://github.com/anujtech313/Melody-Generation/blob/master/LSTM-MELODY%20Generation.png)

