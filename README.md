# Transformers LSTM with XGBRegressor
My proposed model can perform regression to predict the evaluation of grammatical coherence, vocabulary, and grammatical conventions, assigning a score between 1 and 5 to each criterion. Instead of treating the task as a classification problem, I approach it as a regression issue.

To improve my model's performance, I used a transfer learning approach that trains the model sequentially to gradually gain experience. I modified the proposed model to train in the order of syntax, cohesion, vocabulary, phraseology, grammar, and conventions. During training, the model learned to evaluate syntax first and used that experience to train in evaluating cohesion, then vocabulary, and so on.

My methodology leverages the gradual manner in which young children learn new concepts based on their knowledge of previous concepts. By following a similar approach, I achieved a more efficient model with a lower error rate. The order of teaching the model is crucial to the success of the approach. I trained my model in the sequence [syntax, cohesion, vocabulary, phraseology, grammar, conventions], but changing the order based on the sequence of concepts in education could yield even better results.


# Proposed neural network model:
![download - 2023-01-09T122800 186](https://user-images.githubusercontent.com/108609519/211287619-0a4c31b1-ef24-4bc2-b374-b434e110ff57.png)




The learning transfer sequence used in the model resulted in lower error rates at the beginning of each epoch for a new case compared to starting training from scratch. As a result, the model achieved significantly better results than the previous concept.
