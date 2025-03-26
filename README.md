# codebert_gec
'''
This GitHub project aims to provide an open-source implementation of the proposed method for automatically annotating code errors with improved accuracy.
'''
The Seq2editErrorAnnotator project encompasses a meticulously preprocessed dataset and an integrated codebase designed to facilitate the study of error annotation in coding. 
This repository contains everything needed to train, test, and evaluate various annotation methods using the CodeBERT model.
Users are encouraged to read the README file to understand the prerequisites, setup instructions, and step-by-step guide on how to run the code and interpret the results. 
The repository is designed to be user-friendly, ensuring that even newcomers can quickly grasp how to work with the data and code provided.
Objective: This project aims to provide a comprehensive resource for researchers and developers interested in exploring advanced error annotation techniques in coding, leveraging the power of CodeBERT for enhanced accuracy and efficiency.
Outcomes:By utilizing the Seq2editErrorAnnotator, users can expect to gain a deeper understanding of how different annotation methods impact the performance of the CodeBERT model, leading to more informed decisions in their own projects and research.
Note: The accuracy results provided are based on the preprocessed dataset and may vary with different datasets or configurations. It is recommended to review the methodology and adapt the code as needed to suit specific requirements or explore additional annotation techniques.
'''

### required Library
'''
pip install allennlp==1.3.0
pip install ltp==4.1.3.post1
pip install OpenCC==1.1.2
pip install pyarrow
pip install python-Levenshtein==0.12.1
pip install numpy==1.21.1
pip install transformers
'''

### pre-trained model weights
The pretrained codebert model was stored in ./data/codebert/  which named as pytorch_model.bin
```

###Quick Start: Trainng model and predicting model
Please find detail in Untitled.ipynb，

First, copy the required model to the specified directory, and then run the prediction or training directly through Untitled.ipynb.


### The .\tag folder contains all the tagging methods.
tag_word.py  #Word_based method
tag_span.py #Span_based method
tag_seq.py  #Statement_based method
compare.py #Manual Annotation Comparison
convert_tag_codebert.py #Tag convert
