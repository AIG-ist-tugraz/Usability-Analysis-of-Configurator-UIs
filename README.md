# Configurator Usability Analysis

This repository accompanies the paper *Usability Analysis of Configurator UIs with
Multimodal LLMs* and includes the code and data for the analysis of configurator user interfaces using Multimodal Large Language Models (MLLMs). 
The analysis evaluates configurators against a set of predefined usability criteria to identify potential usability issues and areas for improvement.

## Project Structure

- `Usability_Analysis.ipynb`: Main notebook for running the analysis
- `configurator_usability_criteria.json`: Definition of the usability criteria for evaluation
- `data/`: Directory containing sample recordings and input data
- `results/`: Directory containing analysis outputs
  - `Analysis_Results.csv`: Comprehensive analysis results in CSV format (semicolon-delimited)
  - `Analysis_Results.xlsx`: Same analysis results in Excel format for easier filtering and visualization

## Analysis Results

The analysis produces detailed evaluations of configurator interfaces across multiple dimensions. The results files include:

### Data Structure (CSV/Excel)
- **Issue ID**: Unique identifier for each issue
- **Criterion**: The specific usability criterion being evaluated (e.g., 'Customized options', 'Error prevention')
- **Severity**: Classification of the issue (No Issue, Minor Issue, Major Issue)
- **Description**: Detailed description of the usability finding
- **Recommendation**: Suggested improvements or fixes for the identified issue
- **App ID**: Identifier for the application being analyzed as defined in `data/sample_description.json`
- **Criterion ID**: Identifier for the specific criterion as defined in `configurator_usability_criteria.json`

## Getting Started

1. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Run the analysis:
   - Open `Usability_Analysis.ipynb`
   - Paste your Google AI API key into the `GENAI_API_KEY` variable
   - Execute all cells to perform the analysis
