# HebrewLanguageDetoxification
Hebrew Language Detoxification

CoT prompting was used for detoxification, demonstrating that breaking down the detoxification process.
In our work, we adapted the A1 and A3 prompts from the paper

Dementieva, D., Babakov, N., Ronen, A., Ayele, A.A., Rizwan, N., Schneider, F., Wang, X., Yimam, S.M., Moskovskiy, D., Stakovskii, E. and Kaufman, E., 2024. Multilingual and explainable text detoxification with parallel corpora. arXiv preprint arXiv:2412.11691.

for the detoxification of Hebrew-language texts  with the GPT-4o model. These prompts appear in this repository as well.

We extended these prompts by adding more detailed instructions and multiple in-language examples adapted to Hebrew. Specifically, we designed a custom prompt that instructed the model to analyze provided Hebrew sentences for elements of toxicity using a predefined list of keywords and to output detoxified sentences in a structured format. The prompt emphasizes preserving the original meaning, tone, and intent while removing toxic or offensive expressions without introducing unsolicited advice or commentary. We also added two negative examples in Hebrew where the modified sentences contain advice or interpretation not present in the original text. The full prompt is provided in this repository as a pdf image.

The final dataset contains 600 texts in their original form (offensive), LLM-detoxified (after applying the prompt), and after human correction. To train detoxification models, please use the original-human corrected pairs and cite our paper (to appear at RANLP).

