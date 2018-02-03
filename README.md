# Sequence-to-Sequence Translation Model

Implementation of the [legacy seq2seq tutorial](https://www.tensorflow.org/versions/r1.0/tutorials/seq2seq)
adapted to the latest Tensorflow version. Original code used to be in
[`tensorflow/tensorflow/models/rnn/translate/`](https://github.com/tensorflow/tensorflow/tree/r0.7/tensorflow/models/rnn/translate)
package until the seq2seq model got replaced with [NMT](https://github.com/tensorflow/nmt).
Since then, the old model became only compatible with tensorflow not greater than 1.0.

This code in this repo gets updated to the latest tensorflow: it uses corresponding `tensorflow.contrib.legacy_seq2seq` API,
applies the patches where necessary (like [this one](https://github.com/tensorflow/tensorflow/issues/11157#issuecomment-353725791))
and in general keeps the model compatible with tensorflow updates.
