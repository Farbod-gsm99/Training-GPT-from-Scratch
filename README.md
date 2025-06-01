# Training-GPT-from-Scratch

In this project, I first trained a BPE tokenizer based on a vocab we got from the book "Wizard of OZ".
Then I wrote a basic GPT model with a decoder-only attention architecture.

The model code contains a GPT model class with simple forward and generate functions, added by attention blocks and a basic feedforward class.

The model was then trained on a corpus of data containing several textbooks and webpage scrapings.

The trained model fails to write readable answers to questions and doesn't seem to have much reasoning behind it, because of 2 reasons:
1. The amount of data used for pre-training was much less than what a basic GPT model with this block and batch sizes needs
2. The model block size was too small to be used for word generation task.

The model and all the other scripts attached were developed under the guidance of Elliot Arledge from freeCodeCamp
