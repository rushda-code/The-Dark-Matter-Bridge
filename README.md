# The Dark Matter Bridge – AI Search Attribution

This project explores how AI-driven search behavior can be estimated and probabilistically attributed to unexplained direct website traffic. The goal is to bridge the gap between traditional analytics and emerging AI-assisted discovery.

## Project Overview
Traditional analytics tools capture keyword-based searches but fail to account for AI-generated queries. This project:
- Estimates hidden AI prompt volume using search volume, intent, and query complexity
- Clusters AI prompts into intent groups
- Probabilistically attributes direct website sessions to these intent clusters

## Repository Contents
- `The__Dark_Matter__Bridge_.ipynb`  
  Jupyter notebook containing:
  - AI prompt generation using the **Groq API**
  - Intent clustering and complexity scoring  
  - AI volume estimation logic  
  - Probabilistic attribution of direct traffic sessions
- `direct_traffic_sessions.csv`  
  Dataset containing anonymized direct traffic session behavior used for attribution
- `README.md`  
  Project documentation (this file)

## Methodology Summary
- **Volume Estimation:** Combines Google Monthly Search Volume, intent weighting, and prompt complexity to estimate AI search volume.
- **Prompt Generation:** Uses the Groq API to generate diverse AI search prompts reflecting real-world user queries.
- **Attribution Logic:** Applies a probabilistic approach where intent volume acts as a prior and session behavior (time, scroll, actions) acts as likelihood.
- **Outcome:** Assigns the most likely intent cluster to each direct session along with a confidence score.

## How to Run
1. Open the notebook in Jupyter or Google Colab
2. Ensure the CSV file is in the same directory
3. Set the Groq API key as an environment variable
4. Run cells sequentially to reproduce results

## Notes
- AI tools were used responsibly for ideation and prototyping, with all modeling logic and assumptions explicitly defined in the notebook.


