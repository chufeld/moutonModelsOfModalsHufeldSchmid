# moutonModelsOfModalsHufeldSchmid
Code repository for the paper on modal verbs in the BNC2014 by Clemens Hufeld and Hans-Jörg Schmid

This repository contains some of the code and full model results of the publication 

Hufeld, Clemens and Hans-Jörg Schmid "Does the intersubjectivity of modal verbs boost inter-individual differences?" 
in Models of Modals - from Pragmatics and Corpus Lingustics to Machine Learning,
Ilse Depraetere, Bert Capelle, Martin Hilpert, Ludociv De Cuypere, Mathei Dehouck, Pascal Denis, Susanne Falch, Natalia Grabar, Cyril Grandin, Thierry Hamon, Clemens Hufeld, Benôit Leclercq and Hans-Jörg Schmid (Eds.)
De Gruyter, 2023.

The investigation is focussed on modal verbs in spoken British English. The data used for this publication is taken from the BNC2014.
See:

Love, R., Dembry, C., Hardie, A., Brezina, V. and McEnery, T. (2017). 
The Spoken BNC2014: Designing and building a spoken corpus of everyday conversations. International Journal of Corpus Linguistics, 22(3), 319-344.

The full data cannot be reproduced here, as the licence of the BNC2014 does not allow the reproduction of the corpus.

As of now, some of the analysis code is published here, without the data used. The full corpus used for our research can be downloaded here: 
http://corpora.lancs.ac.uk/bnc2014/signup.php

The document 20211006_model_results_publ contains the quasipoisson model results of all bigrams used. The model tested for gender, agerange, educationl and social grade.

The startig point was the data from the BNC website. The entire BNC2014's XML structure was parsed to extract the entire corpus as a CSV file. 
The resulting CSV file is around 600MB. All the Jupyter Notebooks contain Python Pandas code that manipulates the full BNC2014 data 
into one dataframe for each construction, in which each modal occurrence is listed with its appropriate context (no context, one word to the left or to the right, 
two words to the right) indivudally by speaker and contains the speaker's metadata. 

The Jupyter Notebook "extracting comparison ngrams from BNC.ipynb" contains the code used to extract the non-modal constructions from the BNC2014 dataframe.

