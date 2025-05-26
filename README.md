# LLM-Based Natural Language to SPARQL translation over a domain specific Rail Knowledge Graph
This repository contains our:

- [Project code](https://github.com/mhrjabary/NL-TO-SPARQL-RINF/tree/main/Source%20Code)
- [Competency Questions](https://github.com/mhrjabary/NL-TO-SPARQL-RINF/tree/main/Experiment%20Results)
- [Experiment results](https://github.com/mhrjabary/NL-TO-SPARQL-RINF/tree/main/Experiment%20Results)
- [Project Design aand Implemetation Figures and ALgorithms](https://github.com/mhrjabary/NL-TO-SPARQL-RINF/tree/main/Figures)

## Introduction
This research paper presents a zero-shot LLM-Based approach to translate natural language queries into SPARQL over domain-specific KG. Experiments were conducted to examine and evaluate the capabilities of LLMs using GPT and Gemini to translate NL questions to SPARQL queries targeting the European Union Agency for Railways (Agency) Knowledge Graph (KG). Our approach proposes an unadorned fashion approach to perform a zero-shot SPARQL query generation by augmenting LLMs with different arrangements of previously extracted KG information without any prior natural language processing techniques on the input text. Experiment results indicates that augmenting LLM with vocabulary information extracted from a reduced KG ontology shows competitive performance levels for targeted LLM models compared to supplementing LLM with a reduced version of KG. Ultimately, our approach allows benchmarking over a wide spectrum of LLMs models, reduces the augmented KG information size while preserving response accuracy, and allowing off-domain users to interact with KG information and retrieve responses more effectively.

## Design and Implementation



## Experiment Results



## Visual Studio Code Standalone Deployment
You can deploy our work locally through Microsoft VSCode.
1. Download the project files from [VScode folder](https://github.com/mhrjabary/LLMBased-NL-SPARQL/tree/main/VScode).
2. Look for `openai.api_key = ""`, and `genai.configure(api_key= "")` and use your own API keys.  
3. write a question inside the code, look for the variable `nl_input = ""` and write your question.
4. Copy the generated SPARQL query and paste it on the SPARQL endpoint using this [Link](https://data-interop.era.europa.eu/endpoint)

## Demo Usage Tips
It is important to note that LLM inherently may not provide a consistent answer on every run; if the query fails initially, trying again may yield an answer.

## Experiments Resources
- Experiment Results including all questions, question justification, and corresponding SPARQL queries for both Models: [CQ](https://github.com/mhrjabary/LLMBased-NL-SPARQL/blob/main/Experiment%20results%20sheet%201.1.xlsx)
- Score results for each prompt (P1,P2, and P3) for both Gemini and OPENAI GPT 3.5-Turbo for 20 Compatancy Questions: [Score](https://github.com/mhrjabary/LLMBased-NL-SPARQL/blob/main/Experiment%20Results%20percentage.xlsx)
- All prompts P1,P2, and P3: [P1](https://github.com/mhrjabary/LLMBased-NL-SPARQL/tree/main/Prompts), [P2](https://github.com/mhrjabary/LLMBased-NL-SPARQL/tree/main/Prompts), and [P3](https://github.com/mhrjabary/LLMBased-NL-SPARQL/tree/main/Prompts)
- Reduced RINF Ontology Graph: [Generated Reduced Graph](https://github.com/mhrjabary/LLMBased-NL-SPARQL/blob/main/reduced_graph.ttl)

## Public Resources
- The European Union Agency for Railways SPARQL endpoint [Here](https://data-interop.era.europa.eu/endpoint)
- The European Union Agency for Railways Vocabulary [Here](https://data-interop.era.europa.eu/era-vocabulary/)

