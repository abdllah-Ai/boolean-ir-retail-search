# Information Retrieval System with Boolean Search

This project implements a basic Information Retrieval (IR) system using Boolean search logic with stemming and tokenization on a retail dataset.

## 📁 Dataset

- File: `Online_Retail_UTF8.csv`
- Key Columns:
  - `Description`: Textual data to be indexed.
  - `InvoiceNo`: Used to identify documents.

## 🛠️ Features

- Tokenization using NLTK
- Porter Stemming
- Inverted Index creation
- Boolean search: supports AND, OR, NOT
- Precision and Recall calculation

## 🚀 How to Use

1. Place `Online_Retail_UTF8.csv` in the project directory.
2. Run the script:

```bash
python your_script_name.py
```

3. When prompted, enter a Boolean query such as:

```
shirt AND white
```

4. The system will:
   - Display matching document descriptions directly in the console.
   - Show which document IDs matched the query.
   - Compute and print:
     - **Precision**: how many retrieved documents were relevant.
     - **Recall**: how many relevant documents were successfully retrieved.

## 📦 Requirements

Install the required Python packages:

```bash
pip install -r requirements.txt
```

## 📊 Evaluation

The script uses a predefined list of `relevant_docs` for evaluating retrieval performance.

## 🖨️ Output

The output is printed in the terminal/console. It includes:
- List of matching document IDs and their descriptions
- Calculated **precision** and **recall** scores

To redirect the output to a file (optional), you can run the script like this:

```bash
python your_script_name.py > output.txt
```

This will save all printed results into a file named `output.txt`.
