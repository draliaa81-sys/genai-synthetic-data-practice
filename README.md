# Generative AI for Synthetic Data (Practice Notebook)

A Google Colab notebook where I practised four ways to create synthetic data in Python, as part of my Data Analytics and Generative AI study.

[Open the notebook in Colab](https://colab.research.google.com/github/draliaa81-sys/genai-synthetic-data-practice/blob/main/genai_synthetic_data_practice.ipynb)

## What is in the notebook

1. **Fake customer records with Faker.** Creates New Zealand style customers (name, email, age, region, account type, loan) and charts the age spread and the customers per region.
2. **New rows with CTGAN.** Builds a small seed table of 200 customers, lets SDV detect the column types, trains a CTGAN model on it, and generates new rows that follow the same patterns.
3. **Normal and unusual transactions.** Generates everyday transactions and a smaller set of suspicious ones (possible fraud), plots amount against time gap, and saves the result to CSV.
4. **Synthetic text with GPT-2.** Uses the Hugging Face `transformers` library to complete short business prompts, then looks at summary statistics of the generated text.

## Tools

Python, pandas, NumPy, Matplotlib, Faker, SDV (CTGAN), Hugging Face Transformers (GPT-2), Google Colab

## How to run it

Open the notebook in Colab with the link above and run the cells from top to bottom. The install cells add Faker, SDV and Transformers. The first GPT-2 run downloads about 500 MB, so it takes a minute or two.

All data in this notebook is made up. No real customer data is used.

## Related project

I used CTGAN again in a course project on a real public dataset, where synthetic records raised recall for a rare class from 0.375 to 0.946. Details are on my [LinkedIn](https://www.linkedin.com/in/aliaafarag/).

## Author

Aliaa Farag
