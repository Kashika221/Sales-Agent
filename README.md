# Sales-Agent

An interactive **AI-powered sales conversation agent** implemented in a Jupyter Notebook. This repository contains the notebook `Sales_agent_Kashika.ipynb`, which demonstrates how to use a large language model (LLM) to simulate sales dialogue, capture user preferences, and generate relevant product recommendations.

This project is ideal for exploring how modern generative AI can be used to model structured conversation flows such as sales assistance or customer engagements.

---

## Table of Contents

* Overview
* Features
* Requirements
* Installation
* Usage
* How It Works
* Results & Outputs
* Customization
* Contributing
* License

---

## Overview

**Sales-Agent** is a Python notebook that walks through the creation of an AI-driven sales assistant. Using a generative AI model, the notebook demonstrates:

* A multi-turn sales dialogue loop
* Collection of user preferences (budget, features, product type)
* Conversion of user input into structured product recommendations
* Export or display of the conversation transcript

This notebook can serve as a template for building custom conversational agents, especially for sales or customer support use cases.

---

## Features

* AI-generated conversational responses based on user input
* Step-by-step sales dialogue logic
* Demonstrates integration with a large language model (LLM)
* Easy to run interactively within Jupyter Notebook
* Outputs conversation flow clearly for analysis

---

## Requirements

To run this notebook, you will need the following:

* Python 3.8 or later
* Jupyter Notebook or Jupyter-compatible environment (e.g., JupyterLab, VS Code)
* An API key for a generative language model (OpenAI GPT, Google Gemini, etc.)
* Internet access to query the LLM

Common Python packages:

* `openai` or other LLM SDK
* `pandas` (optional, for data handling)
* `json` (built-in)
* `os`, `dotenv` (for managing environment variables)

You will need to install these packages via pip:

```bash
pip install openai pandas python-dotenv
```

---

## Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/Kashika221/Sales-Agent.git
   cd Sales-Agent
   ```

2. **Set Up Environment Variables**

   Create a `.env` file at the root of the repo:

   ```
   API_KEY=<your_llm_api_key_here>
   ```

   This file will be used by the notebook to authenticate with your chosen LLM provider.

3. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

   If a `requirements.txt` is not present, manually install:

   ```bash
   pip install openai python-dotenv pandas
   ```

---

## Usage

1. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

2. Open the file:

   ```
   Sales_agent_Kashika.ipynb
   ```

3. Step through the notebook cells from top to bottom.

4. When prompted, enter your API key (or use the environment variable), and then interact with the agent:

   * Provide your name or persona
   * Specify the product category of interest
   * Enter preferences (budget, features)
   * Receive AI-generated recommendations

---

## How It Works

The notebook uses a basic multi-turn dialog loop:

1. **Initialize** — set up environment, load API key
2. **Prompt Construction** — define message templates for each step of the sales flow
3. **Model Calls** — send user + system messages to the LLM
4. **Response Parsing** — extract intent, suggestions, or next-step prompts
5. **Loop** — continue until the conversation completes
6. **Record and Display** — show final output and conversation history

This structure can be adapted for any agent workflow beyond sales (support, onboarding, FAQs).

---

## Results & Outputs

The notebook demonstrates:

* A sample conversation transcript
* Extracted product suggestions based on user constraints
* A flow that can be extended or enhanced with a product database

You may also export results to CSV/JSON for record-keeping.

---

## Customization

Ideas for enhancing this project:

* Connect to a real product catalog API or database
* Add sentiment analysis to adapt conversation tone
* Persist transcripts in a database
* Deploy the logic as a web or mobile application
* Add evaluation metrics for quality of recommendations

---

## Contributing

Contributions and ideas are welcome. Suggested workflow:

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Open a pull request describing your enhancement

---

## License

This repository currently has no license file. If you want to share permissively, consider adding an **MIT License** or a similar open-source license.
