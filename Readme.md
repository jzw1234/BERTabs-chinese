<h3>Abstractive summarization using bert as encoder and transformer decoder</h3>
I refer to this @https://github.com/IwasakiYuuki/Bert-abstractive-text-summarization
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


