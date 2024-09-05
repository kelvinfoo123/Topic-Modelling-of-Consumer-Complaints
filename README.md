# Topic-Modelling-of-Consumer-Complaints
### **Introduction**
This project aimed to use topic modelling to determine the nature of consumer complaints received.

### **Methodology**
- Upon cleaning the complaint text (ie. making text lowercase, removing punctuation and removing words containing numbers), Tf-idf vectorizer was used to pre-process the text. Based on the below image, a minimum document frequency of 4 was used for Tf-idf vectorizer since as minimum document frequency increases beyond 4, the rate of decrease in number of features become smaller.
![Screenshot 2024-09-05 at 12 54 21](https://github.com/user-attachments/assets/589e7d0f-f2f6-4d06-9fc3-962f57a2b097)
- We experimented with K-Means and latent dirichlet allocation for topic modelling. We were unable to determine an optimal number of clusters for K-Means using sum of squared errors and silhouette score.
- We experimented with having 2-4 topics for latent dirichlet allocation. For results with 3 topics, there was an overlap in the three topics such that they contain complaints related to fraud. For results with 4 topics, topic 0 and topic 4 overlapped such that they contained complaints about identity theft. Hence, the optimal number of topics was set to be 2. Topic 0 contained complaints on fraud and identity theft while topic 1 contained complaints on late payment or incorrect payment status.

### **Results & Analysis**
- There were 1948 complaints related to fraud and identity theft and 3052 complaints related to late payment and incorrect payment status.
![Screenshot 2024-09-05 at 12 58 50](https://github.com/user-attachments/assets/d717098f-356c-4f1b-b82a-c7c0b8248ade)
