# Chatbot-Reddit

Chatbot that is trained on Reddit dump of 2005. This is a word level model which predicts the next sentence based on question statement and context (comments and replies in this case). The model uses encoder/decoder architecture and teacher forcing.

# Dependencies
* [Keras (Tensorflow Backend)](https://keras.io/)
* Numpy
* Scipy
* [Jupyter](http://jupyter.readthedocs.io/en/latest/install.html)

# Usage
1. Download and install Jupyter Notebook and IPython kernel
1. run a Jupyter environment locally using ``` jupyter notebook ``` in the terminal
1. call ``` load_model() ``` to load pretrained model in /models dir or train model for atleast 30 epochs
1. change temperature of output(random sampling coefficient) in ```sample()``` <br>
   (higher value of temperature = higher randomness, lower value of temperature preserves local structure but increases redundancy)
1. call ``` make_inference() ``` with question statements to generate outputs

# Example Output
```
Question: life
Reply: joke not did apparently best non wrong usually when call love you seriously 
```

# References
* [Keras Blog by Francois Chollet](https://blog.keras.io/a-ten-minute-introduction-to-sequence-to-sequence-learning-in-keras.html)

# TODO
* [] Train on dialog dataset for proper answer structure 
* [] Clean dataset for stop words using nltk library
<br>
<h6>
* The bot might say some offensive things(trained on reddit)
</h6>
