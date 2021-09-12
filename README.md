# Text Sentiment Classification using BERT

Text sentiment classification on IMDB moview reviews dataset using BERT model.

The model is built by preprocessing the text using a BERT english preprocessor, followed by feeding the tokenized input to the small pretrained BERT model, and finally a Dropout and Dense layer for the prediction. The model is optimized by implementing and using the [AdamW](https://arxiv.org/abs/1711.05101), an Adam optimizer with weight decay regularization and custom learning rate scheduler used in the [BERT paper](https://arxiv.org/abs/1810.04805).

The small BERT model is fine-tuned and the model is trained on the IMDB train set, and after 5 epochs the model yields 86% test accuracy.

### References
- [BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding](https://arxiv.org/abs/1810.04805)
- [Large Movie Review Dataset](https://ai.stanford.edu/~amaas/data/sentiment/)
