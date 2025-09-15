# Spam vs Ham Classification

This project applies **Logistic Regression** to classify emails as **spam** or **ham** (not spam).  
It explores different text representations and decision strategies to balance **precision** and **recall**.

---

## Project Highlights
- Preprocessed text data for email classification.  
- Compared two feature extraction methods:  
  - **CountVectorizer + Logistic Regression**  
  - **TF-IDF Vectorizer + Logistic Regression**  
- Evaluated models using **cross-validation** and multiple metrics.  
- Tuned the **decision threshold** to improve recall while keeping precision high.  
- Visualized trade-offs with a **Precision-Recall curve**.  
- Summarized results in a clean comparison table.  

---

## Results

| Model                  | Precision | Recall | F1 Score |
|-------------------------|-----------|--------|----------|
| CountVectorizer + LR    | 0.9798    | 0.8564 | 0.9140   |
| TF-IDF + LR             | 0.9964    | 0.6927 | 0.8172   |
| TF-IDF + LR (Threshold) | 0.9684    | 0.8846 | 0.9246   |

- **CountVectorizer + LR** gives a good balance.  
- **TF-IDF + LR** maximizes precision but sacrifices recall.  
- **TF-IDF + LR (Threshold tuned)** achieves the **best F1-score** by improving recall without losing much precision.  

---

## Tech Stack
- Python  
- pandas, numpy  
- scikit-learn  
- matplotlib  

---

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/spam-ham-classification.git
   cd spam-ham-classification
