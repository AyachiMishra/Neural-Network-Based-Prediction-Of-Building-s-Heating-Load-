##  Dataset Description: Energy Efficiency Dataset

### Data Source
The dataset used in this project is the **Energy Efficiency Dataset** obtained from the  
**UCI Machine Learning Repository**.

- **UCI Dataset ID:** 242  
- **Dataset Name:** Energy Efficiency  
- **Repository Link:** https://archive.ics.uci.edu/dataset/242/energy+efficiency  
- **Data File:** https://archive.ics.uci.edu/static/public/242/data.csv  
- **Creators:** Athanasios Tsanas, Angeliki Xifara  
- **Year:** 2012  
- **DOI:** 10.24432/C51307  



---

###  Dataset Overview
- **Number of instances:** 768 simulated buildings  
- **Number of features:** 8 building parameters  
- **Target variables:**  
  - **Y1:** Heating Load  
  - **Y2:** Cooling Load  
- **Feature types:** Continuous and Integer  
- **Missing values:** None  

The dataset is **multivariate** and is suitable for **machine learning analysis**, which is the focus of this project.

---

###  Problem Context

In this project, we focus on predicting **Heating Load (Y1)** using machine learning models.

---

###  Detailed Feature Description

The dataset consists of eight building design parameters that describe the **geometry, size, orientation, and glazing properties** of residential buildings.  
These features directly influence how heat is gained or lost through the building envelope, thereby affecting the heating load.

> **Note:** All geometrical features are derived from simulated building models using Ecotect and are expressed in consistent units across the dataset.

---

| Feature | Name | Unit / Type | Why It Matters for Heating Load |
|--------|------|-------------|---------------------------------|
| **X1** | Relative Compactness | Dimensionless (ratio) | Measures how compact the building shape is. More compact buildings have less exposed surface area per unit volume, leading to lower heat loss and reduced heating load. |
| **X2** | Surface Area | m² | Represents the total external area through which heat can be exchanged with the environment. Larger surface area generally increases heat loss, raising heating demand. |
| **X3** | Wall Area | m² | Walls are major contributors to conductive heat loss. Higher wall area increases exposure to external temperatures, increasing heating requirements. |
| **X4** | Roof Area | m² | Roofs experience significant heat loss due to rising warm air and solar exposure. Larger roof areas can substantially increase heating load, especially in colder conditions. |
| **X5** | Overall Height | m | Indicates building volume and vertical exposure. Taller buildings often have greater heat loss due to increased air volume and wall area, resulting in higher heating load. |
| **X6** | Orientation | Categorical (Integer) | Determines how the building is positioned relative to the sun. Orientation affects solar heat gains, but its impact is typically secondary compared to geometry and size. |
| **X7** | Glazing Area | Ratio (0–0.4) | Represents the proportion of the building covered by windows. Windows have higher heat transfer than walls, so increased glazing generally raises heating load. |
| **X8** | Glazing Area Distribution | Categorical (Integer) | Describes how windows are distributed across building facades. Distribution influences solar gains and directional heat loss, but its effect is often subtle compared to glazing size. |

---
#### Some clarifications
The glazing area is expressed as a dimensionless ratio and is discretized between 0 and 0.4 to represent realistic residential window coverage.

### Target Variables

| Target | Name | Unit | Meaning |
|-------|------|------|---------|
| **Y1** | Heating Load | kWh/m² | Energy required to maintain indoor thermal comfort during cold conditions |
| **Y2** | Cooling Load | kWh/m² | Energy required to remove heat during warm conditions |

---

### Summary
The features collectively describe how **building shape, size, height, and window characteristics** influence thermal performance.  
This makes the dataset especially suitable for studying **linear vs nonlinear relationships** in energy efficiency modeling.



---

### Interpretation of the Metadata Table
The metadata table provides important contextual information about the dataset:

- **Tasks:** The dataset supports both **Regression** and **Classification** (classification if targets are discretized).
- **Characteristics:** Multivariate dataset with mixed feature types.
- **Simulation-Based:** All 768 samples correspond to different simulated building configurations.
- **Purpose:** To quantitatively estimate building energy performance using statistical and machine learning methods.

This makes the dataset well-suited for comparing **linear and nonlinear regression models** and analyzing how building design choices influence energy efficiency.

---

### Why This Dataset Is Appropriate
- Clean dataset with **no missing values**
- Realistic, simulation-based architectural data
- Clear physical interpretation of features
- Ideal for demonstrating **model comparison and feature analysis**

This dataset provides a strong foundation for understanding how architectural parameters influence energy consumption in buildings.
