**Mars Rover Terrain Navigation with Explainable AI**
This project leverages optical flow-based terrain analysis and A path planning* with Explainable AI (XAI) to enable safe and interpretable navigation for Mars rovers. Using the Mars Surface and Curiosity Image Set NASA dataset, the system identifies rough terrain, computes a cost map, and plans an optimal path while providing explanations for each decision.



**Project Highlights**
**Dataset:** Mars Surface and Curiosity Image Set NASA, imported from Kaggle.
**Algorithms Used:**
Optical Flow (Farneback) for terrain analysis.
A* Path Planning for safe navigation.
Explainable AI techniques using SHAP and decision traces to enhance interpretability.


**Goals:**
Enable autonomous, efficient, and safe navigation on challenging Martian terrain.
Provide interpretability for terrain assessment and path-planning decisions.


**Implementation Steps**
**Dataset Loading:** Imported the dataset directly from Kaggle using kagglehub.
**Optical Flow Analysi**s: Calculated optical flow between image pairs to assess terrain roughness.
**Cost Map Generation:** Used optical flow magnitudes to create a cost map, assigning higher costs to rough or obstacle-laden areas.
**Explain Cost Map with SHAP:** Explained terrain classification by applying SHAP, showing feature contributions to traversal difficulty.
**Path Planning with A star:** Calculated the safest, most efficient path across the cost map, avoiding high-cost regions.
**Decision Trace:** Recorded decision explanations for each step in the path, detailing factors like cell cost and distance to the goal.
**Visualization and Counterfactual Analysis:** Displayed the planned path on the cost map and explored alternative routes with slight cost adjustments.



**Results**
The final output includes:

A visualization of the optimal path that avoids hazardous areas.
Explanations for terrain classification (using SHAP) and path-planning decisions (decision trace), enhancing the transparency of the navigation system.
Dataset
Name: Mars Surface and Curiosity Image Set NASA
Source: Kaggle Dataset Link
Project Objectives
Safe Navigation: Avoid hazardous terrain by identifying rough areas.
Efficient Path Planning: Use A* algorithm to optimize the path across the terrain.
Explainable AI: Provide interpretability using SHAP and decision traces, promoting trust in rover navigation.
