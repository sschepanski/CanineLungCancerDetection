# Canine-LungCancer-Detection

## Introduction

This project explores the feasibility of using trained dogs to detect lung cancer from patient-worn masks. The dataset captures the performance and detection outcomes of the dogs under various conditions. By understanding the accuracy and factors influencing detection, we aim to assess the potential of canine scent detection as a non-invasive screening tool for lung cancer.

## Goal

The goal of this project is to comprehensively analyze the detection accuracy of trained dogs and investigate factors that influence performance. This could have significant implications for early and non-invasive lung cancer detection.

## Project Structure

- **`data/`**: Dataset files related to training sessions and detection outcomes.
- **`graphs/`**: Output graphs related to the analysis and detection outcomes.
- **`models/`**: Models related to statistical analysis and model evaluation.
- **`scr/`**: Jupyter notebooks for data exploration, preprocessing, and analysis.

## Analysis

1. **Data Exploration**: Analyze the structure and content of the datasets, understand the documented variables, and their relationships.
2. **Data Preprocessing**: Clean and structure the data, including adding missing rows to represent negative detections accurately.
3. **Exploratory Data Analysis (EDA)**: Visualize the distribution of variables and relationships to gain insights.
4. **Detection Analysis**: Evaluate the detection accuracy of the dogs and identify patterns related to influencing factors.
5. **Feature Engineering**: Refine and create new variables to improve the analysis.
6. **Model Evaluation**: Assess the statistical models used to interpret the dogs' detection capabilities and evaluate influencing factors.
7. **Fine-Tuning**: Iteratively adjust models and methods to optimize results.
8. **Feature Importance**: Identify which conditions or factors most significantly affect detection performance.
9. **Conclusion**: Summarize the findings and implications of the analysis for future research and potential clinical use.

## Data Dictionary

| Feature                            | Description                                                   |
|-------------------------------------|---------------------------------------------------------------|
| `Anlagen_Nr.`                       | Identification number for each detection session.             |
| `Board_Nr.`                         | Identification number for each mask board used.               |
| `Hund`                              | Name of the dog involved in the detection task.               |
| `postive_Maske`                     | Indicates if the mask was positive for lung cancer (Ja/Nein). |
| `Maske_angezeigt`                   | Whether the dog signaled a positive detection (angezeigt).    |
| `Verleitungsmaske`                  | Indicates if a decoy mask was present.                        |
| `Verleitungsmaske_angezeigt`        | Whether the dog falsely signaled on a decoy mask.             |
| `Anzahl_Suchboards`                 | Total number of search boards used in the session.            |
| `Zufallsgenerator_Anzahl_positiv`   | Number of boards with positive masks determined randomly.     |
| `Zufallszahl_positiv_Suchboardnr.`  | Specific board numbers with positive masks.                   |
| `Detection_Accuracy`                | Overall accuracy of the dog's detection performance.          |

## Acknowledgements

This research is based on data provided by Dogscan GmbH, who documented canine scent detection for lung cancer screening. The preprint has been published here [Grah, C., Oei, S. L., Ngandeu Schepanski, S., Wuestefeld, H. F., Blazejczyk, K., Kalinka-Grafe, J., & Seifert, G. (2026). Feasibility Study on Training Dogs to Detect Lung Cancer: Findings of a Retrospective Evaluation. medRxiv, 2026-02.](https://doi.org/10.64898/2026.02.04.26345351)

## Getting Started

1. **Clone this repository:**

   ```bash
   git clone https://github.com/sschepanski/canine-lungcancer-detection.git
   ```
2. **Set up your environment using the provided requirements file:**
   ```bash
   pyenv local 3.11.3
   python -m venv .venv
   source .venv/bin/activate
   pip install --upgrade pip
   pip install -r requirements.txt
   ```
3. **Run the provided notebooks in the scr/ directory to preprocess data, perform analysis, and evaluate results.**
   
## **Contributions**

This project was conducted by Dr. Steven Schepanski.

## **License**

This project is licensed under the MIT License.