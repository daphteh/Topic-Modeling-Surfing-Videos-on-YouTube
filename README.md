# Topic-Modeling-Surfing-Videos-on-YouTube
In this repo is part of a broader project to understand what makes a YouTube Channel (or video) perform well. In this series of notebooks, I use different approaches to Topic Modeling to support my EDA efforts. 
These 

#### Methods Used ####
* Data preprocessing - stemming, stopwords removal, white space removal and etc.
* Topic Modeling: LDA, GSMM, BertTopic

# Methodology

<details>
<summary> Step 0 and 1: Scrape, process and clean the data </summary>
      <br>
      <p>   Develop a baseline understanding of how each of these Chanels behave</p>
      <p>   Clean up features (esp those related to DateTime)</p>
</details>

<details>   
<summary> Step 2a: Topic Modeling - LDA</summary>  
  <br>
  <p>   Clean data, create bigrams and BOW</p>
  <p>   Identify the ideal number of clusters</p>
  <p>   Look at words associated with each cluster to discern what they mean</p>
</details>

<details>
<summary> Step 2b: Topic Modeling - GSMM</summary>
  <br>
  <p>   Cleaning data </p>
  <p>   Refining my approach to Topic Modeling using techniques geared towards short text</p>
<img width="1274" alt="Elbow_Number_Clusters" src="https://github.com/daphteh/Customer_Segmentation_CreditCard_Company/blob/e0989a2d6516a2678311a63c9c3a04dcb983fdb5/Report_Images/Elbow_Number_Clusters.png">
</details>

<details>
<summary> Step 2c: Topic Modeling - BERTTopic</summary>  
 <br>
 <p>   No cleaning necessary</p>
 <p>   Applied BERTTopic</p>
<img width="1274" alt="Customer_Segments_Clusters" src="https://user-images.githubusercontent.com/116262236/213372327-3844e2c7-f67c-4995-9276-561e32ba8bba.png">
</details>

# Final Results
<img width="1274" alt="Summary_n_Recommendations" src="https://github.com/daphteh/Customer_Segmentation_CreditCard_Company/blob/77896663197562f725b460b6a4e34dc077fd63e8/Report_Images/Summary_n_Recommendations.png">
