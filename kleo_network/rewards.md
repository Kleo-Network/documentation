---
label: Rewards for Data
layout: page
---

# Proof Of Contribution Algorithm 

Proof of contribution is built on three major factors, 

- **uniqueness** (calculated using TF-IDF over entire data) 
- **nature of activity**  (activities like doom scrolling get less views)
- **AIable** Can I do what you do? If your actions are not replicable by models, then it is not. 

#### Uniqueness

Uniqueness is measured using the TF-IDF (Term Frequency-Inverse Document Frequency) method, which evaluates how distinctive a user’s contribution is within the entire dataset. The algorithm assesses the frequency of words or actions specific to an individual’s activity compared to the general activity of all users. Higher uniqueness indicates that the content or activity is less common and therefore more valuable.

#### Nature of Activity

The nature of activity considers the type of actions a user performs. Not all activities are treated equally; for instance, activities like “doom scrolling” or passive browsing receive lower value as they lack engagement or productivity. The algorithm prioritizes activities that add more value, such as creating content, engaging meaningfully, or contributing to discussions.

#### AIable

This factor evaluates whether the actions a user performs can be replicated by AI models. If the actions are complex, creative, or require human intuition—something that AI cannot easily replicate—the contribution is scored higher. This ensures that users who bring human-centric skills and creativity are rewarded, emphasizing the importance of unique, non-automatable behaviors.

All these factors also determine overall data quality and thus the activity with highest data quality is something you should pursue. 