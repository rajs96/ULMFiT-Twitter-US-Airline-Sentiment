# ULMFiT Twitter Sentiment Analysis - US Airlines

In this repo, we're going to apply a ULMFiT approach to predict sentiment towards an airline based on a Tweet. The ULMFiT approach was devised by Jeremy Howard and Sebastian Ruder, and it's essentially a transfer learning approach for NLP. 

I wanted to focus as much as I could on explanations that were both intuitive and detailed. If you're not particularly advanced with deep learning and reading research papers, it can be really hard to balance out all the moving parts in a cutting-edge AI problem/solution. I'm confident that anybody can do it, but the process can be inefficient and frustrating if you don't know what you're looking for. 

**This repo focuses on the problem-solving, intuitions, and actual process of applying ULMFiT to a novel problem**.

There are three notebooks in this repo that are of interest:

## Twitter US Airline Sentiment Classification - Understanding the problem background
(Background_info.ipynb)
In this notebook, we'll talk about domain of NLP, more specifically text classification. We'll understand what the initial approaches were, and why a ULMFiT approach is better. Reading this is key to understanding why language modeling is an effective transfer learning approach for NLP.

## ULMFiT Approach
(ulmfit_runthrough-explanation.ipynb)
A run-through of the ULMFiT approach to the Twitter dataset, and explanations throughout.

## ULMFiT Results/Discussion
(ulmfit_results.ipynb)
Functions to produce results with the Twitter dataset, and an analysis of our results (we don't go through every possible combination of hyperparameters, so most of it is just result reporting). We'll also talk about some of the shortcomings of the model and how we might improve going forward.

## References
- "Universal Language Model Fine-tuning for Text Classification": https://arxiv.org/abs/1801.06146
- "Regularizing and Optimizing LSTM Language Models": https://arxiv.org/abs/1708.02182
- "A Comparison of Pre-processing Techniques for Twitter Sentiment Analysis: https://link.springer.com/chapter/10.1007/978-3-319-67008-9_31
- "How transferable are features in deep neural networks?": https://arxiv.org/abs/1411.1792
- "A disciplined approach to neural network hyper-parameters: Part 1 -- learning rate, batch size, momentum, and weight decay": https://arxiv.org/abs/1803.09820 
- "Grokking Deep Learning" - https://www.manning.com/books/grokking-deep-learning
- Andrew Ng's Deep Learning course: https://www.coursera.org/specializations/deep-learning
- Stanford's Deep Learning for NLP course: https://cs224d.stanford.edu/
- fastai documentation: https://docs.fast.ai/
- fastai course: https://course.fast.ai/
- Finding an optimal learning rate: https://sgugger.github.io/how-do-you-find-a-good-learning-rate.html


## Some key corrections
### ulmfit_runthrough_explanation
- When fine-tuning the language model, when we initialize the Learner with 'language_model_learner', the comment above should read "pass in **drop_mult=0.3** to specify that our dropouts for the model are with p = 0.3"
- In the code cell under "Getting back to the big picture, the comment should read "as discussed before, we choose **'1e-2'** because it's slightly **smaller** than the minimum loss LR"

