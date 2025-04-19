The goal was to improve the effectiveness of machine translation and to facilitate easier communication across languages, ultimately reducing differences and promoting inclusiveness. This research paper will offer
valuable insight on how well various transformer-based models perform with low-resource languages and contribute to the creation of more reliable and accurate translation systems for
underrepresented languages.

**RESEARCH OBJECTIVES**

The purpose of this research paper is:
I. To evaluate the performance of three (3) transformer-based models (MT5, AfriMT5, and MarianMT) in enhancing machine translation for English to Akuapem Twi.
II. To compare the effectiveness of the base pre-trained MT5 model, the AfriMT5 model and Marian MT model in translating the English to Akuapem Twi corpus.
III. To investigate and analyze the relative efficacy and behaviour of each model in the specific task of English to Akuapem Twi machine translation, providing insights into their
strengths, weaknesses, and areas of improvement.

**MODEL PERFORMANCE**

![image](https://github.com/user-attachments/assets/74283bd3-2885-4eca-b090-cebdaf42a17e)


**MarianMT Model Performance**

MarianMT exhibited superior performance with significantly higher BLEU scores compared to the MT5 and AfriMT5 models. The MarianMT obtained a high level of translation quality on the
validation set with BLEU scores of 61.53. However, a significant decrease in the BLEU score to 11.72 on the test dataset indicated that the MarianMT is efficient in understanding the patterns in
the training data but faces difficulties in in generalizing to new unseen data. The difference points out the possibility of overfitting, the importance of applying an optimizer and a robust evaluation
methodology to ensure the model’s practical use in real-world situations.

**AfriMT5 Model Performance**

AfriMT5 model, tailored to African languages, demonstrated low performance with a validation
BLEU score of 4.46. However, the model’s BLEU score decreased to 1.82 on the test set, indicating
that the model faces significant challenges in translating most sentences accurately. The model’s
significant size presented memory management issues, which required extensive hyperparameter
adjustment and computing power, making it difficult to train the model and find proper parameters
that optimize the translation prediction.

**MT5 Model Performance**

The MT5 model performed the poorest among the three models, with BLEU scores close to zero
on both the validation and test sets. This indicated that the MT5, without prior fine-tuning specific
to Akuapem Twi language pair, is not sufficient for generating meaningful translations. The
illogical outputs showcased the model’s inability to comprehend and produce coherent translations
in the Akuapem Twi context, confirming the theory that specialized adaptation is essential for
successful machine translation in low-resource languages. The low BLEU score implied that the
model’s translation did not match the referencing language and that the translations contained
significant errors, incorrect words, poor grammar and problematic phrasing. The BLEU score
utilizes n-gram precisions to check how many of the n-grams in the model’s translations match the
those in the reference translations. The low score stipulates that there is a low overlap on the ngrams
between the source language and target/reference language.


**CONCLUSION**

The findings of this study emphasized the crucial need for tailored adaptation and fine-tuning for
of transformer-based models for low resource languages. In the instance of Akuapem Twi, African
low-resource language, it is morphologically rich and contains idiomatic expressions which might
pose as challenges for translation models. The superior performance of the MarianMT indicated
that the models specifically adapted to the language pair (English – Akuapem Twi) and trained on
appropriate datasets can significantly improve translation quality. Nevertheless, the observed
overfitting and variations in the performance highlight the need for regularization techniques,
enhanced evaluation methods, and the inclusion of more diverse and representative data. Future
studies should prioritize enhancing model robustness by implementing better regularization
techniques, leveraging more extensive and diverse datasets, and exploring advanced fine-tuning
techniques to enhance generalization capabilities. Additionally, deeper research on the specific
challenges of translating intricate sentence structures in low-resource languages will be essential
in improving machine translation systems.

In summary, developing more tailored models focused on low-resource languages will improve
the performance of machine translation models, which in turn will significantly contribute to
global development, promoting greater inclusivity, equity and understanding across cultural and
linguistic boundaries. This research paper lays a foundation for future enhancements and
emphasizes the continual requirement for tailored efficient models in the realm of translating lowresource
languages.
