# Sentiment Analysis on Amazon Product Reviews

## Overview

This project utilizes the Cardiff NLP Twitter RoBERTa-based sentiment analysis model to analyze sentiment in a subset of Amazon product reviews. The code processes the dataset, tokenizes text, and computes sentiment scores for each review.

## Installation

### Prerequisites

- [Google Colab](https://colab.research.google.com/): The project is designed to run in a Google Colab environment for seamless execution.

### Setup

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/your-username/sentiment-analysis.git
    cd sentiment-analysis
    ```

2. **Mount Google Drive:**

   Open the Jupyter Notebook in Google Colab and mount your Google Drive to access necessary files.

3. **Install Required Libraries:**

    ```bash
    !pip install pandas numpy matplotlib seaborn tqdm transformers
    ```

4. **Setup Kaggle API:**

   - Place your Kaggle API key in the `kaggle.json` file and copy it to the `~/.kaggle/` directory.
   
    ```bash
    ! mkdir ~/.kaggle
    !cp /content/drive/MyDrive/kaggle.json ~/.kaggle/kaggle.json
    ! chmod 600 ~/.kaggle/kaggle.json
    ```

5. **Download and Extract Dataset:**

    ```bash
    !kaggle datasets download -d arhamrumi/amazon-product-reviews
    !unzip amazon-product-reviews.zip
    ```

## Usage

1. **Open the Jupyter Notebook (`sentiment_analysis.ipynb`).**
2. **Execute the Cells Sequentially.**
3. **Explore Sentiment Analysis Results and Dataset Insights.**

## Model

- **Architecture:** Cardiff NLP Twitter RoBERTa-based sentiment analysis model
- **Model URL:** [cardiffnlp/twitter-roberta-base-sentiment](https://huggingface.co/cardiffnlp/twitter-roberta-base-sentiment)
- **Tokenizer:** [transformers.AutoTokenizer](https://huggingface.co/transformers/main_classes/configuration.html#transformers.AutoTokenizer)
- **Model Class:** [transformers.AutoModelForSequenceClassification](https://huggingface.co/transformers/main_classes/model.html#transformers.AutoModelForSequenceClassification)

## Results

Sentiment scores for each review are computed and stored in the `results_df` DataFrame. The notebook provides visualizations and examples to comprehend the sentiment distribution in the dataset.

## Contributing

We welcome contributions to enhance and expand this project. Feel free to fork the repository, make improvements, and submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
