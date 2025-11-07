# Love and Hate in Poetry — NLP Emotion Analysis (Project 11)

This repository contains the complete implementation and report files for **Project ID 11 – “Love and Hate in Poetry”**, developed as part of the **NLP Course at the University of Oulu**.

The project explores how contrasting emotions — *love* and *hate* — are expressed linguistically in poetry through lexical, semantic, and contextual analysis.  
Using Python (NLTK, WordNet, NRC EmoLex) and data from **Project Gutenberg**, the study quantifies emotional polarity and visualizes patterns through computational text analysis.

---

##  **Project Overview**

| Attribute | Details |
|------------|----------|
| **Course** | Natural Language Processing (University of Oulu) |
| **Project ID** | 11 |
| **Title** | *Love and Hate in Poetry* |
| **Authors** | Rao Ikram, Muhammad Ramish |


---

## **Pipeline Overview**

The project is structured around a 10-step NLP pipeline implemented in the Jupyter Notebook (`hate_and_love_poetry.ipynb`):

1. **Dataset Creation** – Load and label love/hate poetry from Project Gutenberg.  
2. **Text Preprocessing** – Tokenization, lowercasing, and stopword removal using NLTK.  
3. **Lexicon Construction** – Build emotion lexicons via NRC EmoLex + WordNet expansion.  
4. **Lexicon Statistics** – Compute word counts, overlaps, and lexical diversity.  
5. **Frequency & Proportion Analysis** – Normalize emotion counts across corpora.  
6. **Sequential Distance Analysis** – Measure token spacing between emotion terms.  
7. **Semantic Similarity (WordNet)** – Compute proximity between corpus tokens and emotion lexicons.  
8. **Per-Poem Similarity Profiling** – Calculate mean emotion similarity per poem.  
9. **Contextual Co-occurrence Analysis** – Extract and aggregate collocates within context windows.  
10. **Visualization & Interpretation** – Generate comparative histograms and word clouds.

---

##  **Core Methodology**

- **Lexicon-Based Emotion Detection:** Combines NRC EmoLex (Mohammad & Turney, 2013) with WordNet synsets for richer vocabulary coverage.  
- **Normalization Formula:**
  \[
  P_{emotion} = \frac{N_{emotion}}{N_{total}}
  \]
  Ensures comparability between poems of varying lengths.  
- **Context Windowing:** Uses a ±5 token window for co-occurrence extraction.  
- **Semantic Similarity:** WordNet path similarity used to detect implicit affective links.  
- **Visualization:** Word clouds, frequency plots, and statistical summaries created with Matplotlib and WordCloud.

---

##  **Results Summary**

- Love and hate poems show **distinct emotional vocabularies** with only 9 overlapping words.  
- Love poems use **denser affective adjectives** (e.g., *sweet, tenderly, dear*).  
- Hate poems emphasize **aggressive verbs and darker imagery** (e.g., *burn, break, blood, night*).  
- Average token distance between love words ≈ 45, between hate words ≈ 61.  
- Semantic similarity confirms **consistent emotional coherence** across both corpora.

---

##  **Technologies Used**

- **Python Libraries:** `nltk`, `pandas`, `numpy`, `matplotlib`, `wordcloud`
- **NLP Resources:** WordNet, NRC Emotion Lexicon
- **Development Tools:** Jupyter Notebook, GitHub, Overleaf (IEEE LaTeX)
- **Visualization Tools:** Matplotlib, WordCloud

--- 

