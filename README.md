# 🔍 Offensive Language Classification

A multi-label classification project to detect various forms of offensive content in user feedback using Machine Learning, Deep Learning, and Transformer-based models.

---

## 📚 Dataset

- **Train:** English feedback texts with 6 binary labels:  
  `toxic`, `abusive`, `vulgar`, `menace`, `offense`, `bigotry`
- **Validation and Test:** Multilingual texts  
  Only the `toxic` label is available for evaluation.

---

## ⚙️ Approaches & Models

### ✅ Machine Learning
- Models: Logistic Regression (LR), Random Forest (RF)
- Features: TF-IDF, multilingual sentence embeddings
- Tuning: Grid Search & Random Search

### 🤖 Deep Learning
- Models: LSTM, GRU
- Tokenized and padded sequences with Embedding layers

### 🧠 Transformer Models
- Models: BERT, XLM-RoBERTa
- Fine-tuned with dropout + dense layers

---

## 📈 Results Summary

| Model          | Accuracy | F1-Score |
|----------------|----------|----------|
| LR / RF        | ✅ High  | ⚠️ Moderate |
| LSTM / GRU     | ✅ High  | ✅ Better   |
| BERT / XLM-R   | ✅ High  | 🏆 Best     |

---

## 🛠️ Steps to Run the Code

1. **Clone the Repository:**  
   ```bash
   git clone https://github.com/Sajid064/Offensive-Language-Classification.git
   cd Offensive-Language-Classification

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt

3. **Run the notebooks:**
   - Execute cells in task/model1_implementation.ipynb
   - Execute cells in task/model2_implementation.ipynb
  
---

## ⚠️ Key Challenges and Observations

- **Class Imbalance:** High accuracy but relatively lower F1-score
- **Train-Test Mismatch:** Language difference affected performance
- **Label Availability:** Only `toxic` label provided for test set
