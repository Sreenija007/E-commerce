## Dataset
Using the **Amazon Electronics Rating Dataset**, where each product and user is uniquely identified to avoid bias.  
📌 [Dataset Link](https://www.kaggle.com/datasets/vibivij/amazon-electronics-rating-datasetrecommendation/download?datasetVersionNumber=1)

## Approach

### 1️⃣ Rank-Based Product Recommendation
**🔹 Goal:** Recommend products with the highest ratings to new users (**solves Cold Start Problem**).  
**🔹 Method:**
   - Compute the average rating and total interactions for each product.
   - Sort products by ratings and recommend the **top N products**.

### 2️⃣ Similarity-Based Collaborative Filtering
**🔹 Goal:** Suggest products based on similar user interactions.  
**🔹 Method:**
   - Convert user IDs into numerical values.
   - Compute **cosine similarity** between users.
   - Recommend products highly rated by **similar users** but not yet interacted with by the target user.

### 3️⃣ Model-Based Collaborative Filtering
**🔹 Goal:** Predict personalized recommendations using **Singular Value Decomposition (SVD)**.  
**🔹 Method:**
   - Convert the user-product interaction matrix into a **CSR matrix** for efficiency.
   - Perform **SVD** to reduce dimensionality and extract latent features.
   - Predict ratings for all users and recommend **top N products** based on predictions.
   - **Evaluate model** using **RMSE (Root Mean Squared Error)**.

🚀 **This project is for learning purposes and demonstrates the workings of recommendation systems.**
