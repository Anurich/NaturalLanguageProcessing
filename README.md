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
 a> We can find one hot encoding of the data but it's not good because one hot encoding don't tell you about the semantics of  the word it just assign 0 or 1 
b> We can use another approach which is term frequency approach instead of assign 1 or 0 we will assign the total number of time word occure divided by total values of the n_gram .
</b>


<ol>
  <li></li>

</ol>
