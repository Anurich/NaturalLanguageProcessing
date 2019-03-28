# NaturalLanguageProcessing

<p> Hello Everyone I have Made a simple program which help us to classify language , so for  example : if i say my name is Anupam , the model will predict it as english </p>

<b> How do i did it ?</b>
<p> Its very simple and easy first time it might look difficult but if u think in bit depth it will start making sense to you </p>

<ul>
  <li>Get the Data i have provided the file which has ['eng','spn','itl','due'] language its a file with full of text</li>
  <li>we need to preprocess the data what i did in the file is i remove the digits , i only consider word which is more than 2 in length , i perform the stemming and i seprate the label with the text </li>
  <li> Than i put the data into the data frame because if u see it in dataframe its easy to understand what u actually need to do</li>
  <li> so my data is [TEXT,LABEL] for every text i have label </li>
</ul>

<h3> Let's Move to next process </h3>
<p> But before that let me tell you we don't have machine that can understand the text so we basically we need to find the way to convert the data into numeric form so that we can feed that data into the neural network , or any other machine learning algorithm, By keeping this in mind we gonna start thinking how we can actually model the text into the numeric format . </p>

<b>
 a> We can find one hot encoding of the data but it's not good because one hot encoding don't tell you about the semantics of  the word it just assign 0 or 1 <br/>
b> We can use another approach which is term frequency approach instead of assign 1 or 0 we will assign the total number of time word occure divided by total values of the n_gram .
</b>


<ol>
  <li>
    I am finding the ngram of the sentence for example if i have sentence ['hello how are u'] -> ngram =2 for this sentence is going to be [('hello','how'),('how','are'),('are','u')..] 
  </li>
  <li>
    Once i have a bigram i can create a vocabulary which is the unique tuple in my bigram , and find the word to index mapping and index to word mapping .  
  </li>
  <li>
    one more thing to find the bigram i use library nltk , but before finding the bigram we need to tokenized the word we can use the library like nltk or keras preprocessing or anyother library   
  </li>
  <li>
    Now half the work is done we just need to start finding our [X,Y] and pass it through the machine learning algorithm or any deep learning algorithm   
  </li>
  <li>
      i created the vector of the same size of the unique vocabulary np.zeros(len(unique_vocab))  than i read sentence from the preprocessed text and for every sentence i converted it to bigram =2 and than find the frequency of each bigram after that I stack all the value into the array which become my X, and for Y i just replace the value from 0,1,2,3,4 
    
  </li>

</ol>
<b> Now everything is ready to work just create the model or architecture of your neural network and pass the X,y thourgh it and obtain the result </b>

I hope this will help!Thank You
