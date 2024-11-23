## Chatur-GPT

- This project is an implementation of the **`Attention is all you Need`** paper.

  

## Model Description
- **Transformer Based (124M):** 
    Chatur-GPT is a Generative Pre-Trained model built from scratch which is trained on a multilingual dataset, enabling effective translation across various languages.

- **Visualization:**  Added an **attention visualizer** to dynamically  display the attention patterns of the pre-trained model, providing insights into how the model interprets and prioritizes different parts of input sequences.

- **Dataset:** The model has been trained on **`Opus Books`** a Multilingual dataset imported from [![Link](https://img.shields.io/badge/Hugging%20Face-FFD21E?logo=huggingface&logoColor=000)](https://huggingface.co/datasets/Helsinki-NLP/opus_books)

- **Metrics:**  The model has been trained for 20 epochs and the weights have been stored which are later used for inference and visualization. A wordlevel tokenizer has been used for text pre-processing and an input embedding of **`512`** dimensions is used for spatial positioning. The model was able to achieve a **BLEU** score of **`0.68`**, indicating strong translation accuracy and context preservation across languages.



## How to run

* Install the requirements.
```bash
pip install -r requirements.txt
```
* To inference the model, run Inference.ipynb
```bash
run Inference.ipynb
```
* To change the language of translation
```bash
>> Go to config.py
>> Change "lang_tgt" to desired language (the parameters are customizable)
```

* To train the model
```bash
python train.py
```
*Note:* The code written is device agnostic (can run on both a cpu and a gpu)



## Architecture
![Transformer_img](https://github.com/user-attachments/assets/4a7d0052-2d8f-4473-8811-44f2b9ff8780)



## Overview
![Transformer](https://github.com/shubh-man007/Projects/blob/main/ChaturGPT/transform20fps.gif)

[![GoogleAI](https://img.shields.io/badge/Google-4285F4?logo=google&logoColor=white)](https://3.bp.blogspot.com/-aZ3zvPiCoXM/WaiKQO7KRnI/AAAAAAAAB_8/7a1CYjp40nUg4lKpW7covGZJQAySxlg8QCLcBGAs/s1600/transform20fps.gif)  



## Output
![Output](https://github.com/user-attachments/assets/8df960ab-9d7c-4bf8-b635-3e2df0d29081)
* Check the output.txt file for more examples (en-it translation)

*Note:* The output can be syntactically and semantically enhanced by running it for more epochs ~ 30.

## Attention Visualizer

![visualization](https://github.com/user-attachments/assets/01663fca-92c1-438a-bbd1-f1a66a6eb102)

