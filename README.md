![banner](https://github.com/lorainemnrc/llm-nanogpt/assets/23328647/d77ee7e1-d0a2-4436-bffe-dad249d48896)

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

<h1 style="color: #1048CB"><b>Highlights</b></h1>

<p align="justify"> &emsp;
   I looked at 3 cases when experimenting with hyperparameter tuning - (1) increasing the number of iterations, (2) increasing the "block size" or the sequence length for each training sample, and (3) increasing the number of attention heads in the multi-head attention mechanism.
</p>

<p align="justify"> &emsp;
   Results show that increasing the maximum number of iterations generated the most significant decrease in validation loss vs. the baseline model among the scenarios explored. However, it's important to note that this improvement comes at the expense of a longer run time. The increased number of iterations led to a doubling of the training time, taking ~12 mins. compared to the baseline's ~6 mins.
</p>

<p align="justify"> &emsp;
   This trade-off between improved performance and increased computational time is a common consideration in training machine learning models. It is crucial to assess whether the performance gains obtained by increasing the number of iterations justify the additional time investment. The decision to increase the maximum number of iterations should be made based on the specific requirements of the task, the available computational resources, and the desired balance between model performance and efficiency.
</p>
