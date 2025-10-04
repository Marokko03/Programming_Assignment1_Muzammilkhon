# Programming_Assignment1_Muzammilkhon


**Explained variance: PC1 ≈ 55.41%, PC2 ≈ 12.72% (total ≈ 68.13%); visually separable classes: 0.**

## Datasets

* **Images:** Kaggle — *Solar Panel Images*
  Classes used: **Bird-drop**, **Snow-Covered**, **Dusty**, **Clean**
  Link: [https://www.kaggle.com/datasets/pythonafroz/solar-panel-images](https://www.kaggle.com/datasets/pythonafroz/solar-panel-images)
* **Tweets (training set only):** instructor-provided JSON/JSONL.
  In the notebook (section B-1) an adapter converts the dataset to two columns: `text`, `label`.

## What the notebook does

**Part A (Images):**

* Convert to grayscale → Sobel `dx/dy` → angle map.
* Edge-orientation histogram (36 bins) for one image per class.
* Compare two histograms using Euclidean, Manhattan, and Cosine distances.
* HOG descriptor + visualisation for one image.
* PCA 36→2 on **all** images; 2D scatter colored by the four classes + explicit answer to “how many classes are visually separable”.

**Part B (Tweets):**

* `CountVectorizer()` and `TfidfVectorizer()` with **default parameters**.
* Print dimensionality of both representations `(N, D)`.
* Choose 4 classes, run PCA→2D for Count and for TF-IDF (two separate plots).
* Short note on which classes (if any) are visually separable on **both** plots.
**Explained variance: PC1 ≈ 55.41%, PC2 ≈ 12.72% (total ≈ 68.13%); visually separable classes: 0.**
