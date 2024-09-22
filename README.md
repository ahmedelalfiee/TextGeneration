<p align="center">
  <img src="https://github.com/user-attachments/assets/b5712b63-08b5-4567-bbd4-285820d20a5e" width="700" />
</p>

## Project
1. Load and parse text.
2. Train a GRU network for single character generation.
3. Generate some text with the trained GRU network.

## Dataset
Download the text file "Alice's Adventures in Wonderland" from Project Gutenberg
!wget -O wonderland.txt https://www.gutenberg.org/ebooks/11.txt.utf-8

## Trained Network
Gated Recurrent Unit (GRU) with parameters:
- input_size=1,       # Input size: one-hot encoded characters (represented as floats here)
- hidden_size=512,    # Hidden size of the GRU layer
- num_layers=5,       # Number of GRU layers stacked on top of each other
- batch_first=True,   # Input tensors are of shape (batch_size, seq_len, features)
- dropout=0.5         # Dropout rate for regularization
