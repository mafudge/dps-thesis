# Michael Fudge's DPS Thesis Repository

    Michael Fudge
    Doctor of Professional Studies (DPS) Candidate
    The School of Information Studies at Syracuse University
    Spring 2026
    Email: mafudge@syr.edu
    ORCID: 0009-0006-2760-9360


This repository contains the code and resources for my Doctor of Professional Studies (DPS) thesis. 

My thesis investigates the impact of Large Language Models (LLMs) use on learning and computational literacy of participants enrolled in a introduction to programming course.

## Contents

Click to view these contents.

- `thesis/`: Contains the thesis documents in a variety of formats.
   - [Draft-Thesis.md](./thesis2/Draft-Thesis.md): The thesis document in Markdown format.
   - [Draft-Thesis.pdf](./thesis2/Draft-Thesis.pdf): The thesis document in PDF format.
   - [Draft-Thesis.docx](./thesis2/Draft-Thesis.docx): The thesis document in MS Word format.

- `code/`: Contains Jupyter notebooks and Python scripts used for data analysis and modeling. These are viewable on GitHub.
   - [0.0-install_requirements.ipynb](./code/0.0-install_requirements.ipynb) ==> Used for installing the required packages, should you want to run the code.
   - [0.1-thesis_dataset.ipynb](./code/0.1-thesis_dataset.ipynb) ==> Overview of the thesis dataset.
   - [3.3.4-model_selection_reliability_testing.ipynb](./code/3.3.4-model_selection_reliability_testing.ipynb) ==> Notebook for Chapter 3 analysis of LLM selection for content analysis
   - [4.2-research_question_1.ipynb](./code/4.2-research_question_1.ipynb) ==> Notebook for Chapter 4 analysis of RQ1
   - [4.3-research_question_2.ipynb](./code/4.3-research_question_2.ipynb) ==> Notebook for Chapter 4 analysis of RQ2
   - [4.4-research_question_3.ipynb](./code/4.4-research_question_3.ipynb) ==> Notebook for Chapter 4 analysis of RQ3

- `datasets/`: Contains datasets that were used analysis and the LLM model selection. These datasets were sanitized and do not contain any personally identifiable information.
   - [50_sample_original.csv](./datasets/50_sample_original.csv) ==> The 50 chat sessions selected at random from 1024 sessions total, PII removed.
   - [50_sample_human_labels.csv](./datasets/50_sample_human_labels.csv) ==> My classification of the 50 chat sessions.
   - [50_sample_4_llm_3_iterations_labels.csv](./datasets/50_sample_4_llm_3_iterations_labels.csv) ==> The same 50 samples, classified by 4 different LLMs, each run 3 times, 600 rows total.
   - [dps-thesis-dataset.csv](./datasets/dps-thesis-dataset.csv) ==> All features and targets used in the data analysis, PII removed. There are chat 87 participants and 78 chat participants who also completed the survey.


## Running the Code

There are two ways you can run the code in this repository. Local or within a docker container.

### Local Setup

Local setup requires you to have Python 3.12 or higher installed on your machine and the required packages listed in `code/requirements.txt`.

1. Install Python 3.12 or higher. 
2. Install the required packages:
   ```bash
   pip install -r code/requirements.txt
   ```
3. Start Jupyter Lab:
   ```bash
   jupyter lab
   ```
4. Observe the running output in your terminal and open the provided URL in your web browser.
The URL will look something like this: `http://localhost:8888/lab?token=your_token_here`. The token is different each time you start Jupyter Lab.
5. Open the running jupyter lab instance in your browser and navigate to the `code/` directory to access the notebooks.


### Docker Setup

The docker setup is the easiest way to get started. It requires you to have Docker installed on your machine. The python environment and pre-requisites are all contained within the docker image.

1. Install [Docker](https://www.docker.com/get-started) on your computer
2. Start jupyter lab within the docker container:
   ```bash
   docker-compose up
   ```
3. Observe the running output in your terminal and open the provided URL in your web browser.
The URL will look something like this: `http://localhost:8888/lab?token=your_token_here`. The token is different each time you start Jupyter Lab.
4. Execute the `code/0.0-install_requirements.ipynb` notebook to install the required packages.


