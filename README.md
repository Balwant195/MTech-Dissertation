# Sentiment Analysis on Code-Mix Text using XLM-RoBERTa

This repository explores sentiment analysis for code-mixed Hindi-English text (Hinglish) using deep learning techniques. We leverage the XLM-RoBERTa model, a pre-trained cross-lingual transformer, and evaluate several training approaches to handle code-mix text data challenges.

## Overview

Sentiment analysis of code-mixed languages, where Hindi and English are blended, poses unique challenges. This study tests various approaches to improve sentiment analysis performance using the XLM-RoBERTa model. Four distinct training approaches with different dataset combinations were evaluated to determine their effectiveness.

## Approaches Tested

1. **Approach 1**: Trained exclusively on the Hinglish dataset.
2. **Approach 2**: Augmented Hinglish dataset with Spanish-English data.
3. **Approach 3**: Used only mixed datasets without Hinglish data.
4. **Approach 4**: Combined Hinglish and Marathi-English data, excluding Spanish-English data.

## Results

- **Approach 1**: Achieved 61% accuracy.
- **Approach 2**: Also achieved 61% accuracy, similar to Approach 1. This similarity suggests that both datasets contained samples similar to those in the test set.
- **Approach 3**: Resulted in lower performance with 49% accuracy, indicating that the model struggled with the unfamiliar mixed dataset.
- **Approach 4**: Showed the best performance with 62% accuracy. This approach effectively used combined datasets of languages with similar linguistic characteristics (Hindi and Marathi), demonstrating improved performance.

### Key Insights

- Combining datasets of languages with similar linguistic traits (e.g., Hindi and Marathi) led to the best performance, highlighting the model's better understanding of code-mixed languages with shared grammatical structures.
- Augmenting training data with diverse mixed languages (e.g., Spanish-English) did not improve performance, emphasizing that different grammatical structures can hinder model learning.
- Results confirm that the model's performance improves when trained on datasets that share linguistic similarities with the test data, suggesting a focused approach in data augmentation for better outcomes.

## Files and Directories

- `report/`: Contains a detailed report.
- `data/`: Includes datasets used in the study (Hinglish, Spanish-English, Marathi-English).
- `scripts/`: Code for training models and generating performance metrics.

## References

- [XLM-RoBERTa: A Pre-trained Cross-Lingual Model](https://arxiv.org/abs/1911.02116)
- Additional relevant papers and resources are listed in the detailed report.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
