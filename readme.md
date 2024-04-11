# Algerian Names Dataset

This repository contains two datasets providing a rich collection of Algerian names and surnames:

* **Surnames:** A dataset of over 19,000 unique Algerian surnames in both Latin and Arabic script.
* **Names:** A dataset of over 12,000 unique Algerian names in both Latin and Arabic script. Name variations (e.g., Mohamed, Mohammed) are included.

These datasets offer a fantastic resource for anyone with an interest in Algerian names!

**Things to Keep in Mind:**

* **Designed for Learning:** These datasets are primarily for educational purposes. If you're exploring language analysis, researching Algerian names, or undertaking similar projects, you'll find these datasets useful. 
* **Let's Chat:** To ensure responsible use, please contact the repository maintainer (include your contact method) if you'd like to use the datasets. Briefly describe your project, and we'll get you set up!

**Data Format:**

Both datasets are in CSV format with the following columns:

* `latin_name` 
* `arabic_name` 

**Examples (Randomly Selected):**

```python
import pandas as pd
import random

# Surnames Dataset
df_surnames = pd.read_csv('sample_data/algerian_surnames.csv') 
random_surnames = df_surnames.sample(n=3) 

print("Surnames:")
for index, row in random_surnames.iterrows():
    print(f"- {row['latin_name']}") 

# Names Dataset
df_names = pd.read_csv('sample_data/algerian_names.csv')
random_names = df_names.sample(n=3)

print("\nNames:")
for index, row in random_names.iterrows():
    print(f"- {row['latin_name']}") 
