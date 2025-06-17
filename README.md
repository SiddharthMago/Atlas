# 🌍 A-T-L-A-S: Graph Theory Meets the Game of Geography

> "India" ➜ "Australia" ➜ "Austria" ➜ "Albania"... can you trap your opponent using the power of graph theory?

This project reimagines the classic word game **ATLAS** as a directed graph problem. We explore how concepts from **graph theory**, **community detection**, and **machine learning** can provide strategies and predictive insight into the game using real-world datasets of countries and cities.

<br>

## 📘 Project Summary

- Constructed 3 ATLAS-style graphs:
  1. Country Only
  2. City Only (top 500 by population)
  3. Country + City Combined
- Analyzed key properties using NetworkX to uncover gameplay strategies
- Performed **community detection** using Louvain and Girvan–Newman algorithms
- Built a **link prediction model** using Node2Vec and GNNs to anticipate valid transitions
- Created visualizations and strategic insights based on node connectivity

<br>

## 🗂️ File Overview

| File | Description |
|------|-------------|
| `atlas.ipynb` | Main notebook with graph creation, EDA, and strategy logic |
| `observations.ipynb` | Visualizations and exploratory insights |
| `AtlasBONUS.ipynb` | BONUS: Link prediction with Node2Vec & GNN |
| `observations.pptx` | Strategic insights in presentation format |
| `precog.pptx` | Final presentation for submission |

<br>

## ▶️ How to Run

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Open each notebook in Jupyter or Colab:
   - Run the first code cell  
   - Restart the kernel  
   - Run all cells again  
3. `AtlasBONUS.ipynb` was developed on **Colab**; others were built locally.  
4. Some interactive graphs are exported as `.html` and should be opened using **Live Server** in VSCode or a local browser.

<br>

## 📈 Graph Analysis & Strategy

We used 6 graph theory concepts to extract insights from gameplay:

- Degree & Out-degree centrality  
- PageRank  
- Strongly Connected Components  
- Diameter & Density  
- Terminal nodes (Dead Ends)  
- Clustering coefficient  

These were evaluated across all 3 graphs to understand how the game evolves with dataset complexity.

<br>

## 🔎 Community Detection

- **Algorithms**: Louvain, Girvan–Newman  
- **Evaluated via**: Modularity score  
- Communities showed alignment with geographic and linguistic groupings  
- **Strategic insight**: Jumping across communities can isolate opponents

<br>

## 🤖 BONUS: Link Prediction

| **Aspect**   | **Approach**                                           |
|--------------|--------------------------------------------------------|
| Model        | Node2Vec embeddings + Logistic Regression              |
| Optional     | Graph Neural Network via PyTorch Geometric             |
| Features     | Start & end characters, character embeddings           |
| Training     | Unsupervised on masked edges                           |
| Objective    | Predict future transitions in gameplay                 |

<br>

## 📂 Dataset Sources
- **Countries**: [Britannica – List of Countries](https://www.britannica.com/topic/list-of-countries-1993160)
- **Cities**: [World Population Review](https://worldpopulationreview.com/cities)

<br>

## 📚 Resources & References

### Graph Theory
- Professor Foote – Intro to NetworkX ([YouTube](https://youtu.be/flwcAf1_1RU?si=LdETHzpgO6Ijo4dX))
- Wikipedia – [Graph Centrality](https://en.wikipedia.org/wiki/Centrality)
- Wikipedia – [Graph Properties](https://en.wikipedia.org/wiki/Graph_property)

### Community Detection
- [Community Detection Algorithms (Medium)](https://medium.com/towards-data-science/community-detection-algorithms-9bd8951e7dae)
- [Stanford CS224W – ML with Graphs](https://www.youtube.com/playlist?list=PLoROMvodv4rPLKxIpqhjhPgdQy7imNkDn)
- [From Louvain to Leiden – Scientific Reports](https://www.nature.com/articles/s41598-019-41695-z)
- YouTube – [Louvain](https://www.youtube.com/watch?v=akfiGPBtCuM), [Girvan-Newman](https://www.youtube.com/watch?v=2KHfVp8HN_g), [Modularity](https://www.youtube.com/watch?v=0zuiLBOIcsw)

### Link Prediction
- [StellarGraph Node2Vec Tutorial](https://stellargraph.readthedocs.io/en/stable/demos/link-prediction/node2vec-link-prediction.html)
- [Kaggle: Node2Vec + ML](https://www.kaggle.com/code/adilimadeddinehosni/link-prediction-node2vec-and-machine-learning)
- [MovieLens GNN Notebook (Colab)](https://colab.research.google.com/drive/1xpzn1Nvai1ygd_P5Yambc_oe4VBPK_ZT?usp=sharing)

### Inspiration
- [I Made a Graph of Wikipedia…](https://www.youtube.com/watch?v=JheGL6uSF-4&t=117s)

<br>

## 🛠 Tools & Libraries
- Python 3.x
- `networkx`, `matplotlib`, `plotly`, `pandas`, `numpy`
- `community` (Louvain method)
- `scikit-learn`, `gensim`
- `PyTorch`, `PyTorch Geometric`
- `StellarGraph`

<br>

## 🙌 External Support

This project utilized **ChatGPT** to:
- Refine grammar and clarity in written explanations
- Debug syntactic errors in code
- Suggest modeling changes in GNN training
- Maintain library compatibility and resolve import issues

<br>

## 👨‍💻 Authors

Developed by **Siddharth Mago**
Part of a research-focused study on Graph Algorithms and Machine Learning

---