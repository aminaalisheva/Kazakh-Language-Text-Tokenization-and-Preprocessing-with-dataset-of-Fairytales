# NLP: Text Processing

**Date:** February 5, 2025  
**Contributers:**  
- Amina Alisheva  
- Jafar Isbarov  
- Ariana Kenbayeva  

---

## Overview
This project focuses on implementing fundamental text processing techniques in **Natural Language Processing (NLP)** using **Kazakh-language** datasets. The tasks include **tokenization, byte pair encoding (BPE), sentence segmentation, and spelling correction using Levenshtein distance**. The dataset consists of fairy tales collected from online sources, and additional processing was applied using **regular expressions and NLP algorithms**.

## Datasets
- **Self-Created Dataset:** Scraped from **ertegiler.kz** and **balalaralemi.kz** using BeautifulSoup.
- **Open-Source Dataset:** A larger dataset on **Kazakh literature** from **Hugging Face**.
- Both datasets were cleaned and stored as CSV files with metadata.

## Key Features & Methods Implemented
1. **Tokenization:**
   - Standard tokenization applied using **regular expressions**.
   - Reduced redundant suffixes (e.g., "айт-айт" to "айт").
   
2. **Byte Pair Encoding (BPE):**
   - Used for handling out-of-vocabulary (OOV) words.
   - Demonstrated improved vocabulary representation with 1000+ merges.

3. **Heaps' Law Analysis:**
   - Applied to both datasets.
   - **Beta values:** 0.67 - 0.75 for larger datasets.

4. **Sentence Segmentation:**
   - Implemented a segmentation algorithm to handle **missing spaces and punctuation inconsistencies**.

5. **Spelling Correction:**
   - **Levenshtein Distance:** Used to correct misspelled words.
   - **Weighted Edit Distance:** Lowered weights for frequently confused letter pairs.
   - **Confusion Matrix:** Evaluated spelling checker accuracy.

## Challenges & Limitations
- **Dictionary-based spelling correction:** Some **grammatically correct words out of context** may be incorrectly flagged.
- **Out-of-Vocabulary Words:** Not all words were in the self-created dictionary, leading to false negatives.
- **Byte Pair Encoding:** Lacks predefined categories and thresholds for optimal tokenization.

## Contributions
- **Amina Alisheva:** Tokenization, Byte Pair Encoding, Spelling Checker, Weighted Edit Distance, Confusion Matrix.
- **Ariana Kenbayeva:** Heaps' Law Analysis, Sentence Segmentation.
- **Jafar Isbarov:** Dataset collection, data cleaning, review of all code.
- **Report Writing:**
  - **Amina:** Contributions Section.
  - **Ariana:** Introduction, Dataset, Discussion.
  - **Jafar:** Conclusion.

## Results
- Standard **tokenization and BPE** performed well.
- Sentence segmentation correctly identified sentence boundaries.
- The **spelling checker system** using Levenshtein Distance showed promising results.
- Weighted Levenshtein Distance improved accuracy.

## Future Improvements
- Implement **named entity recognition (NER)** and **sentiment analysis**.
- Expand dataset categories.
- Define thresholds for **BPE tokenization**.

## References
- **https://ertegiler.kz/** (retrieved on February 2, 2025)
- **https://balalaralemi.kz/** (retrieved on February 4, 2025)

