# Blockchain Applications for Sustainable Development in the EU Public Sector: Insights from AI-Based SDG Mapping

### A. Paula Rodriguez Müller(1), Jaume Martin Bosch(2), Marco Combetto(3), Luca Tangi(4)

* (1)European Commission, Joint Research Centre, Seville, Spain 
* (2)Engineering International Belgium S.A., Brussels, Belgium 
* (3)Fincons S.p.A., Vimercate, Italy
* (4)European Commission, Joint Research Centre, Ispra, Italy

---------------------------------------------------------
BLOCKCHAIN USECASE DATASET
---------------------------------------------------------
## Dataset Details
- **Dataset Name:** bc4sdgs_202507_merged_upd_pub.csv
- **Dataset Description:** list of selected blockchain usecases used in the research. 
- **Data source:** [Public Sector Tech Watch](https://interoperable-europe.ec.europa.eu/collection/public-sector-tech-watch)
- **Data extraction date:** July 2025
- **Number of blockchain cases:** 306
- **License:** CC-BY 4.0

The dataset schema is the PSTW schema documented here https://publications.jrc.ec.europa.eu/repository/handle/JRC137409
The dataset has been enriched with additional columns for each SDG that are the following: 

| Column Name                          | Description                                                         |
| ------------------------------------ | ------------------------------------------------------------------- |
| `SDG_[n]_vote`                       | Vote assigned by the automatic keywords match                       |
| `SDG_[n]_vote_rev`                   | Vote assigned by the human expert                                   |
| `SDG_[n]_vote__4o_t01_202507`        | Vote assigned by the gpt-4o LLM                                     |
| `SDG_[n]_vote__llama3_t01_202507`    | Vote assigned by the Llama3 LLM                                     |
| `SDG_[n]_comment`                    | Text comment to the vote assigned with the automatic keywords match |
| `SDG_[n]_comment__4o_t01_202507`     | Text comment to the vote assigned by gpt-4o LLM                     |
| `SDG_[n]_comment__llama3_t01_202507` | Text comment to the vote assigned by Llama 3 LLM                    |


---------------------------------------------------------
SDGS DATASET
---------------------------------------------------------
## Dataset Details
- **Dataset Name:** sdgs.csv
- **Dataset Description:** list of SDGs names, definitions and keywords
- **Data source:** [United Nations SDGs](https://sdgs.un.org/goals)
  **License:** CC-BY 4.0


--------------------------------------------------------
SOURCE CODE
---------------------------------------------------------
## Code Details
- **File Name:** BC4SDGs_Evaluator.ipynb
- **File Type:** Jupyter Notebook (Python)
- **Description:** This notebook is the analytical tool used to qualitatively evaluate a dataset of 306 blockchain use cases against the 17 United Nations Sustainable Development Goals (UN SDGs). It applies the official SDG definitions as the evaluation framework and uses a language-model-based pipeline to assign a score and supporting rationale for each use case across all 17 goals. The notebook also manages data loading, result storage, and supporting explainability functions, enabling a structured and reproducible assessment of how each blockchain use case aligns with the UN SDG agenda.
- **License:** AGPL




last update: 27 february 2026


