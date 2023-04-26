# How to Generate Synthetic Data for a Financial Report Using LlamaIndex?

Generating synthetic data can be a game-changer in financial analysis, and with LlamaIndex, it's both efficient and cost-effective. Here's how you can leverage an LLM to create valuable insights without the need for manual labeling.

![Synthetic Data Generation: LlamaIndex and GPT-4o-mini](../images/synthetic_data_llamaindex_financial_report.png)

## The Core Idea: 
Use a Large Language Model (LLM) to generate hypothetical questions that align perfectly with specific pieces of context. This approach allows for the scalable creation of synthetic pairs of (query, chunk context) without relying on human intervention.


## Step-by-Step Process:

- Chunk Your Report: Start by breaking down your financial report into manageable pieces using the SimpleNodeParser from LlamaIndex.
I used a 10K financial report.

- Create Prompt Templates: Design a prompt template that instructs the LLM to generate one or more questions for each chunk of the report. 
In the notebook, I specified that the LLM should behave as a financial analyst and generate questions using key metrics from a financial report

- Generate Answers (Optional): Modify your prompt to have the LLM generate answers based on the questions and context provided.

## Cost:
Example: For the financial report in the notebook, I get 118 nodes. I asked the LLM, using GPT-4o-mini, to generate 3 questions per node. The total cost? Less than $0.02.

## Maintainer

Nikunj Shah - Software Developer

*   [GitHub](https://github.com/)
*   [LinkedIn](https://linkedin.com/)
*   Email: nikunjshah0310@gmail.com
