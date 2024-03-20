# Topic-Modeling-Surfing-Videos-on-YouTube
In this repo is part of a broader project to understand what makes a YouTube Channel (or video) perform well. In this series of notebooks, I use different approaches to Topic Modeling to support my EDA efforts. 

#### Data ####
* YouTube video titles from Surfing channels
* The Surfing Chanels comprise of content posted by training companies, main Surf brands as well as that by Pro Surfers.
* 8821 videos
* The average YouTube Video title is 5.21 words long
* Kudos to 'How to Rip', 'Nathan Florence', 'Nic Von Rupp', 'Barefoot Surf','Kai Lenny', 'Surf Strength Coach', 'Ombe Surf', 'Rip Curl', 'Surfline', 'Red Bull Surfing', 'Kale Brock' for the inspiration and wonderful content.

<img width="800" alt="Surfer" src="https://github.com/daphteh/Topic-Modeling-Surfing-Videos-on-YouTube/blob/dae5708a66e3962b59eeaf888e4d29043d8aa330/Report_Images/Nathan_Florence.jpeg">
</details>

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
<img width="1274" alt="Words clusters from LDA" src="https://github.com/daphteh/Topic-Modeling-Surfing-Videos-on-YouTube/blob/6b454af344c37da62d04f4d0c87826b34b7b2a0c/Report_Images/LDA_Topics_Words.jpg">
</details>


<details>
<summary> Step 2b: Topic Modeling - GSMM</summary>
  <br>
  <p>   Cleaning data </p>
  <p>   Refining my approach to Topic Modeling using techniques geared towards short text</p>
      <img width="1274" alt="Word clusters from GSMM" src="https://github.com/daphteh/Topic-Modeling-Surfing-Videos-on-YouTube/blob/6b454af344c37da62d04f4d0c87826b34b7b2a0c/Report_Images/GSMM_Topics_Words.jpg">
</details>

<details>
<summary> Step 2c: Topic Modeling - BERTTopic</summary>  
 <br>
 <p>   No cleaning necessary</p>
 <p>   Applied BERTTopic</p>
</details>

# Final Results
The number of topics in the corpus vary based on technique.
LDA: 28 topics
GSMM: 6 topics
BERTtopic: 236 topics

<img width="1274" alt="Topic Map from BERTopic" src="https://github.com/daphteh/Topic-Modeling-Surfing-Videos-on-YouTube/blob/e0e676c160b19d3a8bece38ec2c843f50317ef3e/Report_Images/BERTTopic_Map.jpeg">


I personally found GSMM the best in terms of simplifying the categorization process. Nonetheless, mapping the categories onto the individual titles showed a significant amount of descrepancy. BERTopic created far too many topics, but they were relatively meaningful when I checked the results against each title. It was also useful that the is functionality to show how these topics build on each other. BERTopic can be improved by removing words like ['surf', 'surfer', surfing'].
