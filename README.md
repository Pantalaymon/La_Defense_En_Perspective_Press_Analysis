# La_Defense_En_Perspective_Press_Analysis
Presse analysis of the representations of "La Défense" During Master 2 Internship


In this repository you'll find the following directories and files:

- corpus
  - Toutes_mentions_Defense_EN.csv : 
  - Toutes_mentions_Defense_FR.csv
  - grandfinal_EN_indexé.xml : Semi-manually tagged english press corpus. The mentions of "La Défense" and its meronyms (locations inside La Defense) are surrounded by xml tags
  - grandfinal_EN_annoté.xml : Final english corpus. Same as above with supplemented with semantic annotations in the element attributes. Those annotations are the work of a team of annotators
  - grandfinal_FR_indexé.xml : Semi-manually tagged french press corpus. The mentions of "La Défense" and its meronyms (locations inside La Defense) are surrounded by xml tags
  - grandfinal_FR_annoté.xml : Final French corpus. Same as above with supplemented with semantic annotations in the element attributes. Those annotations are the work of a team of annotators

- detection_designations 
  - Detection_Designations_Defense_Camembert.ipynb : Training of a CamemBERT-based token classification (NER) to detect the mentions of "La Défense" in a french press corpus
  - Detection_Designations_Defense_RoBERTa.ipynb : Training of a RoBERTa-based token classification (NER) to detect the mentions of "La Défense" in an english press corpus
  - Detection_Designations_Defense_neuralcoref_EN.ipynb : detection of mentions of "La Défense" in english presse with a rule-based method using the 'neuralcoref' coreference module
  
- classiication_typologie :
  - Classification_typologie_contexte.ipynb : Training of CamemBERT-based classification models to predict the semantic annotations related to the predication surrounding the french mentions
  - Classification_typologie_contexte_EN.ipynb : Training of RoBERTa-based classification models to predict the semantic annotations related to the predication surrounding the english mentions
  - Classification_typologie_designations.ipynb : Machine learning and rule-based classification models to predict the semantic annotations related to the french mentions's features
  - Classification_typologie_designations_EN.ipynb : Machine learning and rule-based classification models to predict the semantic annotations related to the english mentions's features
  - Extraction_features_classification_designations.ipynb : generation of wor2vec representations and word2vec-based expert features to be fed to the models above. French
  - Extraction_features_classification_designations_EN.ipynb : generation of wor2vec representations and word2vec-based expert features to be fed to the models above. English
