# Online Female Mutual Support Communities: Themes and Engagement Mechanisms

**Author:** Yunfei Wang  
**Advisor:** Zhao Wang  
**Preceptor:** Henry Dambanemuya  
**Graduation Date:** May 2025

This repository contains the data and code supporting the thesis titled **"Online Female Mutual Support Communities: Themes and Engagement Mechanisms"**, which investigates engagement dynamics, prevalent themes, and factors driving interaction within the Douban "Women in Academia" online support community.

## Thesis Abstract

Online mutual support communities provide vital spaces for individuals to seek guidance, share experiences, and engage in collective discourse. Using a large-scale dataset collected from the Douban group "Women in Academia," this research identifies prevalent discussion topics and explores factors influencing user engagement using computational text analysis, sentiment analysis, and network-based modeling approaches. The study contributes to understanding online feminist discourse, digital engagement mechanisms, and network structures within female-oriented communities.

For detailed information and findings, please refer to the [complete thesis document](paper folder link).(Latex format see [Overleaf](https://www.overleaf.com/project/671ec5e1cd1d69d56b6e9f7e).)

## Repository Structure

### Data

- **`data/post_data.csv`**: Contains original posts from the Douban "Women in Academia" group, with attributes including post content, author details, publishing time, and engagement metrics (likes, comments, reposts, collections).
- **`data/reply_data.csv`**: Includes reply interactions within the community, capturing original posts, comments, author details, and timestamps.

### Codes

The folder `codes` contains Jupyter Notebooks (`.ipynb`) detailing each step of data processing, analysis, and modeling:

| Notebook                                    | Description                                                                                         |
|---------------------------------------------|-----------------------------------------------------------------------------------------------------|
| [00_data_wrangling.ipynb](https://github.com/yunfeiavawang/MA_Thesis_YunfeiWang/blob/main/codes/00_data_wrangling.ipynb) | Initial data preparation                                                  |
| [01-post_dataset_preprocessing.ipynb](https://github.com/yunfeiavawang/MA_Thesis_YunfeiWang/blob/main/codes/01-post_dataset_preprocessing.ipynb) | Preprocessing steps for original posts data, including tokenization and normalization              |
| [01-reply_dataset_preprocessing.ipynb](https://github.com/yunfeiavawang/MA_Thesis_YunfeiWang/blob/main/codes/01-reply_dataset_preprocessing.ipynb) | Preprocessing steps for reply data, constructing reply network edges                                |
| [02_descriptive_analysis.ipynb](https://github.com/yunfeiavawang/MA_Thesis_YunfeiWang/blob/main/codes/02_descriptive_analysis.ipynb) | Exploratory data analysis, distributions, correlations, and visualizations of engagement metrics    |
| [03-active_user_detection.ipynb](https://github.com/yunfeiavawang/MA_Thesis_YunfeiWang/blob/main/codes/03-active_user_detection.ipynb) | Detection and categorization of active users based on posting and replying frequency                |
| [04-topic_modeling.ipynb](https://github.com/yunfeiavawang/MA_Thesis_YunfeiWang/blob/main/codes/04-topic_modeling.ipynb) | Identification and interpretation of prevalent topics using Latent Dirichlet Allocation (LDA)       |
| [05-classification_with_LLM.ipynb](https://github.com/yunfeiavawang/MA_Thesis_YunfeiWang/blob/main/codes/05-classification_with_LLM.ipynb) | Classification of posts into support-seeking and support-provision categories using DeepSeek            |
| [06-sentiment_analysis.ipynb](https://github.com/yunfeiavawang/MA_Thesis_YunfeiWang/blob/main/codes/06-sentiment_analysis.ipynb) | Sentiment analysis on post contents using SnowNLP                                                   |
| [07-test_reliability.ipynb](https://github.com/yunfeiavawang/MA_Thesis_YunfeiWang/blob/main/codes/07-test_reliability.ipynb) | Reliability testing of computational labels with Cohen's Kappa            |
| [08-network_analysis.ipynb](https://github.com/yunfeiavawang/MA_Thesis_YunfeiWang/blob/main/codes/08-network_analysis.ipynb) | Network analysis of reply interactions, including calculation of centrality measures                |
| [09-Modeling.ipynb](https://github.com/yunfeiavawang/MA_Thesis_YunfeiWang/blob/main/codes/09-Modeling.ipynb) | Predictive modeling using XGBoost to identify factors influencing user engagement                   |

## Instructions for Replication

1. **Clone the repository:**

```bash
git clone git@github.com:yunfeiavawang/MA_Thesis_YunfeiWang.git
```

2. **Dependencies:**

Install the required Python packages:

```bash
pip install -r requirements.txt
```

3. **Execution:**

Run the Jupyter notebooks in the order listed in the table above to replicate the analysis step by step.

## Citation

Please cite this repository and the thesis appropriately if used in your work.

```bibtex
@misc{wang2025online,
    author = {Yunfei Wang},
    title = {Online Female Mutual Support Communities: Themes and Engagement Mechanisms},
    year = {2025},
    publisher = {GitHub},
    howpublished = {\url{git@github.com:yunfeiavawang/MA_Thesis_YunfeiWang.git}}
}
```

## Contact

For any questions or inquiries, please reach out at:

- **Email:** yunfeiavawang@uchicago.edu

---
