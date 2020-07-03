# To organize later

## Encoder-decoder implementation architecture
To implement the encoder-decoder architecture, you should follow this :-

Add an embedding layer which consumes the input
Add a Bidirectional RNN layer (with return_sequences= false) which runs on top of embedding layer and produces the final encoder hidden state.
Add a repeatVector as shown above which then repeats the final encoder state decoding number of steps time , here `output_sequence_length`.
Then Add another Bidirectional RNN layer for decoder
Time Distributed dense to predict the logits across french_vocab
