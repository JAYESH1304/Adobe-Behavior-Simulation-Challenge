# Adobe-Behavior-Simulation-Challenge

## Overview
The problem statement is based on the fundamental process of communication in marketing, focusing on behavior simulation (Task-1) and content simulation (Task-2) to assist marketers in estimating and enhancing user engagement on social media platforms. The team aims to provide solutions for simulating user behavior and creating content that effectively elicits the desired KPIs, offering valuable insights for optimizing social media strategies.

## Objective
Companies often rely heavily on leveraging the power of social media platforms such as Twitter, Instagram, Facebook, etc. to promote their products, boost sales, and build a brand identity. Thus, it is important for companies to optimize their posts to maximize user interaction and ensure efficiency in their campaigns.
User engagement on Twitter is quantified by metrics like user likes, retweets, comments, mentions, follows, clicks on embedded media and links. For this challenge, we consider the number of likes to be our KPI for user engagement. The given problem statement consists of the following two tasks:

• Task 1: Given the content of a tweet, the task is to predict its user engagement, measured by likes.

• Task 2: Given the tweet metadata, generate the tweet text.

The team has leveraged the latest advancements in Deep Learning and Generative AI to tackle the above two tasks.

## How to Run

### Task 1: Predicting Number of Likes (Behavior Simulation)
1. **Media Caption Generation**:
   - Utilize BLIP-2 for generating captions for media content, including Images, Videos, and GIF thumbnails.
2. **Data Preparation**:
   - Integrate these captions with tweet metadata (text, company, username, timestamp) from dataset.
   - Create an Instruction dataset, combining all data as a single prompt for inference.
3. **Classification and Regression**:
   - Employ DistilBERT for predicting engagement levels (like ranges or Buckets) based on the combined prompt.
   - Implement regression models within the predicted engagement bucket to estimate the specific number of likes for each tweet.

     
### Task 2: Content Generation (Content Simulation)
1. **Media Caption Generation**:
   - Utilizing BLIP-2 to generate captions for various media types such as Images, Videos, and GIF thumbnails.
2. **Text Extraction from Media**:
   - Employing PaddleOCR for extracting text present on Images or Video thumbnails, enhancing content contextualization.
3. **Data Preparation**:
   - Merging generated captions and extracted text with tweet metadata (including company name, username, and timestamp) from our dataset.
   - Creating an Instruction dataset where all data components are used as a single prompt during the inference process.
4. **Text Generation**:
   - Feeding the compiled prompt to our fine-tuned Llama2 model to produce the final text content for tweets.

### Config files of Fine-tuned Llama2 ---> https://drive.google.com/file/d/1ly94C5o7iPq5qwzF7FVECfE283V2Qwk/view?usp=sharing
## Results
### Task 1


### Task 2:

