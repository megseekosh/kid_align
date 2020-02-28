# kid_align

Forced aligners, trained on largescale child speech corpora, that are more successful than adult models. 

Montreal forced aligners (MFAs) trained on controlled child speech in English and Quechua (word list readings). Stay tuned for child Spanish aligner. 

Some quick instructions:

1) Download the MFA (https://montreal-forced-aligner.readthedocs.io/en/latest/installation.html) (McAuliffe et al., 2020) and move to directory where it is now stored. 

2) Move the language model (e.g. `child_English.zip`) to the same directory as the MFA. 

3) Create a language dictionary with an entry for each lexical item to be aligned. Example of the Quechua dictionary included in repo. 

4) Run the following:

`bin/mfa_align corpus_directory dictionary_path language_model output`

where `corpus_directory` is the directory containin each speaker's textgrid and .wav files;

`dictionary_path` is the dictionary for the language you are aligning

`language_model` is the zip file containing the aligned model

and `output` is the folder where you would like the aligned textgrids to go

Quechua_dict.txt - Dictionary used for Quechua training 


McAuliffe, M., Socolof, M., Mihuc, S., Wagner, M., and Sonderegger, M. (2020). Montreal Forced Aligner [Computer program]. Version 1.1.0.

