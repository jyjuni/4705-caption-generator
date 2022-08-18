# Image Captioning with Conditioned LSTM Generators

Repo for HW5 - NLP Summer 2022 @ Columbia University

## Overview

This project is consists of the following components:

- Create matrices of image representations using an off-the-shelf image encoder.
- Read and preprocess the image captions.
- Write a generator function that returns one training instance (input/output sequence pair) at a time.
- Train an LSTM language generator on the caption data.
- Write a decoder function for the language generator.
- Add the image input to write an LSTM caption generator.
- Implement beam search for the image caption generator.

## Model

The conditional generator takes in encoded text and encoded image vector as input. Image vectors are encoded using InceptionV3. The encoded image is taken as additional context input and feed into a customized bi-LSTM generator.



<img src="README.assets/Screen Shot 2022-07-27 at 5.38.49 PM.png" alt="Screen Shot 2022-07-27 at 5.38.49 PM" style="zoom:50%;" />

## Reference
http://www.phontron.com/slides/nlp-programming-en-13-search.pdf
