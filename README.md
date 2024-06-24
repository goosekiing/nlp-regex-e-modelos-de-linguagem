# NLP: Regex and Language Models

This repository contains a project focused on Natural Language Processing (NLP) using regex and language models. The project utilizes datasets with programming-related questions asked by users on forums. These datasets include questions in English, Portuguese, and Spanish. The goal of the project is to create models trained with these datasets to develop a system capable of recognizing the language of a given text.

## Project Overview

### Initial Approach
- **Data Preprocessing:**
  - Handling code snippets using regex
  - Unifying and tokenizing the texts
- **Models:**
  - Trained three Maximum Likelihood Estimator (MLE) models, one for each language
  - Used these models to calculate the perplexity of a given text (lower perplexity indicates a closer match to the tested model)
  - Identified a limitation: MLE can assign zero probability to unseen events in the training data
- **Improved Approach:**
  - Implemented Laplace smoothing to address the zero probability issue

### Final Classifier
- **Functionality:** 
  - Classifies text based on perplexity scores
  - Achieved high accuracy rates for the test data:
    - Portuguese: 100%
    - English: 100%
    - Spanish: 97%

## Course Details
This project was completed as part of the 'Advanced Machine Learning' course on Alura. For more information about the course, visit [Alura](https://cursos.alura.com.br/formacao-machine-learning-avancada).

## Objectives Achieved
- Advance studies in Natural Language Processing (NLP).
- Learn how regex can assist in processing textual data.
- Understand language models and their applications.
- Create a model that automatically detects languages.
- Practice using Python libraries such as NLTK and Scikit-Learn.

## Technologies Used
- Python (v3.11.4)
- Jupyter Notebook
- NLTK
- Scikit-learn
- Pandas
- NumPy

## Project Structure
The directory structure of the project is as follows:
```
nlp-regex-e-modelos-de-linguagem/
│ database-english-project-06.csv
│ database-portuguese-project-06.csv
│ database-spanish-project-06.csv
│ project-06.ipynb
│ README.md
```

## Setup Instructions
1. Clone the repository:
   ```sh
   git clone https://github.com/goosekiing/nlp-regex-e-modelos-de-linguagem.git
   ```
2. Navigate to the project directory:
   ```sh
   cd nlp-regex-e-modelos-de-linguagem
   ```
3. Create a virtual environment and activate it:
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```
4. Install the required libraries:
   ```sh
   pip install numpy pandas scikit-learn nltk
   ```
5. Download additional NLTK data (if not already done):
   ```python
   import nltk
   nltk.download('all')  # Uncomment and run this in the notebook if needed
   ```

## Running the Notebook
1. Open Jupyter Notebook:
   ```sh
   jupyter notebook
   ```
2. Run the `project-06.ipynb` notebook to see the analysis and language classification in action.

## Language
The language used in this project is Brazilian Portuguese (pt-br).

## Author
GitHub Username: [goosekiing](https://github.com/goosekiing)
