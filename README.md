# PIT-UN-Project4

## Team Member Introductions: 
### Jessica Lin
Jessica is a rising junior from Northern VA. She is at Wellesley College studying Data Science and Psychology. 

### Emma Zou
### Danielle Sitalo

## Narrative Intelligence and Impact Signatures of Flash Flood Events in DC, Maryland, and Virginia

### Project Objectives
1. Download and filter flash flood event data from 1996 to present for Washington, D.C.,
and neighboring counties in Maryland and Virginia, using only events that contain
narrative descriptions.

2. Apply large language models (LLMs) to extract structured impact tags from unstruc-
tured event narratives.

3. Quantify flood severity by computing a composite Flood Impact Score (FIS) for
each event.
4. Explore contextual patterns through co-occurrence of impact types, spatial clustering,
and temporal trends.

5. Develop a data-driven understanding of high-impact flood typologies to inform re-
silience and emergency planning.

--------------------------------------------------------------------------------------------
Each narrative is processed with an LLM to classify presence or absence of the following
impact indicators:

Tag : Description
death : Human fatalities
injury : Physical injuries
evacuation : Any form of population displacement
rescue : Emergency or civilian water rescues
car_crash : Explicit vehicle collisions or crashes
home_damage : Flooded or damaged residences
infrastructure_damage : Roads, bridges, water plants, etc.
school_damage : Impacts on schools or educational buildings
hospital_damage : Impacts on hospitals or clinics
road_closure : Blocked roads or intersections
power_outage : Loss of electricity or power infrastructure

--------------------------------------------------------------------------------------------

### Quantifying Combined Impact: Flood Impact Score (FIS)
Each event receives a Flood Impact Score (FIS) — a weighted sum of the above tags
that quantifies overall severity based on:
• Human impact
• Physical infrastructure disruption
• Service system breakdowns
Weights may be adjusted based on expert judgment, statistical learning, or downstream
modeling needs.

--------------------------------------------------------------------------------------------

### Descriptive and Exploratory Analysis Plan: 
- Tag Frequency Analysis
  • Distribution of impact types across all events.
  • Cross-tabulations by state and decade.

- Tag Co-Occurrence Networks
  • Heatmap and network visualizations showing which tags appear together most often.
  • Identification of characteristic combinations (e.g., rescue + car crash + home damage).
  
- Spatial Analysis
  • Mapping average and maximum FIS by county (VA/MD) and Washington, D.C.
  • Detecting spatial clusters of high-impact events using local spatial statistics.
  
- Temporal Trends
  • Time series of flood counts and average FIS.
  • Analysis of changes over time in narrative complexity or dominant flood typologies.
  • Examination of seasonal patterns (e.g., spring snowmelt vs. summer storms).

--------------------------------------------------------------------------------------------

### Advanced Contextual Analyses
- Flood Typology Clustering
  • Use of LLM-labeled tags to cluster floods into categories such as:
    – “High-disruption, low-casualty”
    – “Urban flash floods with rescues”
    – “Infrastructure-heavy winter floods”
- Risk Prediction Modeling (Optional)
  • Predicting FIS using metadata: date, location, damage estimates.
- Expected Deliverables
  • A structured event-level dataset with LLM-labeled impacts.
  • A derived Flood Impact Score for each event.
  • Visual analytics: tag frequency plots, spatial heatmaps, co-occurrence networks.
  • A replicable method to use LLMs for extracting disaster intelligence from text.
