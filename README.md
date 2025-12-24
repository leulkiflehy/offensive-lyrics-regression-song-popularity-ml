# Profanity in Hip-Hop Lyrics and Its Relationship to Spotify Popularity

This project analyzes whether profanity in hip-hop lyrics affects a song’s popularity on Spotify. Using a subset of a large lyrics dataset, the study focuses on profanity frequency, normalized profanity levels, and their statistical relationship with popularity scores.

---

## 1. Overview

The goal of this project is to determine whether higher profanity usage correlates with higher (or lower) popularity.  
The analysis:

- Focuses strictly on profanity, not hate speech  
- Uses recent hip-hop tracks (2020–2024)  
- Applies rule-based profanity detection and lyric preprocessing  

---

## 2. Dataset

**Source:** “900K+ Spotify Songs with Lyrics, Emotions & More” (Kaggle)  
**Sample:** 5,000 randomly selected hip-hop tracks  

Features used:

- song title  
- artist  
- lyrics  
- genre  
- Spotify popularity  

---

## 3. Methods

### Data Cleaning
- Removed missing lyrics/popularity  
- Lowercased text, removed tags like `[Verse]`  
- Tokenized lyrics  
- Removed punctuation, stopwords, and leftover contractions  

### Profanity Detection
- Loaded profanity list from `badwords_en.txt`  
- Counted profanity occurrences  
- Calculated normalized profanity (per 100 words)  

### Analysis
- Word frequency visualizations  
- Histogram of profanity counts  
- Popularity comparison between clean and profane songs  
- Correlation heatmap  
- Scatterplot: profanity vs. popularity  

---

## 4. Key Findings

- No meaningful correlation between profanity and Spotify popularity  
- Normalized profanity also showed no predictive value  
- The null hypothesis is supported: profanity does not impact popularity in this dataset  

Popularity appears more influenced by external factors such as artist reputation, playlisting, and marketing.

---

## 5. Limitations

- Spotify popularity is shaped by many hidden variables  
- Profanity detection is rule-based and not context-aware  
- The study is correlational, not causal  
- Sample limited to hip-hop and 5,000 tracks  

---

## 6. Tools Used

Python, Pandas, NumPy, NLTK, Matplotlib, Seaborn, WordCloud

---

## 7. Conclusion

Profanity in hip-hop lyrics does not appear to influence Spotify popularity.  
The results suggest that lyrical content alone is not a strong predictor of streaming performance, and future work could explore artist-level metadata or more advanced NLP models.

## Author

**Leul Kifle**  
George Mason University  
Computational Data Science


