


<h1 style="color: #1048CB"><b>Overview</b></h1>

<p align="justify"> &emsp;
Language models (LM) are statistical models that estimate the probability distributions of linguistic units, such as words or sentences. There are two main categories of language models: count-based models, also known as N-gram LMs, and continuous space models like Neural LMs.
</p>

<p align="justify"> &emsp;
Transformers and attention mechanisms are architectural components that a Language model can use to capture context and relationships between words or positions in a sequence. Some of the common applications of LMs are text completion and generation, machine translation, sentiment analysis, and  text summarization.
</p>

<p align="justify"> &emsp;
For this exercise, we explore applications of language models with the following learning objectives in mind:
</p>

<p align="justify"> &emsp;
1. What is a language model?

2. Describe the dataset being used. What preprocessing steps need to be done in preparation for training the model?
   
3. What is self-attention?
   
4. Compare and contrast the concept of attention, self-attention, and cross-attention.
   
5. What is multi-head attention?
    
6. What is a transformer?
    
7. Describe the other components of a transformer: residual connections, layer normalization, and dropout. What purpose do each of them serve?
    
8. Tune the nanoGPT model (e.g., add more epochs, adjust batch size, learning rate, embedding dimensions, dropout, other hyperparameters, etc.). Compare a set of generated samples from before and after your tuning.
    
9. As you experiment with tuning, describe your thought process. Which hyperparameters did you decide to adjust? What were your hypotheses for how it would affect the model?
</p>


<h1 style="color: #1048CB"><b>Data Source</b></h1>
The project uses a sample subset of the [`Tiny Shakespeare`](https://cs.stanford.edu/people/karpathy/char-rnn/) dataset consisting of around **1.1M** characters and **65** unique characters extracted from the literary works of William Shakespeare.
