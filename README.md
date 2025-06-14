# **PIT-UN Project 4**: Narrative Intelligence and Impact Signatures of Flash Flood Events in D.C., Maryland, and Virginia

## Project Objectives
The primary goal of this project is to improve understanding of the impacts of the flash floods in Washington, D.C., and its neighboring counties in Maryland and Virginia by utilizing data science techniques. We focus on events from 1996 to the present that include narrative description, with the primary objectives to extract structured impact information from unstructured event narratives using large language models (LLMs), compute a Flood Impact Score (FIS) for each event, and analyzing contextual patterns such as co-occurence of impact types, spatial clustering, and temporal trends. Ultimately, we intend to obtain findings that can be used to inform resilience strategies and emergency planning by identifying high-impact flood scenarios. 

## Data Sources
Data used in this project is sourced from the National Oceanic and Atmospheric Administration’s (NOAA) Storm Events Database. This dataset provides information about flash floods in the D.C., Maryland, and Virginia area from 1996 to the present. A key feature of this dataset is its inclusion of “narratives”: qualitative descriptions of each flood event. 
Link to dataset: https://www.ncdc.noaa.gov/stormevents/ftp.jsp

## How to Run Code
To run the code, users should open the data_model_code.ipynb file and execute each cell sequentially. The workflow is chronological: it begins with downloading and filtering the raw NOAA data, then applies LLMs to extract structured impact tags from the narrative text. Then, we compute the Flood Impact Score (FIS) for each event and generate visual analytics. 

## Summary of Contents and File Structure
1. README.md: Introduction that includes information about the project, the developers, and the project repository.
2. License.txt: License file with MIT.
3. Inside the csv_files folder:
    - **NEW_TAG_dc_md_va_flashfloods_1996_pres.csv**: a CSV file that contains original data from NOAA's storm database, containing information about flash flood events.
    - **dc_md_va_flashfloods_1996_pres.csv**: a version of the original CV data file that includes ~900 manually labeled observations with tags.
    - **tag_corpus.csv**: includes the tags with the synonyms/words that correspond to each one. 
4. Inside the spatial_temporal_data:
    - **cb_2024_us_county_500k.zip**: shape file for counties in the U.S.
5. **data_model_code.ipynb**: a Jupyter Notebook File containing the code for creating the tagging classification method, data visualizations, and FIS_score model.
6. **TechnicalReport.pdf**: a PDF of our technical report, made using the LaTeX editor Overleaf.

## Meet the Team

**Jessica Lin** is a rising junior from Northern Virginia, studying Data Science and Psychology at Wellesley College.

**Danielle Sitalo** is a rising junior from Texas, studying Statistics at Texas A&M University. 

**Emma Zou** is a rising sophomore from Maryland, studying Applied Math-Computer Science and Music at Brown University. 

## Acknowledgments
PIT-UN contributed funding for this work. PIT-UN is a project of the New Venture
Fund (NVF), a 501(c)(3) public charity that supports innovative and effective
public interest projects.
