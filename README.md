# UU_SwedishNovels_1800-1940
A corpus of Swedish literary novels and collections of short stories from 1800–1940. 

This repository contains a corpus of Swedish literary novels and collections of short stories from 1800–1940. The data is sourced from [Litteraturbanken](https://litteraturbanken.se/). The works selected to fulfill the following criteria:
* From the period 1800–1940
* Written in Swedish; no translations are included
* Not written by a Finland-Swedish author
* Available in proofread OCR from Litteraturbanken
* Available under an open license (CC_BY or CCO)

## Data and formats
The original data from Litteraturbanken is available as XML-files, describing the page layout of the works. This corpus contains the text extracted from the works and automatically analyzed versions.  The data is available in two formats:
* Text 
  - Raw text with light XML formatting
* Parsed
  - Automatically analyzed data in CoNLLU format:
     * Sentence segmented, tokenized, and lemmatized by the [Swedish annotation pipeline](https://github.com/robertostling/efselab)
     * Part-of-speech tagging, morphological analysis, and dependency parsing by [Machamp](https://github.com/machamp-nlp/machamp)
   
Machamp was trained on Swedish-Talbanken for the XPOS-tags, and for dependency parsing and UPOS-tags on a combination of Swedish: Talbanken and LinES, Norwegian: Bokmaal, Nynorsk, NynorskLIA, and Danish-DDT. See [Universal Dependencies](https://universaldependencies.org/) for an overview of the treebanks, and this paper for an overview of the training:

Sara Stymne, Carin Östman, and David Håkansson. [Parser Evaluation for Analyzing Swedish 19th-20th Century Literature](https://aclanthology.org/2023.nodalida-1.35.pdf). In Proceedings of the 24th Nordic Conference on Computational Linguistics (NoDaLiDa). Pages 335-346. May 22–24, 2023. Tórshavn, Faroe Islands.

Two types of works are included. Original works from Litteraturbanken and text-critical editions of original works, from which we have extracted only the text of the original work, and excluded editor comments, word lists, et.c. Metadata for all works are available in the files:
* original-work-overview.txt
* text-critical-work-overview.txt


## Acknowledgements
This work is funded by the Swedish Research Council under project 2020-02617: *Fictional prose and language change. The role of colloquialization in the history of Swedish 1830–1930*. 

Thank you to Johan Roxendal at Littaraturbanken for help extracting the original files.

## Contact
This corpus was created by Sara Stymne, David Håkansson, Carin Östman, and Johan Svedjedal at Uppsala Unviersity
Contact email: sara.stymne@lingfil.uu.se
