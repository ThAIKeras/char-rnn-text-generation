# Recurrent Neural Networks for Character-Level Language Modeling

Forked from [yxtay](https://github.com/yxtay)'s [char-rnn-text-generation](https://github.com/yxtay/char-rnn-text-generation).
For simplicity, only Keras related files are left in this fork.

Two major modifications are made for conducting experiments in [this article](https://medium.com/@u41ppp/1264028567a5). (The article is written in Thai language.)

- A dictionary is now built from training data
- The test section has been added

These are some usage changes from the original version.

### Training
- Add an optional argument --test-path TEST_PATH for validation data.

### Text Generation
- The default of --top-n is the total number of characters.
- The training file must be provided in --text-path in order to build a dictionary.

### Testing
```
usage: keras_model.py test --checkpoint-path CHECKPOINT_PATH
                           --text-path TEXT_PATH
                           --test-path TEST_PATH
```
