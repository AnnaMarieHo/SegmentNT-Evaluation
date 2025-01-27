# SegmentNT Evaluation
As an exploration of Machine Learning, I chose to run some analyses on the LLM SegmentNT. This personal exploration is a downstream study of my lab research at the University of Kentucky. It has served as a way to delve deeper into machine learning models as applied to clinical datasets, learn about large scale data analysis, and familiarize myself with huggingface models as well as the huggingface platform.

My testing framework: 

    a) prepare a data set for machine learning (cleaning, selection, manipulation)
    b) run the model on a given data set
    c) compare output across runs (and across data sets)

# STEPS TO RUN

Run each block of code in the, "RUNNING THE MODEL" section. The functions will read in test data of a reasonable size, and output results in a dedicated folder.

There is no code to run in the "PREPROCESSING SECTION". Likewise, the preprocessing steps are not executable in python. Instead, preprocessing steps are documented as markdown

The test datasets are meant to be read from the same directory as the as the Final Project notebook. Results will be output into the same directory as well

# NOTEBOOK SECTIONS
    a) Data Preparation
    b) Running the Model
    c) Results

# ABSTRACT
Nucleotide transformers have shown significant potential in functional genomic region prediction. SegmentNT (GitHub repository: https://github.com/instadeepai/nucleotide-transformer), a specialized model, predicts 14 classes of genetic elements, including protein-coding genes and splice sites. This study focuses on exon predictions across 3 samples to evaluate SegmentNT's numerical consistency across overlapping windows and its sensitivity to genomic context using 3 whole-genome sequences from a cohort of 808 ADNI participants, focusing on chromosome 21. Findings reveal high-confidence predictions with localized deviations influenced by genomic context. Future work will explore single-nucleotide prediction stability to enhance the model's generalizability.

# DATA PREPARATION
*The scripts utilized during data preparationare not executable in python notebooks. Additionally, the original datasets are too large to upload. Therefore, I have included samples of the datasets for running the model, and provided an outline of the steps taken to produce sample data like the ones provided*

##### Table of Contents 
* Data Preprocessing
   - Dataset Selection (selection)
   - Sequence Construction (manipulation)
   - Obtaining Phased Genome Information (manipulation)
   - Input Preparation (cleaning)
       - Capturing Context
       - Retrieving Sequences
* Full Scripts
   - getContext.py
   - getSequences.py

CITATIONS
The Beagle 5.4 genotype phasing method is described in:
B L Browning, X Tian, Y Zhou, and S R Browning (2021) Fast two-stage phasing of large-scale sequence data. Am J Hum Genet 108(10):1880-1890. doi:10.1016/j.ajhg.2021.08.005


