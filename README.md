# AI systems that generate deceptive explanations can amplify beliefs in false information
A repository for the paper "AI systems that generate deceptive explanations can amplify beliefs in false information," TBD. 

Author: Valdemar Danry<sup>1</sup>, Pat Pataranutaporn<sup>1</sup>, Matthew Groh<sup>2</sup>, Ziv Epstein<sup>1</sup>, Pattie Maes<sup>1</sup>

<sup>1</sup> MIT Media Lab, Massachusetts Institute of Technology, Cambridge, Massachusetts, United States   
<sup>2</sup> Northwestern University, Evanston, IL, United States     
\* e-mail: vdanry[at]mit.edu

## Abstract
Artificial Intelligence systems, such as large language models (LLMs), have the remarkable capability to not only generate responses on various topics but also can provide supportive explanations for their responses, thereby bolstering their credibility. However, there is also potential for these systems to generate plausible yet deceptive explanations such as false political commentary and manipulative decision support, which could mislead individuals for malicious purposes. We investigate the impact of AI-generated deceptive explanations on people and the personal factors that mediate their effects in a pre-registered experiment with 23,840 observations from 1192 participants. We demonstrate that with a single prompt, a large language model can easily be used to generate deceptive explanations of information that the public may encounter. Our study reveals that AI-generated deceptive explanations significantly increase belief in false headlines and decrease belief in true headlines. Compared to deceptive classifications without explanations, AI-generated deceptive explanations can be more persuasive in convincing people. We also investigated the personal factors that moderate the influence of AI-generated deceptive explanations such as measures of cognitive reflection, trust in AI, and prior knowledge. These findings indicate that the proliferation of advanced AI systems could potentially reshape the misinformation landscape, underlining the necessity of further study on mitigating these effects.

### For more information: https://www.media.mit.edu/projects/beliefs-about-ai/overview/

## Analysis
This repository contains the analysis for the paper titled "AI Systems That Generate Deceptive Explanations Can Amplify Beliefs in False Information". 

The **Analysis** folder contains the following notebooks:

- `stimuli_generation_news.ipynb`: This notebook generates the news headlines stimulus set with AI explanations (Deceptive/Honest) based on the LIAR-PLUS dataset available at [https://github.com/Tariq60/LIAR-PLUS](https://github.com/Tariq60/LIAR-PLUS).
- `stimuli_generation_trivia.ipynb`: This notebook generates the trivia stimulus set with AI explanations (Deceptive/Honest) based on the article available at [https://www.cosmopolitan.com/uk/worklife/a32612392/best-true-false-quiz-questions/](https://www.cosmopolitan.com/uk/worklife/a32612392/best-true-false-quiz-questions/).
- `results_preprocessing_trivia+news.ipynb`: This notebook converts the raw participant ratings (`raw_results.csv`) and stimuli meta data (`metadata.csv`) to a processed file for further analysis (`results_processed.csv`).
- `results_analysis_and_plotting.ipynb`: This notebook computes all the analysis reported in the paper and supplementary information.

## Results

The **Results** folder contains the following files:

- `results_raw.csv`: Participant ratings from Qualtrics.
- `metadata.csv`: Ground truth of the stimuli.
- `demographics_raw.csv`: Raw demographics data from Prolific.
- `results_processed.csv`: Processed experimental results.

## Stimuli

The **Stimuli** folder contains the following files:

- `items_news_raw.csv`: News headlines items without AI explanations.
- `items_trivia_raw.csv`: Trivia items without AI explanations.
- `stimuli_news_raw.csv`: News headlines items with AI explanations.
- `stimuli_trivia_raw.csv`: Trivia items with AI explanations.
- `stimuli_trivia+news_processed.csv`: Combined processed news headlines and trivia items with AI explanations.

Please refer to the methodology section of the paper "AI Systems That Generate Deceptive Explanations Can Amplify Beliefs in False Information" for more details on the experiment.
