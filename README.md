<h2>Language Classification</h2>
<p> I have Made a simple program which help us to classify language , so for  example : if i say my name is Anupam , the model will predict it as english </p>
<h2> Dataset Structure. </h2>
  <ul>
    <li>Y:X ->  Data file contain label and its corresponding sentences. For example ("eng"-"hello how are you")</li>
  </ul>
<h2> Project Overview ?</h2>
<ul>
  <li>You can use the Data I have provided, which consist of sentences in  ['eng','spn','itl','due']. </li>
  <li>In preprocessing step, I only consider word which are more than 2 in length as well use nltk stemming.</li>
  <li> Rearrange the data after preprocessing step now data looks something like [TEXT,LABEL]</li>
  <li> I use simple feed forward network to feed the data.</li> 
</ul>
  <h2>Data Preprocessing</h2>
  As discuss above, I only consider the word which has length more than 2 as well as converting word to stemming using nltk library.
  Next I create word to index and index to word dictionary of bigram words, which consist of frequency of bigram words i.e. how many times certain word occur in the text.
  Since now I have the dictionary, I can use this to convert the text data to numerical data. which I can later feed into my model. 
  
  <h2>Discussion.</h2>
  Its a small project, it was made to play around with natural language processing approaches.
