# Melody and Chord Extraction Pipeline

## Directory Contents

### Folders
- `clean_midi/` - Original MIDI dataset
- `chord_segments/` - 8-bar MIDI segments
- `matrix_data/` - Raw piano-roll matrices
- `matrix_data_only_chords/` - Chord vectors
- `monophonic_matrices/` - Single-line melodies
- `normalized_matrices/` - Pitch-normalized melodies and chords
- `no_pauses_matrices/` - Continuous melodies and chords -> use to train model without pauses
- `silence_matrices/` - Melodies with explicit silence row (129x128) and chords -> use to train model with marked pauses
- `reconstructed_midis/` - Generated MIDI files (examples)

### Data Files 
- `valid_midi_files.pickle` - 4/4 time signature files list
- `melody_chord_files.pickle` - Valid track pairs list
- `track_indices.pickle` - Track numbers list
- `dense_melodies.pickle` - Filtered melodies list

### Code
- `melody_chord_separation_tested.ipynb` - Main pipeline