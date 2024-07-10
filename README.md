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
