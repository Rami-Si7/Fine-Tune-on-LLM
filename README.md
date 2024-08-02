# Fine-Tune-on-LLM
Given a dataset of courses from Coursera Courses &amp; Skills dataset 2024. We want to generate course titles based on skills. To achieve our goal, we are going to fine tune a large language model on the dataset to generate course titles.
Our approach was to use the pre-trained FLAN-T5-base Model with SEQ2SEQ LM encoder-decoder architecture.
We loaded the data and splited it to train and test.
We defined a custom class that process the data and tokenize it.
We used tokenizer from AutoTokenizer and passed it to the class to tokenize the data.
We fine-tuned the pre-trained model on the given dataset by training.
For training, we used defined Seq2SeqTrainingArguments and passed them to Seq2SeqTrainer to train
We evaluate the model.
