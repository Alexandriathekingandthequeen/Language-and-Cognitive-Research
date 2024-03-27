# Language-and-Cognitive-Research

## Overview
This project, supervised by Dr. Catherine Sandhofer and led by graduate student Erjing Zhang, focuses on the cognitive aspects of language acquisition in children. Utilizing text mining and visualization tools, we explore how young children use adjectives to describe various referents in picture-reading activities.

## Team Members
- Dr. Catherine Sandhofer (Supervisor)
- Erjing Zhang
- Qilin Zhou
- Shalmalee Joshi

## Data Source
We analyzed 33 counterbalanced transcripts from the CHILDES database, specifically from Gelman's 2014 individual differences corpus. The transcripts are based on picture-reading activities involving one-referent pictures, conducted between children and their parents.

Participants included children, aged between 3 years and 9 months to 4 years and 11 months (average age 4 years and 4 months), along with their parents, totaling 72 child-parent pairs. Each pair participated in recordings of their interactions, as well as interactions between each individual and a researcher, during two laboratory visits spaced three to four weeks apart. Consequently, each pair contributed to six distinct interaction scenarios: Child-Parent for the first visit (C-P1), Child-Parent for the second visit (C-P2), Child-Researcher for the first visit (C-R1), Child-Researcher for the second visit (C-R2), Parent-Researcher for the first visit (P-R1), and Parent-Researcher for the second visit (P-R2). During these interactions, participants engaged with a 15-page picture book without text, which featured an equal distribution of images depicting animals, foods, and humans.

- [Project Description for 2014 - Individual Differences Project](https://childes.talkbank.org/access/Eng-NA/Gelman.html)
<p align="center">
  <img src="king.png" width="400"><br>
  <em>Social Referent-King</em>
</p>

<p align="center">
  <img src="penguin.png" width="400"><br>
  <em>Animal Referent-Penguin</em>
</p>

<p align="center">
  <img src="ice-cream.png" width="400"><br>
  <em>Food Referent-Ice Cream</em>
</p>

  

## Text Mining Methodology
1) spaCy Parsing to get referent-adj dictionary
- **spaCy**: For text mining, specifically focusing on the use of adjectives for each referent in the pictures, including n-grams analysis for adjectives and nouns. In SpaCy, a Transformer (TRF) model leverages a neural network architecture that has been pre-trained on a large corpus of text using self-attention mechanisms. Hence, we use spacy.load("en_core_web_trf").

2) N-distance analysis for adj-noun pairs
- **bigram within a specified distance**: Although 
2) Network Visualization
- **Pyvis**: To visualize the associations between adjectives and different types of referents (e.g., social, food, animals).



## Sample Visualization
- ![Adjs Across Categories by spaCy](https://github.com/QilinZhou56/Language-and-Cognitive-Research/blob/main/referential_communication/Result/general_adj_freq_Spacy.png)
- ![N_grams](https://github.com/QilinZhou56/Language-and-Cognitive-Research/blob/main/referential_communication/Result/n_grams_viz.png)
- ![Food Adjs Frequency](https://github.com/QilinZhou56/Language-and-Cognitive-Research/blob/main/referential_communication/Result/food_adj_freq.png)
  
[View Pair-wise Association](https://htmlpreview.github.io/?https://github.com/QilinZhou56/Language-and-Cognitive-Research/blob/main/referential_communication/Result/food_adj_referent.html)

If not worked properly, you could reference [HTML](https://github.com/QilinZhou56/Language-and-Cognitive-Research/blob/main/referential_communication/Result/food_adj_referent.html)

## Findings
Our findings reveal interesting patterns in the use of adjectives by four-year-old children:
- For food referents, children commonly used color, size, and taste adjectives, while **quality or functional adjectives were less frequent**.
- In describing human referents, children focused more on perceptual features and **less on inherent qualities like "alive", "good", or "kind"**.
- There was a larger variety of adjectives used for food referents compared to human referents, indicating a **protracted process in adjective usage** relative to noun acquisition.

## Cross-Validation
1. We extended our research by conducting cross-validation with other linguistic transcripts. This further established spaCy transformers as a robust tool for identifying parts of speech and analyzing language patterns in young children, with consistent 90% **baseline** accuracy. 
2. We will **continue improving** this model with modification regarding dependency and classification threshold, and training methods of existing files.

## Conclusion
Our project contributes to understanding how children's language and cognitive abilities develop, particularly in the context of adjective usage in descriptive tasks. These insights can be crucial for further research in developmental psychology and linguistics.

## Acknowledgments and Confidentiality
We would like to thank all contributors and participants involved in this research project. The two sample data, if used, should inform us for research confidentiality purposes.
