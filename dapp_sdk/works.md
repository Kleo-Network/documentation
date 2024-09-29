# How Kleo SDK Works
![](/images/flow.png)

#### User Owned Corpus
The corpus consists of multiple content owned by the user as captured from the LLM. 

#### Contextual Activity Classification Model
THis takes input from the **User Owned Corpus** captured creates a contextual classification based on most likely activity being performed. This in turn generates the activity chunks of specific activity. 

#### Activity Chunk Outputs
Multiple activity chunks are generated as outputs from the **Contextual Activity Classification Model**. Each activity chunks contains a lot of documents along top keywords in that activity.

#### Reranking Algorithm for Pages
   - Receives **Activity Chunks** as input.
   - Now based on reranking algorithm using Term Frequency / Inverse Document Frequency and Gemini Vector Embeddings, the pages are reranked based on most relevance. 
     - **Embedding Model**
     - **TF-IDF**
   - Entities already extracted from the page corpus, for top 10 documents is then sent to LLM once again. 

#### LLM - Large Language Model
It takes input from, 
     - **Reranking Algorithm for Pages** to get the most relevant pages with context.
     - **SDK Prompt**: A prompt from the SDK specifying additional requirements.
The **LLM** processes the information and provides the most suitable user-owned data considering the given context and SDK prompt.

#### Result
   - Outputs the final result based on the decision made by the **LLM**.

