# UGGroup11 Social Media Analysis A2

This project analyses online communication about hantavirus across Bluesky and YouTube. The aim is to understand how users discussed the topic, how communities formed around the discussion, and how sentiment, emotion, topic framing, and homophily appeared across the two platforms.

The project combines network analysis and NLP-based text analysis. Bluesky was mainly used for network and community analysis, while YouTube was used to compare a more broadcast-based platform through comments, engagement, sentiment, and keyword framing.

## Project Structure

```text
UGGroup11_SocialMedia_A2/
│
├── Data/
│   ├── Bluesky_dataset_UG11.csv
│   ├── bluesky_user_sentiment.csv
│   ├── hanta_posts_with_community.csv
│   ├── hantavirus_youtube_data.json
│   ├── youtube_comments_final_analysis.csv
│   └── youtube_videos_final_analysis.csv
│
├── Graphs/
│   ├── HV_full_enriched.graphml
│   ├── HV_sentiment_graph.graphml
│   ├── UG11_Network_Graph.graphml
│   ├── UG11_communities.graphml
│   └── modUG11_Network_Graph.graphml
│
├── images/
│   ├── engagement_binned.png
│   ├── engagement_vs_sentiment.png
│   ├── keyword_framing.png
│   ├── keyword_framing_refined.png
│   ├── network_by_community.png
│   ├── network_by_sentiment.png
│   ├── network_by_topic.png
│   ├── nrc_emotion_comparison.png
│   └── polarisation_comparison.png
│
├── UG11_Networks_Analysis.ipynb
├── UG11_Sentiment_Analysis.ipynb
├── UG11_Homophily_Analysis.ipynb
└── UG11_Youtube_Analysis.ipynb
```

## Notebook Overview

### `UG11_Networks_Analysis.ipynb`

This notebook focuses on the Bluesky network analysis. It builds and analyses the reply/post network, calculates network measures, detects communities, and exports graph files for further analysis and visualisation.

**Main outputs include:**

- Network graph files
- Community detection results
- Centrality measures
- Network-level statistics

### `UG11_Sentiment_Analysis.ipynb`

This notebook analyses sentiment in the Bluesky dataset. It links sentiment scores with users, posts, and network/community structures to understand how positive, neutral, and negative discussion appeared across the dataset.

**Main outputs include:**

- Sentiment-enriched data
- Sentiment graph files
- Sentiment-based comparisons across communities

### `UG11_Homophily_Analysis.ipynb`

This notebook examines whether users with similar characteristics or views tend to interact within the same communities. It supports the discussion of homophily, polarisation, and whether communities show similar or mixed sentiment/topic patterns.

**Main outputs include:**

- Homophily-related analysis
- Community comparison results
- Supporting visualisations for polarisation and topic grouping

### `UG11_Youtube_Analysis.ipynb`

This notebook analyses YouTube videos and comments related to hantavirus. It focuses on sentiment, engagement, emotion, and keyword framing to compare YouTube discussion with the Bluesky network.

**Main outputs include:**

- Cleaned YouTube video and comment datasets
- Engagement and sentiment analysis
- Emotion comparison
- Keyword framing visualisations

## Data

The `Data/` folder contains the cleaned and processed datasets used across the notebooks.

- `Bluesky_dataset_UG11.csv` contains the main Bluesky dataset.
- `bluesky_user_sentiment.csv` contains user-level sentiment results.
- `hanta_posts_with_community.csv` contains Bluesky posts with assigned community information.
- `hantavirus_youtube_data.json` contains the collected YouTube data.
- `youtube_comments_final_analysis.csv` contains processed YouTube comment analysis data.
- `youtube_videos_final_analysis.csv` contains processed YouTube video-level analysis data.

## Graph Files

The `Graphs/` folder stores GraphML files created during the network analysis.

These files are used to preserve the network structure, centrality scores, sentiment attributes, and community detection results. They can also be opened in network visualisation tools such as Gephi.

## Images

The `images/` folder contains exported figures used for analysis and reporting.

These include visualisations for:

- Engagement and sentiment
- Keyword framing
- Emotion comparison
- Network communities
- Network sentiment
- Network topics
- Polarisation comparison

## Requirements

Each notebook includes its own import and library setup section. Before running the analysis, run the import/setup cells at the top of each notebook.

Common libraries used in this project may include:

- pandas
- numpy
- matplotlib
- seaborn
- networkx
- nltk
- scikit-learn
- community detection libraries
- sentiment and text analysis libraries

## How to Run

1. Open the project folder in Jupyter Notebook or JupyterLab.
2. Keep the `Data/`, `Graphs/`, and `images/` folders in the same directory as the notebooks.
3. Open each notebook and run the import/setup cells first.
4. Run the notebooks in this suggested order:

   1. `UG11_Networks_Analysis.ipynb`
   2. `UG11_Sentiment_Analysis.ipynb`
   3. `UG11_Homophily_Analysis.ipynb`
   4. `UG11_Youtube_Analysis.ipynb`

This order is recommended because the network and sentiment notebooks generate outputs that may be used in the later homophily and comparison analysis.

## Project Aim

The main aim of this project is to examine how hantavirus-related information spread and was discussed across different online platforms. The analysis compares Bluesky as a decentralised social media platform with YouTube as a more broadcast-style platform.

The project investigates:

- Which users or groups were central in the Bluesky discussion
- How communities formed around the topic
- Whether sentiment and topic patterns differed across communities
- Whether homophily or polarisation appeared in the network
- How YouTube discussion compared with Bluesky discussion
- How engagement, emotion, and keyword framing shaped the overall conversation

## Notes

This project was completed for Social Media and Network Analytics Assignment 2 by UGGroup11. The notebooks, datasets, graph files, and images are organised to support reproducibility and make it easier to follow the full analysis workflow.
