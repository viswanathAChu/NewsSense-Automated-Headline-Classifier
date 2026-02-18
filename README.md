# HeadlineLens: Automated Large-Scale News Categorization

## 📌 Project Overview
HeadlineLens is an Unsupervised Machine Learning project designed to organize and categorize massive archives of unstructured text data. Utilizing a dataset of over **1.1 million news headlines** spanning 15 years, this project implements a robust NLP pipeline to discover latent topical patterns without the need for manual labeling.

## 🛠️ Technical Workflow
1. **Data Loading & Cleaning**: Handled a large-scale dataset (1.1M+ rows) using `Pandas`, ensuring data integrity and handling missing values.
2. **Text Preprocessing**: 
   - Tokenization and Lowercasing.
   - Removed stop words and punctuation to reduce noise.
   - Utilized **WordNetLemmatizer** to reduce words to their root forms, ensuring semantic consistency across the corpus.
3. **Feature Engineering**: 
   - Converted raw text into numerical vectors using **TF-IDF (Term Frequency-Inverse Document Frequency)**.
   - Optimized vocabulary size to manage memory efficiency while maintaining high-dimensional semantic relationships.
4. **Clustering Architecture**: 
   - Applied the **K-Means algorithm** to segment headlines into distinct topical groups.
   - Utilized the **Elbow Method** to determine the optimal number of clusters ($k$).
5. **Dimensionality Reduction & Visualization**: 
   - Implemented **PCA (Principal Component Analysis)** to project high-dimensional text vectors into 2D space for cluster interpretability and overlap analysis.

## 🧰 Tech Stack
- **Language:** Python
- **Libraries:** NumPy, Pandas, Scikit-Learn, NLTK
- **Visualization:** Matplotlib, Seaborn
- **Environment:** Jupyter Notebook / VS Code

## 📈 Key Results
- Successfully categorized a decade's worth of news into coherent topics (e.g., International Politics, Sports, Finance, and Local News).
- Proved the scalability of K-Means for large-scale text mining.
- Achieved clear cluster separation as validated through PCA visualization.

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/viswanathAchu/HeadlineLens.git](https://github.com/viswanathAchu/HeadlineLens.git)
