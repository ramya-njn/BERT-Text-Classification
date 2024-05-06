# What is BERT?

BERT, Bidirectional Encoder Representation from Transformers, is a language model that is trained on a large corpus of unlabelled data. Unlike the earlier NLP approaches like word2Vec, BERT captures contexutal representations in a bidirectional manner. This implies that it takes into account the previous and the next word to encode a given word in a sentence generating contextually meaningful word embeddings.

# BERT Architecture

BERT is a stack of Transformer encoder layers. Each encoder layer consists of multiple self-attention heads wrapped with a residual connection followed by layer normalization. The combined multi-head self attention output is fed to a feed-forward fully connected layer that is also with a residual connection followed by layer normalization. BERT models are pre-trained on two tasks: Masled Langugae Modelling (MLM) and Next Sentence Prediction (NSP). The pre-tranied model can be later fine-tuned on various tasks such as text classification, NER, question answering etc. For fine-tuning, one or more fully connected layers are added to the final encoder layer.

# Fine Tuning Approaches
Fine tunining involves taking a pretrained model and adapting it to a new task using task-specific datasets. The focus of this repository is on fine tuning a text classification model via are three approaches:

  i.   Tensorflow Keras
  
  ii.  Pytorch
  
  iii. Hugging Face Trainer API
