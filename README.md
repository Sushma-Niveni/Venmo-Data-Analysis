
## Venmo Data Analysis 



### **Introduction**
- **Objective**: Analyze Venmo transaction data to uncover spending behaviors, social network metrics, and predictive features.
- **Scope**: Utilize Spark for data processing, Python/R for visualization, and explore advanced techniques like GNN.

### **Text Analytics **
1. **Dictionary Expansion**:
   - **Task**: Identify and add 10 new words to the existing text dictionary that are not already included.
   - **Method**: Open the Venmo app, examine transactions, and ensure no duplicates before adding.

2. **Classification of Transactions**:
   - **Emoji Analysis**: Classify transactions by emoji and text using the provided dictionaries. 
   - **Metrics**: Calculate the percentage of transactions with only emojis, identify the top 5 emojis and top 3 emoji categories.

3. **User Spending Profiles**:
   - **Static Profile**: For each user, categorize their transactions and compute their spending profile based on categories (e.g., food, activity).

4. **Dynamic Spending Profiles**:
   - **Task**: Analyze and plot how spending profiles evolve monthly from the user's first transaction up to 12 months.
   - **Method**: Use window functions to track changes over time and visualize average spending profiles with confidence intervals.

### **Social Network Analytics **
1. **Friendship Discovery**:
   - **Task**: Develop a script to identify a user's friends and friends of friends based on transaction interactions.
   - **Complexity**: Describe the algorithm used and its computational complexity.

2. **Social Network Metrics**:
   - **Metrics**: Calculate and analyze:
     - Number of friends and friends of friends.
     - Clustering coefficient of each user’s network.
     - PageRank of each user, utilizing efficient methods for large-scale graphs.

### **Predictive Analytics with MLlib **
1. **Dependent Variable Creation**:
   - **Task**: Define `Y` as the total number of transactions a user made by the end of their first year.

2. **Recency and Frequency Metrics**:
   - **Task**: Compute recency and frequency metrics for each user.
   - **Method**: Define recency as the time since last activity and frequency as the number of transactions per month.

3. **Regression Analysis**:
   - **Models**:
     - **Recency and Frequency**: Perform regression and plot Mean Squared Error (MSE) for predictions over time.
     - **Spending Behavior Profiles**: Include spending behavior in regression and compare MSE.
     - **Social Network Metrics**: Integrate social network metrics in regression models and plot MSE.
     - **Social Network Spending Behavior**: Assess the impact of social network spending behavior on predictions and compare MSE.

### **Graph Neural Network (GNN) Analysis**
1. **Graph Preparation**:
   - **Task**: Transform Venmo transaction data into a graph format with users as nodes and transactions as edges.

2. **GNN Model Implementation**:
   - **Task**: Implement a GNN model to learn user representations. Include features such as emoji/text metrics.
   - **Framework**: Utilize PyTorch Geometric or DGL.

3. **Comparative Analysis**:
   - **Tasks**:
     - Compare GNN performance with manual feature engineering in terms of efficiency and predictive accuracy.
     - Analyze differences in feature importance between GNN and manually engineered features.
     - Reflect on insights gained from using GNN for Venmo data analysis.
    
   ***CUT SHORT***
   **Text Analytics: Analyzing transaction messages and spending profiles.
Social Network Analytics: Exploring user connections and network metrics.
Predictive Modeling: Forecasting transaction counts and user behavior.
Graph Neural Networks (GNN): Applying advanced methods to analyze network data.**
