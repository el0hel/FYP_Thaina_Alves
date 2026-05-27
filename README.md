# AI Approaches to Detecting Language Variation in Opinions Between Brazilian and European Portuguese

This repository contains the source code and datasets created in support of the thesis **"AI Approaches to Detecting Language Variation in Opinions Between Brazilian and European Portuguese"**, submitted as the final assessment for the Bachelor of Science in Information Technology (Honours) (Artificial Intelligence) at the University of Malta.

---

## Repository Structure

### `code.ipynb`
This notebook contains the complete end-to-end pipeline for the project:
* **Data Extraction:** Scraping iFood and Glovo reviews using the `google-play-scraper` library.
* **Data Cleaning:** Pre-processing steps required for dataset construction.
* **Model Training:** Training, validating, and evaluating the performance of 6 classification models across 9 distinct dataset configurations.
* **Dialect Classification:** Utilising the `fasttext-euptvid` dialect classifier for qualitative error analysis.

### `dataset_all_versions/`
Contains the datasets at various stages of the pipeline to ensure reproducibility:
* `initial_data`: The raw scraped app reviews prior to any pre-processing.
* `emoji_number_preprocessing`: Reviews after filtering out emoji-only or number-only entries.
* `non_pt_preprocessing`: Reviews after filtering out non-Portuguese text.
* `demojize_preprocessing`: Reviews with emoji characters converted to textual tokens.
* `punctuation_preprocessing`: Reviews with repetitive punctuation converted to textual tokens.
* `*_sampling`: BP (Brazilian Portuguese), EP (European Portuguese), and MIX reviews separated after random sampling for a class-balanced dataset.
* `final_ds`: The 3 distinct final corpora after the removal of singleton words.

---

## Contact & Model Weights

If you require the trained weights for the Deep Learning models or have any questions regarding the research, please feel free to reach out via email at [alvesthainahelena@gmail.com](mailto:alvesthainahelena@gmail.com).
