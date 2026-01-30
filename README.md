# BioVix: An Integrated Large Language Model Framework for Data Visualization, Graph Interpretation, and Literature-Aware Scientific Validation
![License: MIT License](https://img.shields.io/badge/License-MIT-blue.svg)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Streamlit](https://img.shields.io/badge/Streamlit-UI-green)
![Contributors](https://img.shields.io/badge/contributors-4-blueviolet)


## Table of Contents
1. [overview](#overview)
2. [Features](#features)
3. [Prerequisites](#prerequisites)
4. [BioVix Installation](#biovix-installation)
5. [Running BioVix](#running-biovix)
6. [Outputs](#outputs)
7. [Deployment](#deployment)
8. [Tips for Success](#tips-for-success)
9. [Reference](#reference)
10. [License and Issues](#license-and-issues)
11. [Contact Us](#contact-us)

## overview

BioVix is an AI-assisted visualization tool built on Streamlit that streamlines the workflow from data analysis to literature discovery. By integrating Plotly for visualization, DeepSeek V3.1 for query processing, and Semantic Scholar for bibliographic search, it offers a robust analytical environment. Furthermore, the system incorporates GPT-OSS-20B for structured dialogue and Qwen2.5-VL-32B-Instruct for visual graph reasoning, enabling users to gain a deeper understanding of data trends through natural language interaction.


![User Interface](https://github.com/MuhammadZain-Butt/BioVix/blob/main/overview.jpg)

       
## Features

- **Data Upload & Management**: Supports CSV, TSV, and Excel (.xlsx) formats.  
- **AI-Powered Chart Generation**: Create interactive Plotly visualizations from natural language queries.  
- **AI Insights**: Automatically analyze and provide explanations for generated charts.  
- **Academic Research Integration**: Discover relevant research papers via Semantic Scholar.  
- **Graph Interpreter**: Analyze uploaded graph images using AI.  
- **Data Q&A**: Ask questions about your dataset and receive AI-driven answers.  
- **Sample Datasets**: Access pre-loaded datasets for quick testing (Apple Stock, Gene Expression, Hospital Data).  

## Prerequisites

- [Python 3.8+](https://www.python.org/downloads/)
- API keys for:
  - [DeepSeek API (via OpenRouter)](https://openrouter.ai/deepseek/deepseek-chat-v3.1)
  - [GPT API (via OpenRouter)](https://openrouter.ai/openai/gpt-oss-20b:free)
  - [Qwen API (via OpenRouter)](https://openrouter.ai/qwen/qwen2.5-vl-32b-instruct)
  - [Semantic Scholar API](https://www.semanticscholar.org/product/api#api-key)

## BioVix Installation

### 1. Clone the repository

```bash
git clone https://github.com/MuhammadZain-Butt/BioVix.git
cd BioVix
```

### 2. Create a Virtual Environment (Recommended)
It is highly recommended to use a virtual environment to avoid dependency conflicts.

#### Windows:
```powershell
python -m venv env_name
.env_name\Scripts\activate.bat
```
Note: Replace `env_name` with your preferred name for the virtual environment.
#### Linux / macOS:
```powershell
python3 -m venv env_name
source env_name\bin\activate
```
Note: Replace `env_name` with your preferred name for the virtual environment.

### 3. Install Dependencies

```powershell
pip install -r requirements.txt
```

### 4. Configure Environment Variables

Create a `.env` file in the project root directory (as in BioVix):

```
DEEPSEEK_API_KEY="your_deepseek_key_here"
GPT_API_KEY="your_gpt_key_here"
QWEN_API_KEY="your_qwen_key_here"
SEMANTIC_SCHOLAR_API_KEY="your_semantic_scholar_key_here"
```
Tip: If you do not have these API keys, you can create accounts here to generate them:
- [OpenRouter](https://openrouter.ai/models) 
- [Semantic Scholar](https://www.semanticscholar.org/product/api)

## Running BioVix

After installing dependencies and setting up your environment, you can start BioVix using Streamlit.

```powershell
streamlit run app.py
```
Once the command runs, the app will automatically open in your default browser at: `http://localhost:8501`

## Outputs

The following panels illustrate the outputs of BioVix across varying datasets.  **(A)** displays the raw input data, while **(B,C,D)** presents the corresponding interactive visualization rendered with Plotly. **(E)** provides the AI-generated interpretation of the graph, along with the derived search query. Finally, **(F)** lists the relevant research papers retrieved from Semantic Scholar using the formulated query: 

- **Figures**:
  1. **Gene-level Protein Expression Dataset**
      
     ![Gene-level Protein Expression](https://github.com/MuhammadZain-Butt/BioVix/blob/main/results/Figure%2004.jpg)
     
  2. **Peak Annotation dataset**
     
     ![Peak Annotation dataset](https://github.com/MuhammadZain-Butt/BioVix/blob/main/results/Figure%2005.jpg)
     
  3. **Clinical Diabetic Dataset**
     
     ![Clinical Diabetic Dataset](https://github.com/MuhammadZain-Butt/BioVix/blob/main/results/Figure06.jpg)



## Deployment

BioVix is deployed on Hugging Face and can be tested or used by users directly, [click here](https://huggingface.co/spaces/MuhammadZain10/BioVix)

## Tips for Success

- Ensure that input files are correctly formatted (e.g., CSV, XLSX, or TSV) and contain all information required for visualization.
- Write queries in a clear and detailed manner, and avoid using informal language.
- Use consistent naming conventions for columns and variables to improve clarity and interpretation.
  

## Reference
In Process.

## License and Issues

This BioVix is licensed under the MIT License - see the [LICENSE](License) file for details.
Submit issues or contributions via [GitHub Issues](https://github.com/MuhammadZain-Butt/BioVix/issues).


## Contact Us
For any questions or issues, please contact us at:
- **Mr. Muhammad Zain Butt**: [zain.202302328@gcuf.edu.pk](mailto:zain.202302328@gcuf.edu.pk)
- **Mr. Rana Sheraz Ahmad**: [ranasheraz.202101902@gcuf.edu.pk](mailto:ranasheraz.202101902@gcuf.edu.pk)
- **Ms. Eman Fatima**: [eman.202204127@gcuf.edu.pk](mailto:eman.202204127@gcuf.edu.pk)
- **Dr. Muhammad Tahir ul Qamar**: [m.tahirulqamar@hotmail.com](mailto:tahirulqamar@gcuf.edu.pk)




