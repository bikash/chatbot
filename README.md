# chatbot
seq2seq chatbot in python using Tensorflow. Tensorflow is one of the best deep learning algorithm till date. 


## Setup


* Create temporary working directory prior to training

```bash
mkdir working_dir
```

* Download test/train data from Cornell Movie Dialog Corpus

```bash
cd data/
bash pull_data.sh
```

## Training

```bash
# edit seq2seq.ini file to set 
#		mode = train
python execute.py
# or use custom ini file
#		python execute.py my_custom_conf.ini
```

## Testing

```bash
# edit seq2seq.ini file to set 
#		mode = test
python execute.py
```

## Serve

```bash
# configuration : seq2seq_serve.ini
python ui/app.py
# wait until this message shows up
#		"Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)"
# open up the address in browser, chat with the bot
```

