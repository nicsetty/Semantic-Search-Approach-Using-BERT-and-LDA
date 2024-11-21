# Semantic Search Using BERT and LDA (TF-IDF)

## Project Overview
This project demonstrates a semantic search approach applied to a dataset of books. It employs two methods:

1. **BERT-Based Semantic Search**:  
   - Uses pre-trained sentence embeddings to understand the contextual meaning of book titles and queries.  
2. **LDA-Based Semantic Search (TF-IDF)**:  
   - Utilizes TF-IDF vectorization and cosine similarity to calculate relevance scores.

The project improves information retrieval by using both contextual embeddings and statistical methods for comparison.

---

## Features

### Preprocessing:
- Text preprocessing using **spaCy** to remove stopwords and lemmatize book titles.

### BERT-Based Semantic Search:
- Encodes book titles and queries using a pre-trained **SentenceTransformer** model.
- Calculates cosine similarity between the query and dataset embeddings.

### TF-IDF (LDA-Based) Semantic Search:
- Vectorizes book titles using **TF-IDF**.
- Computes similarity scores using cosine similarity.

### Visualization:
- Displays similarity scores as a bar chart for both approaches.

---


## Tools Used
- **Python**: Programming language.
- **pandas**: Data manipulation and analysis.
- **scikit-learn**: For TF-IDF vectorization and cosine similarity calculations.
- **spaCy**: NLP for text preprocessing (lemmatization and stopword removal).
- **sentence-transformers**: For BERT-based sentence embeddings.
- **matplotlib**: Data visualization (bar charts).
- **tabulate**: Tabular data display.
  
---

## Example Results
-**Input Query** : "Science Fiction"
-**Output(TF-IDF)** :
+----------------------+--------------------+----------------+----------------+
|        Book          |      Author(s)    |     Genre      | tfidf_similarity |
+----------------------+--------------------+----------------+----------------+
| The Time Machine     | H.G. Wells        | Sci-Fi         |       0.87       |
| Dune                 | Frank Herbert     | Sci-Fi         |       0.81       |
+----------------------+--------------------+----------------+----------------+
-**Output(BERT)** :
+----------------------+--------------------+----------------+----------------+
|        Book          |      Author(s)    |     Genre      | bert_similarity |
+----------------------+--------------------+----------------+----------------+
| The Time Machine     | H.G. Wells        | Sci-Fi         |       0.92       |
| Dune                 | Frank Herbert     | Sci-Fi         |       0.88       |
+----------------------+--------------------+----------------+----------------+
---
## Visualization

### TF-IDF Similarities:
- Displays a bar chart of books ranked by their **TF-IDF similarity scores**.

### BERT Similarities:
- Shows a bar chart of books ranked by their **BERT similarity scores**.
---
### Future Enhancements:
-1.Explore combining BERT and TF-IDF scores for hybrid ranking.
-2.Extend the dataset with more book attributes for richer queries.
-3.Develop a web-based interface for easier interaction.

