# Text-Generation-using-LSTM

<h3>TOPIC:</h3>
To develop a simple a simple LSTM network to learn sequences of characters from Alice in Wonderland.These experiments are not limited to text, you can also experiment with other ASCII data, such as computer source code, marked up documents in LaTeX, HTML or Markdown and more.
<br/>


<h3>Files Included:</h3>
1. saved weights large network: this contains saved models for different epochs for the bigger slightly more complex model<br/>
2. saved weights small network: this contains saved models for different epochs for the smaller and simpler model<br/>
3. shakerpere corpus : this folder contains differnt acts by shakespere classified by different genres in txt format. feel free to use this text to generate text in shakespere language<br/>
4. wonderland.txt : this is text format of the famous child novell alice in the wonder land. we had used this book for our predictive text generation<br/>


<h3>EXAMPLE:<h3>
here is an example of the text generated by the neural network.
"
‘what is a "
 larter ’ said the ming. ‘i dan to the thing the was to the thing the was to the thing the was a little said the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with the was oot a little sabbit with 
"
here we can see that the network is able to write well formed sequenses of words sometimes like "to the thing " but also makes spelling mistakes like rabbit is written as "sabbit" and too is witten as "oot"
<br/>

<h3>Tips to improve network performance: </h3>
1.Predict fewer than 1,000 characters as output for a given seed.<br/>
2.Remove all punctuation from the source text, and therefore from the models’ vocabulary.<br/>
3.Try a one hot encoded for the input sequences.<br/>
4.Train the model on padded sentences rather than random sequences of characters.<br/>
5.Increase the number of training epochs to 100 or many hundreds.<br/>
6.Add dropout to the visible input layer and consider tuning the dropout percentage.<br/>
7.Tune the batch size, try a batch size of 1 as a (very slow) baseline and larger sizes from there.<br/>
8.Add more memory units to the layers and/or more layers.<br/>
9.Experiment with scale factors (temperature) when interpreting the prediction probabilities.<br/>
10.Change the LSTM layers to be “stateful” to maintain state across batches.<br/>
