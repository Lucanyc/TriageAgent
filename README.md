# TriageAgent

[EMNLP 2024 Findings] TriageAgent: Towards Better Multi-Agents Collaboration for Large Language Model-Based Clinical Triage

Paper: https://openreview.net/pdf?id=R5YLhou5PX

We propose a dynamic multi-agent collaboration framework. The framework illustrates the reasoning process through five stages when given clinical documents with questions as input: 1). \textbf{Allocating Documents}: Patient clinical records are assigned to expert agents to initiate ESI discussions. 2).\textbf{Group-Based Proposition Analysis}: Agents are divided into two groups to combine \textbf{coarse} and \textbf{fine-grained} classification. 3). \textbf{Confidence Report Summarization}: A summarized report is created based on previous analysis, incorporating \textbf{confidence scores}. 4).\textbf{Collaborative Discussion}: Agents discuss the summarized report, iteratively revising it according to the key information, rationales, and confidence scores. In this step, an \textbf{early-stopping mechanism} is triggered by consistent high confidence scores with \textbf{evidence} across multiple rounds. The cross sign in the figure represents incorrect classifications, while the tick sign represents correct results proposed by the agents. 5).\textbf{Consensus Agreement}: The ultimate result is precise and thoroughly validated, highlighting the importance of collaborative decision-making.

[Main-structure-1.pdf](https://github.com/user-attachments/files/17099495/Main-structure-1.pdf)


Requirements

Install all required python dependencies:

pip install -r requirements.txt

Data
We release our clinical triage dataset collected from the Emergency Severity Index, Version 4: Implementation Handbook. Please check our Google Drive: 
https://drive.google.com/drive/folders/1vSgAOwaj-T7YNmQ3B_JP9RTX9c-5im0P



Implementations
Input your own openai api key in api_utils.py.
sh inference.sh


Cite Us
If you find this project useful, please cite the following paper:
