
#### project based on deep improvisation developed by Tatsuya, 2017
* todos:
  * bill Evans style
  * replicate this in magenta and see the difference 
  * generate bass and drums in the same way or extract the original bassline and drums 
  * train it on real Bill Evans input 

## Usage: 
* run the driver file with the name of the original training piece in the midi/original

# This repo is based on Deep Improvisation

Easy-to-use Deep LSTM Neural Network to generate song like containing improvisation.

[Demo (SoundCloud)](https://soundcloud.com/tsyworks/sets/deep-improvisation)


## Dependencies

 - Keras
 - TensorFlow
 - Python MIDI

## Usage for individual file

  #### 1. Set up environment (conda recommended)

  ```
  pip install -r requirements.txt
  ```

  #### 2. Parse MIDI file to text

  ```
  python ./src/parse_midi_to_text.py
  ```

  #### 3. Train the model (GPU recommended)

  ```
  python ./src/training.py
  ```

  #### 4. Generate music

  ```
  python ./src/generate_music.py
  ```

## Note

 - You can use other MIDI file to train the model to generate new song. Change the file `./midi/original/original_song.mid`.
 - MIDI format is usually consist of multiple track and this repository is currently not supporting automatic detection which track is main part of the song. So you may have to choose track as index of the pattern in `parse_midi_to_text.py`.


## Credits 

MIT © [Tatsuya Hatanaka](https://github.com/tatsuyah)
