# Michael Fudge's DPS Thesis Repository

    Michael Fudge
    Doctor of Professional Studies (DPS) Candidate
    The School of Information Studies at Syracuse University
    Email: mfudge@syr.edu
    ORCID: 0009-0006-2760-9360


This repository contains the code and resources for my Doctor of Professional Studies (DPS) thesis. 

My thesis investigates the impact of Large Language Models (LLMs) use on learning and computational literacy. 


## Contents

- `code/`: Contains Jupyter notebooks and Python scripts used for data analysis and modeling.
- `datasets/`: Contains datasets used in the analysis. This datasets are sanitized and do not contain any sensitive information.
- `thesis/`: Contains the thesis document.


## Getting Started

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


## Contents

### Notebooks

The main notebooks used for analysis can be found in the `code/` directory.

- `0.0-install_requirements.ipynb` ==> Install the required packages
- `0.1-thesis_dataset.ipynb` ==> Notebook load the Thesis for user exploration
- `3.3.4-model_selection_reliability_testing.ipynb` ==> Notebook for Chapter 3 analysis of model selection for content analysis
- `4.2-research_question_1.ipynb` ==> Notebook for Chapter 4 analysis of RQ1
- `4.3-research_question_2.ipynb` ==> Notebook for Chapter 4 analysis of RQ2
- `4.4-research_question_3.ipynb` ==> Notebook for Chapter 4 analysis of RQ3

### Datasets

The datasets used in the analysis can be found in the `datasets/` directory. These datasets are sanitized and do not contain any personally identifiable information.

Samples for model selection:

- `50_sample_original.csv` ==> The original 50 chat sessions selected at random from 1024 sessions, PII removed.
- `50_sample_human_labels.csv` ==> My classification of the 50 chat sessions.
- `50_sample_4_llm_3_iterations_labels.csv` ==> The same 50 samples, classified by 4 different LLMs, each run 3 times, 600 rows total.

Samples in the final data analysis:

- `dps-thesis-dataset.csv` ==> All features and targets used in the data analysis, PII removed. There are chat 87 participants and 78 chat participants who also completed the survey.

#### Data Dictionary for `dps-thesis-dataset.csv`

One row per participant

| Column Name       | Description                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| participant_number | The unique identifier of each participant. |
| survey_done        | Whether the participant completed the survey. Either "Yes" or "No". |
| chatbot_done       | Whether the participant engaged with the chatbot. Either "Yes" or "No". |
| chatbot_group      | The AI group the participant was assigned to. Either "Control" or "Treatment". |
| first_year         | From the survey: Is the participant a first-year student. Either "Yes" or "No". |
| gender             | From the survey: The gender of the participant. |
| first_prog_course  | From the survey: Is this the participant's first programming course. Either "Yes" or "No". |
| C1 | The Participant's score on the first computational diagnostic (max=28) |
| C2 | The Participant's score on the second computational diagnostic (max=28) |
| E1 | The Participant's score on the Midterm Exam (max=45) |
| Difference_C2_C1 | The difference between the second and first computational diagnostic (C2 - C1) |
| inconclusive_session_count | Count of Chat sessions labeled as inconclusive. |
| task_completion_session_count | Count of Chat sessions labeled as "Task Completion". |
| learning_session_count | Count of AI sessions labeled as "Learning". |
| total_session_count      | The total number of AI sessions. |
| total_interaction_count  | The total number of interactions. An interaction is defined as the number of user prompts in a 


