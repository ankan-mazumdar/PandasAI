# PandasAI - Enhancing MYSQL(local DB)and  Pandas with Generative AI

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


<img width="658" alt="Screenshot 2024-11-24 at 7 44 12 PM" src="https://github.com/user-attachments/assets/55b5270a-a86f-4500-a94d-5d2e49be887a">

![image](https://github.com/user-attachments/assets/a779e8a5-abdc-4b95-b123-da13a162e7c9)

![image](https://github.com/user-attachments/assets/92388f8c-5d31-41bf-8244-7bde9f1a199b)

![image](https://github.com/user-attachments/assets/26c98954-6a43-4577-a6d1-c26aec64bb37)

![image](https://github.com/user-attachments/assets/a8dc699e-8c4c-4241-9d5c-9493185a06ed)

![image](https://github.com/user-attachments/assets/fe50814b-7abf-4679-af10-a2f42d309ae3)

<img width="274" alt="Screenshot 2024-11-24 at 8 04 38 PM" src="https://github.com/user-attachments/assets/9cd5c924-b210-4587-9821-f6b2b4ecbfd5">


![image](https://github.com/user-attachments/assets/15969eb3-54f4-4e82-b358-ddf6aeaf0eb6)

![image](https://github.com/user-attachments/assets/9920f4d9-29cc-49b1-a49d-0b6a2204cfc4)

<img width="454" alt="Screenshot 2024-11-24 at 8 06 31 PM" src="https://github.com/user-attachments/assets/c54f15c3-47fb-4784-9898-9455690548d9">

![image](https://github.com/user-attachments/assets/c57f0d28-2538-478b-a69d-4a367fd06604)

![image](https://github.com/user-attachments/assets/d59e06f3-06a4-4d9d-a974-551cd6192a56)


![image](https://github.com/user-attachments/assets/15dee406-5d84-4074-b5b4-7578ad22b0c5)


![image](https://github.com/user-attachments/assets/7544f00c-bc4e-4f8f-b40f-8ee9f3c889ae)



