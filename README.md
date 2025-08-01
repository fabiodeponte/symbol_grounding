# Grounding Words in Visual Perceptions

Abstract

In recent years, Natural Language Processing models have shown compelling progress in generating and translating text. Yet, the symbols that are manipulated by these models are not produced within the models themselves. On the contrary, they are externally given in the form of tokens. The models only measure the probability that a specific token comes after another (or a group of others) and allow the generation of a list of tokens, each of which has a certain probability of following the previous one. There is no connection to sensory perceptions, and the semantic interpretation of the outputs – as well as of the inputs – of these models is completely invisible to the system that produces them. Therefore, language cannot be used by the system to manipulate information about the perceived world. This is commonly referred to as the Symbol Grounding Problem and, as of today, there is not a generally accepted procedure to solve it. This paper explores a possible solution: a sequence-to-sequence model trained over videos characterised by visual elements which reliably predict the presence of acoustic co-occurring elements. A dataset was created ad-hoc, with videos that include 5 types of objects and 5 actions. Two research questions were considered: whether such a model could map video features onto audio features, in fact producing a categorization without labels, where the categories would emerge from the parallel, simultaneous generalization of both input and target; and whether the model would be able to combine learned information about objects and movements to correctly describe a new combination, shown in a video it was not exposed to during training, a process that is referred to as compositional semantics. The experiment showed that the model was able to generalize simultaneously over videos and over the utterances that were paired with them. Further, it produced sentences that were in some cases more accurate than the original ones, precisely because of the process of generalization. However, the results suggest also that the model did not develop the ability to combine information taken from different samples. In other words, while symbol grounding seems to have been achieved, compositional semantics does not. The experiment shows that sensory perceptions can be mapped onto one another with a sequence-to-sequence model trained over a dataset where elements coming from different sensory domains are paired. However, it is not sufficient to develop compositional semantics.


The **paper** was published in the Proceedings of the Sixth Workshop on Natural Language for Artificial Intelligence (NL4AI 2022) co‑located with 21th International Conference of the Italian Association for Artificial Intelligence (AIxIA 2022), Udine, Italy, 28 Nov. ‑ 2 Dec., 2022.: https://ceur-ws.org/Vol-3287/paper6.pdf


The **complete project**, the text of the final **thesis** for the MSc of Data Science and Artificial Intelligence: https://github.com/fabiodeponte/symbol_grounding/blob/main/grounding_words_visual_perceptions.pdf (2022).


The **dataset**: https://www.kaggle.com/datasets/fabiodeponte/symbolgrounding.



**The content of the directories**:

- **audio extractor**: the code of Wav2vec audio encoder (from audio to features vector) and decoder (from features vector to written text)

- **video extractor**: the code of the CLIP model

- **seq2seq chollet**: the code of the seq2seq model







