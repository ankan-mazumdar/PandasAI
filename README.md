# PandasAI - Enhancing Pandas with Generative AI

A Python library that extends Pandas capabilities using generative AI models for advanced data analysis and manipulation.

## Features

- Enhanced data preprocessing and cleaning
- Complex data manipulations using natural language
- Pattern detection and outlier analysis
- Missing value handling through AI
- Data visualization using simple prompts
- Support for multiple LLM backends

## Supported LLM Integrations

- OpenAI models
- HuggingFace models (Starcoder, Falcon)
- Google PaLM
- Google VertexAI
- Azure OpenAI
- LangChain models

## Installation

```bash
pip install pandasai
```

## Quick Start

```python
import pandas as pd
from pandasai import PandasAI
from pandasai.llm.openai import OpenAI

# Set up OpenAI
import os
openai_api_key = os.environ["OPENAI_API_KEY"]
llm = OpenAI(api_token=openai_api_key)

# Initialize PandasAI
pandas_ai = PandasAI(llm)

# Load your data
df = pd.read_csv("your_data.csv")

# Run analysis with natural language
response = pandas_ai.run(df, prompt='Your analysis question here')
```

## Alternative LLM Setup

```python
# Google PaLM
from pandasai.llm.google_palm import GooglePalm
llm = GooglePalm(api_token="YOUR_GOOGLE_API_KEY")

# Starcoder
from pandasai.llm.starcoder import Starcoder
llm = Starcoder(api_token="YOUR_HF_API_KEY")

# Falcon
from pandasai.llm.falcon import Falcon
llm = Falcon(api_token="YOUR_HF_API_KEY")
```

## Features

- **Data Analysis**: Query your data using natural language
- **Data Visualization**: Create plots and charts with simple prompts
- **Statistical Analysis**: Perform complex calculations using conversational language
- **Pattern Recognition**: Identify trends and patterns in your data
- Clean datasets by addressing missing values.
- Enhance data quality through feature generation.
- Connect to various data sources like CSV, XLSX, PostgreSQL, MySQL, BigQuery, Databrick, Snowflake, etc.

## Example Usage

```python
# List top entries
response = pandas_ai.run(df, prompt='List the first 5 job titles by salary')

# Calculate averages
response = pandas_ai.run(df, prompt='What is the average salary by job titles?')

# Create visualizations
response = pandas_ai.run(df, prompt='Plot a bar chart showing top 10 job titles')
```

## Requirements

- Python 3.6+
- pandas
- API key for chosen LLM provider

[3] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/14488466/4e9454ba-cc90-468c-a658-558b4d730396/Presentation-1.pptx

### Features:

- Ask questions about your data in natural language.
- Generate plots to visualize your data.




