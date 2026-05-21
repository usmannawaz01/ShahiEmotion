# ShahiEmotion: A Benchmark Dataset for Punjabi Shahmukhi Emotion Detection

ShahiEmotion is a sentence-level Punjabi Shahmukhi emotion detection dataset. It contains 30,379 annotated instances across seven emotion categories: sadness, surprise, happiness, anger, neutral, fear, and disgust.

The dataset is designed to support research on Punjabi Shahmukhi emotion analysis, low-resource NLP, and multilingual affective computing.

## Dataset Description

Punjabi written in the Shahmukhi script is an under-resourced language variety for emotion detection. ShahiEmotion provides a benchmark-style dataset with fixed train, development, and test splits for supervised emotion classification.

Each instance contains:

- a Punjabi Shahmukhi sentence
- one emotion label

The task is formulated as a seven-class sentence-level classification problem.

## Emotion Labels

The dataset contains the following emotion categories:

| English Label | Description |
|---|---|
| Sadness | Sentences expressing sadness or sorrow |
| Surprise | Sentences expressing surprise |
| Happiness | Sentences expressing happiness or positive emotion |
| Anger | Sentences expressing anger |
| Neutral | Sentences with no clear emotion |
| Fear | Sentences expressing fear |
| Disgust | Sentences expressing disgust |

## Dataset Statistics

| Split | Number of Sentences |
|---|---:|
| Train | 24,303 |
| Development | 3,038 |
| Test | 3,038 |
| Total | 30,379 |

## Label Distribution

| Label | Count |
|---|---:|
| Neutral | 17,459 |
| Happiness | 6,687 |
| Disgust | 2,516 |
| Sadness | 1,355 |
| Fear | 1,008 |
| Anger | 826 |
| Surprise | 528 |
| Total | 30,379 |

## Baseline Results

The paper evaluates several pretrained transformer models under the same fine-tuning setup. XLM-RoBERTa base achieves the best overall performance.

| Model | Accuracy | Macro-F1 | Weighted-F1 |
|---|---:|---:|---:|
| mBERT cased | 77.72 | 54.14 | 76.90 |
| mBERT uncased | 77.42 | 54.71 | 76.74 |
| DistilBERT multilingual | 76.07 | 52.02 | 75.31 |
| XLM-RoBERTa base | 77.95 | 58.47 | 77.60 |
| Urdu RoBERTa small | 77.45 | 56.32 | 76.84 |

## Recommended Use

This dataset is intended for:

- Punjabi Shahmukhi emotion detection
- low-resource text classification
- multilingual NLP research
- affective computing
- benchmark evaluation of transformer models

The dataset and models should not be used for high-stakes decision-making.

## Dataset Source and Attribution

ShahiEmotion is derived from the English–Punjabi (Shahmukhi) Parallel Sentences Corpus (Mediamen Archives), distributed through the Mozilla Data Collective under the CC BY-NC 4.0 license.

We use the Punjabi Shahmukhi sentences from the original corpus and add sentence-level emotion annotations for seven emotion categories.

## License

ShahiEmotion is released under the Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0).

The underlying source sentences remain subject to the original CC BY-NC 4.0 license. The added emotion annotations are also released under CC BY-NC 4.0.

This dataset may be used, shared, and adapted for research and other non-commercial purposes only, with appropriate attribution. Commercial use is not permitted without explicit permission from the relevant rights holders.

For full license details, see the `LICENSE` file.

## Citation

If you use this dataset, please cite the ShahiEmotion paper.

```bibtex
@misc{shahiemotion2026,
  title = {ShahiEmotion: A Benchmark Dataset for Punjabi Shahmukhi Emotion Detection},
  author = {Anonymous},
  year = {2026},
  note = {Punjabi Shahmukhi emotion detection dataset}
}
