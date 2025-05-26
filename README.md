# LLM-Based Natural Language to SPARQL translation over a domain specific Rail Knowledge Graph
This repository contains our:

- [Project Source Code](https://github.com/mhrjabary/NL-TO-SPARQL-RINF/tree/main/Source%20Code)
- [Competency Questions & Coressponding SPARQL Queries](https://github.com/mhrjabary/NL-TO-SPARQL-RINF/tree/main/Experiment%20Results)
- [Experiment Results](https://github.com/mhrjabary/NL-TO-SPARQL-RINF/tree/main/Experiment%20Results)
- [Project Design and Implemetation Figures and ALgorithms](https://github.com/mhrjabary/NL-TO-SPARQL-RINF/tree/main/Figures)

## Introduction
This research paper presents a zero-shot LLM-Based approach to translate natural language queries into SPARQL over domain-specific KG. Experiments were conducted to examine and evaluate the capabilities of LLMs using GPT and Gemini to translate NL questions to SPARQL queries targeting the European Union Agency for Railways (Agency) Knowledge Graph (KG). Our approach proposes an unadorned fashion approach to perform a zero-shot SPARQL query generation by augmenting LLMs with different arrangements of previously extracted KG information without any prior natural language processing techniques on the input text. Experiment results indicates that augmenting LLM with vocabulary information extracted from a reduced KG ontology shows competitive performance levels for targeted LLM models compared to supplementing LLM with a reduced version of KG. Ultimately, our approach allows benchmarking over a wide spectrum of LLMs models, reduces the augmented KG information size while preserving response accuracy, and allowing off-domain users to interact with KG information and retrieve responses more effectively.

## Design and Implementation
Our proposed test bed is used to explore the ability of LLM to generate SPARQL queries and retrieve information from a domain-specific KG using NL questions using two scenarios. As illustrated the Figure below, our method involves generating an enhanced prompt augmented with in-domain KG ontology vocabulary information extracted from the Register of Infrastructure (RINF) ontology KG. The generated prompt is then fed to the LLM in the form of a zero-shot prompt[15][8 ] to translate the NL question into a SPARQL query, which is used to obtain the answer from the ERA SPARQL endpoint. All Project Design and Implemetation Figures and ALgorithms [can be found here](https://github.com/mhrjabary/NL-TO-SPARQL-RINF/tree/main/Figures)
![Proposed Model Design](https://github.com/user-attachments/assets/880db58b-ee9d-44bc-a51a-24151e081392)


## Experiment Results
Experiment Results including all questions, question justification, and corresponding SPARQL queries for both Models: can be found [here](https://github.com/mhrjabary/NL-TO-SPARQL-RINF/tree/main/Experiment%20Results)

## Visual Studio Code Standalone Deployment, you will need to supply a paied version of chatGBT and Gemini API to handle the amount of passed tokens.
You can deploy our work locally through Microsoft VSCode.
1. Download the project files from [Source Code]([https://github.com/mhrjabary/LLMBased-NL-SPARQL/tree/main/VScode](https://github.com/mhrjabary/NL-TO-SPARQL-RINF/tree/main/Source%20Code)).
2. Look for `openai.api_key = ""`, and `genai.configure(api_key= "")` and use your own API keys.  
3. write a question inside the code, look for the variable `nl_input = ""` and write your question.
4. Copy the generated SPARQL query and paste it on the SPARQL endpoint using this [Link](https://data-interop.era.europa.eu/endpoint)

## Experiments Resources
- Experiment Results including all questions, question justification, and corresponding SPARQL queries for both Models: [CQ](https://github.com/mhrjabary/LLMBased-NL-SPARQL/blob/main/Experiment%20results%20sheet%201.1.xlsx)
- Score results for each prompt (P1,P2, and P3) for both Gemini and OPENAI GPT 3.5-Turbo for 20 Compatancy Questions: [Score](https://github.com/mhrjabary/LLMBased-NL-SPARQL/blob/main/Experiment%20Results%20percentage.xlsx)
- All prompts P1,P2, and P3: [P1](https://github.com/mhrjabary/NL-TO-SPARQL-RINF/blob/main/Figures/Prompt%20P1.jpeg), [P2](https://github.com/mhrjabary/NL-TO-SPARQL-RINF/blob/main/Figures/Promtp%20P2.jpeg), and [P3](https://github.com/mhrjabary/NL-TO-SPARQL-RINF/blob/main/Figures/Promtp%20P3.jpeg)
- Reduced RINF Ontology Graph: [Generated Reduced Graph](https://github.com/mhrjabary/NL-TO-SPARQL-RINF/blob/main/Ontology/reduced_graph.ttl)

## Public Resources
- The European Union Agency for Railways SPARQL endpoint [Here](https://data-interop.era.europa.eu/endpoint)
- The European Union Agency for Railways Vocabulary [Here](https://data-interop.era.europa.eu/era-vocabulary/)

