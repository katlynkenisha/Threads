# Exploring User Reviews of Threads App through Topic Modeling
![threads](https://github.com/katlynkenisha/Threads/assets/109913754/06bc31f7-1821-4c56-bea7-ec6c6243dc5b)

## Introduction
In today’s fast-paced world where trends can shift rapidly, understanding customer sentiments is crucial for creating successful and marketable products. However, gaining insights can become a time-consuming and challenging task, especially with a large customer base. Not to worry, Natural Language Processing (NLP) techniques provide a promising solution to tackle this issue.

This research aims to analyze user reviews of Threads, a text-based application recently developed by Instagram, in order to assess its position in the social media market. Key themes discussed by users were extracted using topic modeling through Non-Negative Matrix Factorization (NMF). These results were visualized using word clouds to highlight the strengths, weaknesses, problems, and suggestions from users' perspectives.

## Methodology
### 1. Data Collection
The dataset consists of approximately 32000 user reviews from July 2023, collected through web scraping. The dataset is accessible on Kaggle (https://www.kaggle.com/datasets/saloni1712/threads-an-instagram-app-reviews).
The variables obtained include:
- **Source**: The platform on which reviews were submitted, specifically Google Play or App Store.
- **Review**: Comments provided by users.
- **Rating**: Number of stars users scored the app.
- **Review Date**: The date when users submitted their reviews.

### 2. Data Cleaning & Preparation
The data cleaning and preparation process was carried out separately for each variable.

#### Review
The data cleaning and preparation process for the “Review” variable involves; converting words into lowercase, correcting typos and errors, tokenizing sentences into individual words, removing non-alphabet characters, eliminating extra spaces, removing stopwords, lemmatizing words into their base forms, and substituting specific words with their most commonly used synonym in the context of app reviews.

#### Rating
The data cleaning and preparation process for the “Rating” variable involves categorizing ratings into different classes such as; negative (1-2 stars), neutral (3 stars), and positive (4-5 stars).

#### Review Date
The data cleaning and preparation process for the “Review Date” variable involves removing the time component from the review date as it is irrelevant in this context.

### 3. Data Exploration
Some of the key findings from the data exploration process include:

![threads](https://github.com/katlynkenisha/Threads/assets/109913754/fb1e68f7-f206-46ea-965f-2c10035ab920)
- Majority of Threads users were Android-based.

![threads](https://github.com/katlynkenisha/Threads/assets/109913754/70fb23dd-8a83-421c-83ff-9efbd5a75472)
- Threads received a significant number of extreme ratings, either 1 or 5 stars, indicating that users’ sentiments were polarized towards extreme satisfaction or dissatisfaction with the app.

![threads](https://github.com/katlynkenisha/Threads/assets/109913754/d70f6bad-6d9d-40e9-bede-7a73da28e52b)
- Threads’ ratings experienced a declining trend over time.

![threads](https://github.com/katlynkenisha/Threads/assets/109913754/dda29232-b636-46dd-ae9a-78b06e128812)
- Android users tend to have a better experience in comparison to IOS users.

### 4. Topic Modeling 
Topic modeling using Non-Negative Matrix Factorization (NMF) was applied to analyze general themes of user opinions based on reviews which have been categorized into positive, neutral, and negative based on their corresponding ratings.

#### Positive
- Smooth app performance.
- Impressive and clean user interface.
- Stands out as the best app among other social media platforms.

#### Neutral
- Good start, although perceived as an “okay” application.
- Users encountered issues such as seeing posts from accounts they were not following.
- Similar to Twitter.

#### Negative
- Users perceived the app as a mere imitation of Twitter with lack of innovation.
- Users were facing account synchronization issues with Instagram.
- Inability to delete account.
- Negative user experience.
- Poor user interface.
- Users had privacy concerns.
- Various occurrences of bugs, glitches, and crashes.
- Users found the app to be unproductive and uninteresting.

### 5. Identifying Problems Faced by Users
Based on the numerous complaints outlined by users as seen from the negative reviews, further analysis was carried out to determine the proportion of users experiencing different types of challenges. These challenges were defined based on common issues faced by users when using apps in general, such as:
- **Technical**: Bugs, glitches, freezes, crashes, lags
- **Compatibility**: Screen size, device, user interface
- **Account**: Sign up, login, password recovery

![threads](https://github.com/katlynkenisha/Threads/assets/109913754/afaf0f8e-d2a5-4c48-8d18-56f37218d966)
Threads’ main problem centers on its technical performance, with roughly 11% of users encountering issues in this aspect.

### 5. Identifying Suggestions from Users
User suggestions were analyzed using the same approach of topic modeling via Non-Negative Matrix Factorization (NMF). However, additional keywords such as “add” and “feature” were incorporated as these terms would possibly signify a suggestion that a user has made. Overall, suggestions from users can be summarized into:

1. **Enhancing posts recommendations**: A significant number of users voiced their concern on encountering irrelevant posts from random users who they were not following. Refining the post recommendation algorithm should be a priority to improve user experience.
2. **Translation**: Given Threads' global audience, the integration of a translation feature becomes fundamental in facilitating interactions among its diverse user base.
3. **Saving photos**: Enabling the option to save photos within Threads would increase the app's functionality and utility.
4. **Trending hashtags**: Incorporating a dedicated page showcasing hashtags would provide an easy access for users to be able to keep up with current popular trends.
5. **Dark theme**: A number of users also voiced complaints regarding the strains caused by the existing light theme. Introducing a dark theme option would enhance user comfort and app usability.
6. **Simplified account switching**: Users encountering challenges while toggling between personal and professional accounts suggest the need for an optimized account-switching process without the need to reverify every single time.
7. **Retrieving hidden threads badge**: Some users faced frustration due to the inability to restore their Threads badge on their Instagram profile after testing/accidentally hiding it.

## Conclusion
The decline in ratings highlights the urgency of improving the app, particularly by addressing performance-related issues and incorporating missing features to enhance user experience. With a targeted approach, Threads has the potential to succeed as a user-centric application.
