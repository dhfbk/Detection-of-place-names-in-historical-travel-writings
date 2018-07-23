# Detection-of-place-names-in-historical-travel-writings
We manually annotated a corpus of 100,000 tokens taken from a collection of English travel writings (both travel reports and guidebooks) about Italy published in the second half of the XIX century and the ’30s of the XX century. The corpus is annotated in BIO format using the tag LOCATION to mark all named entities (including nicknames) referring to: (i) geographical locations; (ii) political locations; (iii) functional locations.

The corpus has been used to retrain the Stanford NER module (https://stanfordnlp.github.io/CoreNLP/ner.html) and to train new models using the neural architecture proposed by Reimers and Gurevych (https://github.com/UKPLab/emnlp2017-bilstm-cnn-crf) tested with several pre-trained word embeddings.

 - The *NER_Travel* folder contains the annotated texts divided into training, development and test sets. After setting up the neural architecture, just copy the folder in the "data" folder of the neural implementation to replicate the experiments.
 - GloVe, Levy and FastText embeddings are available on the websites of the corresponding projects.
 - Historical embeddings are available in a shared Google Drive folder: https://drive.google.com/drive/folders/1FHuAwS9T0jPd1Bn6eW2BSFF_AiqB1KTK?usp=sharing
 - Our best model, obtained with HistoGloVe embeddings, is a shared Google drive folder: https://drive.google.com/drive/folders/1cPIrz0MexPq_8GG1BWl1okXYDDOqsS9Z?usp=sharing. You can run this model on your own data using the script *RunModel.py* provided with the neural architexture. 
 - The full collection of travel writings, from which the annotated corpus is extracted, is released in a dedicated website: https://sites.google.com/view/travelwritingsonitaly/
