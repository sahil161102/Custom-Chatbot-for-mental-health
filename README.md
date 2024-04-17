
Generative-based Chatbots: Generative models do not rely on predefined responses. They come up with new replies from scratch. Machine Translation techniques are typically used in generative models, but instead of translating from one language to another, we "translate" from input to output (response). Generative models are used for the creation because they learn from scratch.


## Overview of the bots trained 
The dataset was picked up from Kaggle - [Mental Health FAQ](https://www.kaggle.com/narendrageek/mental-health-faq-for-chatbot). This dataset consists of 98 FAQs about Mental Health. It consists of 3 columns - QuestionID, Questions, and Answers. 

**Note that to train the retrieval chatbot, the CSV file was manually converted to a JSON file**. Since this is not the original dataset used for the research (read intro), I have used only the first 20 rows for training the model.
For generative-based chatbots, NLP was used since **NLP enables chatbots to learn and mimic the patterns and styles of human conversation**. It gives you the feeling that you are talking to a human, not a robot. It maps user input to an intent, with the aim of classifying the message for an appropriate predefined possible response.
- An encoder-decoder model was trained on the CSV file. Endoder-decoder is a seq2seq model, also called the encoder-decoder model uses Long Short Term Memory- LSTM for text generation from the training corpus.
- What does the seq2seq or encoder-decoder model do in simple words? It predicts a word given in the user input, and then each of the next words is predicted using the probability of likelihood of that word occurring. 

  
