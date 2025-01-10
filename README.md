# MedCompare

The main research question of this project is: How can we use large language models (LLMs)
and retrieval-based techniques to create reliable and user-friendly summaries in real time that
compare medications with similar use cases, focusing on their uses and side effects?

The primary focus of our project is to create a retrieval-based system that identifies and retrieves
real-time information about medications with similar uses and extracts and summarizes details
about the side effects, providing users with a side-by-side comparison.

Comparing the baseline:
We want to compare Bio+ClinicalBERT-based results to the TF-IDF ones to benchmark
the performance of Bio+ClinicalBERT. Also we want to conduct a detailed error analysis
to identify cases where Bio+ClinicalBERT performs significantly better than TF-IDF.
This will help clarify where the additional complexity of using a transformer model is most
beneficial, such as cases involving complex symptom descriptions or nuanced ingredient
interactions.

To realise this task we had to choose a suitable Dataset. It should contain detailed information about various medicines,
including their composition, uses and side effects. We decided to use "Medicine_Details" by MattBaster from HuggingFace
because it suited our dependencies. For our work we focused on the collumns "Medicine Name", "Composition", "Uses", and "Side_effects".
For further information about the dataset visit HuggingFace: https://huggingface.co/datasets/MattBastar/Medicine_Details
