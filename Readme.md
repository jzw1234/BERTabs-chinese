<h3>Abstractive summarization using bert as encoder and transformer decoder</h3>
I used other's document to obtain a BERTabs-chinese
I have used a text generation library called Texar , Its a beautiful library with a lot of abstractions, i would say it to be 
scikit learn for text generation problems.

The main idea behind this architecture is to use the transfer learning from pretrained BERT a masked language model ,
I have replaced the Encoder part with BERT Encoder and the deocder is trained from the scratch.

One of the advantages of using Transfomer Networks is training is much faster than LSTM based models as we elimanate sequential behaviour in Transformer models.

Transformer based models generate more gramatically correct  and coherent sentences.


<h3>To run the model</h3>
<pre>

Place the story and summary files under data folder with the following names.
-train_story.txt
-train_summ.txt
-eval_story.txt
-eval_summ.txt
each story and summary must be in a single line (see sample text given.)


Step1:
Run Preprocessing
<b>python preprocess.py</b>

This creates two tfrecord files under the data folder.

Step 2:
<b>python main.py</b>

Configurations for the model can be changes from config.py file


</pre>


