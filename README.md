![Header](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,4,6&height=200&section=header&text=📊%20Nike%20Page%20SNA&fontSize=42&fontColor=fff&animation=fadeIn&fontAlignY=35&desc=Social%20Network%20Analysis%20on%20Nike's%20Facebook%20Page%20using%20Gephi&descAlignY=55&descSize=15)

[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![Gephi](https://img.shields.io/badge/Gephi-9452CE?style=for-the-badge&logo=gephi&logoColor=white)](https://gephi.org)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)

> *Uncovering the hidden social structure inside one of the world's most followed brand pages.*

---

## 📌 Overview

This project applies **Social Network Analysis (SNA)** to Nike's official Facebook page to understand how users interact, who the key influencers are, and what the community structure looks like at scale.

Using the **Netvizz** data extraction tool and **Gephi** for visualization and analysis, the network reveals clusters, bridges, and high-influence nodes hidden within thousands of user interactions.

---

## 🔍 What is Social Network Analysis?

Social Network Analysis maps relationships between entities (people, pages, accounts) as a graph:

- **Nodes** = users / entities
- **Edges** = interactions (comments, replies, tags)
- **Metrics** = centrality, clustering, density

It's used in sociology, marketing, epidemiology, and increasingly in product analytics.

---

## 🌐 The Network

| Property | Value |
|---|---|
| Source | Nike Official Facebook Page |
| Data Tool | Netvizz |
| Graph Type | Undirected (mutual interactions) |
| Visualization | Gephi |
| Analysis | Centrality, Community Detection, Clustering |

---

## 📐 Key Metrics Analyzed

### Centrality Measures

- **Degree Centrality** — Who has the most direct connections?
- **Betweenness Centrality** — Who acts as a bridge between communities?
- **Closeness Centrality** — Who can reach others most efficiently?

### Community Structure

- **Modularity** — How strongly clustered is the network?
- **Connected Components** — How many isolated sub-networks exist?
- **Average Path Length** — How many hops between any two users on average?

---

## 🔑 Key Findings

- The network exhibits **scale-free properties** — a small number of "superfan" accounts account for a disproportionate share of engagement
- Clear **community clusters** formed around product categories (Jordan, running, football)
- High betweenness centrality nodes are often **brand advocates**, not Nike's official accounts
- The average path length is short (~3.2 hops), suggesting a **small-world network** structure
- Community detection revealed **6 major clusters** of engagement behavior

---

## 🛠️ Tools and Methodology

```
Data Collection → Netvizz (Facebook Graph API export)
        ↓
Network Parsing → Python (NetworkX for preprocessing)
        ↓
Visualization → Gephi (ForceAtlas2 layout)
        ↓
Analysis → Gephi Statistics Panel + Python
        ↓
Export → HTML visualization for sharing
```

---

## 🚀 Getting Started

### Prerequisites

- [Gephi](https://gephi.org/users/download/) 0.9+
- Python 3 with `networkx`, `pandas`

### Run

```bash
git clone https://github.com/shreyneil/Nike_page_sna.git
cd Nike_page_sna

# Open the .gexf or .csv network file in Gephi
# Or open index.html in a browser for the interactive visualization
```

---

## 📁 Project Structure

```
Nike_page_sna/
├── index.html              # Interactive network visualization
├── network_data/           # Raw exported network files (.gexf / .csv)
├── gephi_project/          # Gephi project file with layouts saved
├── analysis/               # Metric outputs and charts
└── README.md
```

---

## 💡 Applications

This type of analysis has real-world applications in:

- **Brand marketing** — identify superfans and organic amplifiers
- **Community management** — find bridge users to reduce fragmentation
- **Influencer campaigns** — target high-betweenness nodes for max reach
- **Crisis comms** — understand how information (or misinformation) spreads

---

## 👨‍💻 Author

**Shreyash Sharma** — PM2 @ ThoughtSpot · Data and network enthusiast

- [GitHub](https://github.com/shreyneil)
- [LinkedIn](https://www.linkedin.com/in/shreyash-sharma-b19918117/)

---

*Interested in network analysis or brand community research? Let's connect!*

![Footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,4,6&height=100&section=footer)
