# ULMFiT Twitter Sentiment Analysis

In this repo, we're going to apply a ULMFiT approach to predict sentiment towards an airline based on a Tweet. The ULMFiT approach was devised by Jeremy Howard and Sebastian Ruder, and it's essentially a transfer learning approach for NLP. 

I wanted to focus as much as I could on explanations that were both intuitive and detailed. If you're not particularly advanced with deep learning and reading research papers, it can be really hard to balance out all the moving parts in a cutting-edge AI problem/solution. I'm confident that anybody can do it, but the process can be inefficient and frustrating and if you don't know what you're looking for. 

There are three notebooks in this repo that are of interest:

## Twitter US Airline Sentiment Classification - Understanding the problem background
(Background-info.ipynb)
In this notebook, we'll talk about domain of NLP, more specifically text classification. We'll understand what the initial approaches were, and why a ULMFiT approach is better.

## ULMFiT Approach
(ulmfit-runthrough-explanation.ipynb)
A run-through of the ULMFiT approach to the Twitter dataset, and explanations throughout.

## ULMFiT Results/Discussion
(ulmfit-results.ipynb)
Functions to produce results with the Twitter dataset, and an analysis of our results (we don't go through every possible combination of hyperparameters, so most of it is just result reporting). We'll also talk about some of the shortcomings of the model and how we might improve going forward.

## References
- "Universal Language Model Fine-tuning for Text Classification": https://arxiv.org/abs/1801.06146
- "Regularizing and Optimizing LSTM Language Models": https://arxiv.org/abs/1708.02182
- "A Comparison of Pre-processing Techniques for Twitter Sentiment Analysis: https://link.springer.com/chapter/10.1007/978-3-319-67008-9_31
- Andrew Ng's Deep Learning course: https://www.coursera.org/specializations/deep-learning
- Stanford's Deep Learning for NLP course: https://cs224d.stanford.edu/
- fastai documentation: https://docs.fast.ai/
- fastai course: https://course.fast.ai/
- https://link.springer.com/chapter/10.1007/978-3-319-67008-9_31
