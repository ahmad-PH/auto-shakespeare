
# AutoShakespeare

This program generates shakespear-style text from a piece of starting text that you provide. This is a pytorch implementation of the tensorflow tutorial on [generating text with an RNN](https://www.tensorflow.org/tutorials/text/text_generation).


## Usage
These are the arguments the program can receive:
```
       [-h] [--starting_text STARTING_TEXT] [--output_size OUTPUT_SIZE]
       [--use_pretrained {none,rnn,gru,lstm}]
       [--recurrent_module {rnn,gru,lstm}] [--dropout DROPOUT]

optional arguments:
  -h, --help            show this help message and exit
  --starting_text STARTING_TEXT, -s STARTING_TEXT
                        piece of text used as starting point for generation
  --output_size OUTPUT_SIZE, -o OUTPUT_SIZE
                        length of text to generate (in characters)
  --use_pretrained {none,rnn,gru,lstm}
                        which pretrained model to use?
  --recurrent_module {rnn,gru,lstm}, -r {rnn,gru,lstm}
                        type of recurrent module used for training
  --dropout DROPOUT, -d DROPOUT
                        how much dropout to use for training (between 0 and 1)
```

If `--use_pretrained` is not `none`, then a new model will be trained before generation begins, otherwise the specified pre-trained model is used.

## Dependencies

```
* PyTorch - 1.5
* matplotlib - 3.2
* numpy - 1.18
```

The versions provided above are those the program was tested with. It is probably not at all dependent on these specific versions, since the features it uses are pretty basic.

## Authors

* **Ahmad Pourihosseini** -  [ahmad-PH](https://github.com/ahmad-PH)

## Acknowledgments

* The idea of this project is inspired by the tensorflow tutorial on [generating text with an RNN](https://www.tensorflow.org/tutorials/text/text_generation) and that is also were the dataset is downloaded from.
