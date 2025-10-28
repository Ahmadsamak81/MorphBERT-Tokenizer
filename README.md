# MorphBERT

## Project Overview

**MorphBERT** is an Arabic morphology-aware tokenizer and model designed to enhance **Named Entity Recognition (NER)** performance by integrating **morphological segmentation** with **subword tokenization**.  
The notebook `MorphBERT_V2.ipynb` demonstrates:  
- Arabic morphological analysis and segmentation  
- Hybrid tokenization that preserves roots and affixes  
- Model training and NER evaluation using the **ANERCorp** dataset  

---

## How to Run on Google Colab

1. **Open the notebook in Google Colab**  
   Click to open [`MorphBERT_V2.ipynb`](./MorphBERT_V2.ipynb) in [Google Colab](https://colab.research.google.com/).

2. **Install dependencies**  
   The notebook installs all required libraries automatically.  
   If needed, run manually:
   ```python
   !pip install transformers torch datasets numpy pandas
   ```

3. **Run all cells**  
   Go to **Runtime → Run all** to execute the notebook:  
   - Loads the morphological analyzer  
   - Builds and trains the MorphBERT tokenizer/model  
   - Evaluates NER performance metrics (Precision, Recall, F1-Score)

4. **(Optional) Save results to Google Drive**  
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```

---

## Output Files

After running all cells, the following outputs are generated:

- **`/content/models/`** → saved tokenizer and model checkpoints  
- **`/content/results/`** → evaluation metrics and logs  
- **`/content/outputs/`** → exported charts, tokenization examples, and analysis tables  

If Google Drive is mounted, results are also saved under your Drive folder for permanent storage.
