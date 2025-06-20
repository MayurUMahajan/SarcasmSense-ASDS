# SarcasmSense-ASDS
# Sarcasm and Sentiment Detection in Political News

This project uses two BERT-based models to perform:
- **Sarcasm Detection**: Classifies text as sarcastic or non-sarcastic.
- **Sentiment Classification**: Categorizes text into one of five sentiments:
  - Very Negative
  - Negative
  - Neutral
  - Positive
  - Very Positive

---

## Files Included

- `model_1-5.py`: Python script containing full pipeline (preprocessing, training, and prediction)
- `KaggleDataset_with_sarcasm.csv`: Dataset file (must be present in the same directory)
- `requirements.txt`: Required Python packages
- `README.md`: Project overview and instructions

---

## Setup

Install all dependencies using:

```bash
pip install -r requirements.txt
```

---

## How to Use

1. Make sure `KaggleDataset_with_sarcasm.csv` is in the same folder as `model_1-5.py`.
2. Run the script:

```bash
python model_1-5.py
```

3. Enter a political news text when prompted.
4. The model will output whether it's sarcastic and its sentiment category.

---

## Dataset Format

The dataset (`KaggleDataset_with_sarcasm.csv`) should contain the following columns:

- `text`: The raw political news statement
- `sarcasm`: Sarcasm label (e.g., sarcastic / not sarcastic)
- `sentiment`: One of the five sentiment classes

---

## Model Details

- **Tokenizer**: `bert-base-uncased` from HuggingFace
- **Architecture**: `BertForSequenceClassification`
- Two separate models trained for sarcasm and sentiment tasks using PyTorch.

---

## License

This project is under the MIT License.
