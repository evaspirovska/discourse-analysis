# Dataset Creation Repository

This repository contains the code for creating datasets used in the project. The dataset creation process is documented and executed in the Jupyter notebook located in the `datasets_creation` folder.

## Repository Structure

- `datasets_creation/`
  - `eng_dep_covdtb_datasets_creation.ipynb`: Jupyter notebook containing the dataset creation code.

## Dataset Creation Process

The dataset creation process involves the following steps:

1. **Extract Abstract Documents**: Read and process a `.tok` file to extract document abstracts and save them to a CSV file.
2. **Extract EDUs**: For each document abstract, extract Elementary Discourse Units (EDUs) and save them to a separate CSV file.
3. **Extract Discourse Relations**: Process the texts to identify discourse relations and save the relations to another CSV file.

## Output Files

- `eng_dep_covdtb_texts_test.csv`: Contains document abstracts.
- `eng_dep_covdtb_edus_test.csv`: Contains extracted EDUs for each document.
- `eng.dep.covdtb_test_relations.csv`: Contains discourse relations between text units.

## Usage

Run the Jupyter notebook `eng_dep_covdtb_datasets_creation.ipynb` to generate the datasets. Ensure that all necessary input files are available in the specified paths.


# Notebooks

This folder contains Jupyter notebooks for various tasks related to relation classification and discourse unit classification using BERT and GPT models.

## Folder Structure

- `bert/`
  - `bert_for_relation_classification_all_classes.ipynb`: Notebook for relation classification using BERT, including all classes.
  - `bert_for_relation_classification_elaboration_excluded.ipynb`: Notebook for relation classification using BERT, excluding the elaboration class.
  - `bert_for_relation_classification_only_elaboration.ipynb`: Notebook for relation classification using BERT, focusing only on the elaboration class.

- `gpt/`
  - `discourse_relation_classification/`
    - `gpt4_for_discourse_relation_classification_all_classes.ipynb`: Notebook for relation classification using GPT-4, including all classes.
    - `gpt4_for_discourse_relation_classification_only_elaboration.ipynb`: Notebook for relation classification using GPT-4, focusing only on the elaboration class.
    - `gpt4_for_discourse_relation_classification_elaboration_excluded.ipynb`: Notebook for relation classification using GPT-4, excluding the elaboration class.
  - `elementary_discourse_units_classification/`
    - `gpt4_for_discourse_units_classification.ipynb`: Notebook for classifying elementary discourse units using GPT-4.
  - `results/`
    - `gpt4_eng_dep_covdtb_test_results.ipynb`: Notebook for analyzing the test results of the GPT-4 models on the eng_dep_covdtb dataset.

## Usage

Each notebook is designed to handle specific tasks related to relation classification and discourse unit classification. To use the notebooks:

1. Open the notebook in the respective subfolder.
2. Follow the instructions and code cells to preprocess data, train the models, and evaluate the results.
3. Ensure all necessary input files and dependencies are available and properly configured.

## Notes

- The BERT notebooks focus on relation classification tasks with different configurations (all classes, elaboration excluded, and only elaboration).
- The GPT notebooks cover both relation classification and elementary discourse unit classification, with additional notebooks for analyzing test results.
- The same approach is used to generate and evaluate results for other GPT models, such as GPT-3.5 and GPT-4 Mini and is also used to generate results for the SciDTB dataset, based on the prompt messages defined in the appendix.
