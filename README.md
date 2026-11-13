# Configurator Usability Analysis

This repository accompanies the paper *Usability Analysis of Configurator UIs with
Multimodal LLMs* and includes the code, data, and evaluation results for the analysis of configurator user interfaces using a Multimodal Large Language Models (MLLM).
The analysis evaluates configurators against a set of predefined usability criteria to identify potential usability issues and areas for improvement.

## Project Structure

- `Usability_Analysis.ipynb`: Main notebook for running the analysis
- `Results_Summary.ipynb`: Notebook for visualizing and summarizing the analysis results
- `Evaluation.ipynb`: Notebook for the computation of evaluation metrics used in the paper
- `configurator_usability_criteria.json`: Definition of the usability criteria for evaluation
- `data/`: Directory containing sample recordings and input data
- `report/`: Directory containing the raw MLLM analysis reports
  - `analysis_report.json`: Detailed report of the analysis in JSON format created by the MLLM
- `results/`: Directory containing analysis outputs, evaluation results, and visualizations
  - `Analysis_Results.csv`: MLLM analysis results in CSV format
  - `Evaluations.csv`: Evaluation results of human reviewers in CSV format
  - `severity_by_configurator.png`: Bar plot showing severity distribution per configurator
  - `severity_by_criterion.png`: Bar plot showing severity distribution per usability criterion

## Analysis Results

The analysis produces detailed evaluations of configurator interfaces across multiple dimensions. The results files include:

### Data Structure (CSV)
- **Criterion**: The specific usability criterion being evaluated (e.g., 'Customized options', 'Error prevention')
- **Severity**: Classification of the issue (No Issue, Minor Issue, Major Issue)
- **Description**: Detailed description of the usability finding
- **Recommendation**: Suggested improvements or fixes for the identified issue
- **App ID**: Identifier for the application being analyzed as defined in `data/sample_description.json`
- **Criterion ID**: Identifier for the specific criterion as defined in `configurator_usability_criteria.json`
- **Request Duration**: Duration of the LLM request in seconds

## Getting Started

1. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Run the analysis:
   - Open `Usability_Analysis.ipynb`
   - Paste your Google AI API key into the `GENAI_API_KEY` variable
   - Execute all cells to perform the analysis
  
## How to Cite

If you want to cite the research paper, we suggest using the following reference:

```
@InProceedings{10.1007/978-3-032-40763-4_10,
    author="Lubos, Sebastian and Felfernig, Alexander and Garber, Damian and Kralji{\'{c}}, Adnan and Kralji{\'{c}}, Tarik and Le, Viet-Man and Tran, Thi Ngoc Trang and Leitner, Gerhard and Schwazer, Julian and Suppan, Doris and Willfort, Reinhard and Dukic, Ivan and Fuchs, Jeremias and Henrich, Manuel",
    editor="Perrouin, Gilles and Berger, Thorsten and Papadopoulos, George A. and Schaefer, Ina and Fortz, Sophie",
    title="Usability Analysis of Configurator User Interfaces with Multimodal Large Language Models",
    booktitle="Software and Systems Reuse, Product Lines, and Configuration",
    year="2027",
    publisher="Springer Nature Switzerland",
    address="Cham",
    pages="170--190",
    isbn="978-3-032-40763-4"
}
```
