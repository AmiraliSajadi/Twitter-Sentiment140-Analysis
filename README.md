# Twitter-Sentiment140-Analysis
Binary classification of sentiment140 data set using LSTM neural network.<br/>


<p align="left">
  <img src="https://user-images.githubusercontent.com/48511939/127962271-673b57a8-8aaa-4907-86fb-8831d669d355.jpg", width=550/> 
</p> <br/>
          
The code classifies the text based on having positive or negative sentiment.<br/><br/>
The code consits of three major parts:<br/>
* Data pre-processing (Exploring, Cleaning, Tokenization, Lemmatization)
* Defining a costum embedding layer (using GloVe embedding)
* Creating a model, training the model and optimizing it.<br/>

The final product gives out predictions such as this:<br/>
![image](https://user-images.githubusercontent.com/48511939/127893581-681b708b-ffc7-4da9-90f8-f51dd2dd363f.png)<br/>
where numbers close to 1 indicate a positive statement and numbers closer to 0 indicate the opposite.<br/><br/>


Further explenation is given in the notebook on each part.
