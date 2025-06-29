## Analysis Questions & Key Findings

This project aimed to analyze the `News_2025.csv` dataset to uncover various patterns and insights related to news publication. Below are the questions addressed and their key findings:

### Initial Questions:

1.  **How many distinct news sources are represented in our dataset?**
    * **Finding:** There are **98 distinct news sources** present in the dataset.

2.  **Which news sources are the most prolific, contributing the highest number of articles to the dataset?**
    * **Finding:** The most prolific news sources include **The Daily Galaxy** (13 articles), **The New York Times** (11 articles), and **Space** (8 articles).

3.  **Can we extract and analyze the top-level domains from the `sourceUrl` column to understand the variety of news outlets (e.g., `.com`, `.org`, `.gov`)?**
    * **Finding:** The most frequent domains broadly align with the top sources, with `dailygalaxy.com`, `www.nytimes.com`, and `www.space.com` being the most prominent.

4.  **Are there any significant trends or spikes in news publication over time (e.g., daily, weekly)?**
    * **Finding:** News articles are most frequently published on **Thursdays** (99 articles) and **Wednesdays** (87 articles). Publication activity peaks during the **late morning and afternoon hours** (specifically from 9 AM to 5 PM UTC).

5.  **What is the statistical distribution of news title lengths (e.g., average, median, minimum, maximum, and standard deviation)?**
    * **Finding:** News titles have an average length of approximately **12.7 words** (mean), with a standard deviation of about 3.68 words. Title lengths range from a minimum of 3 words to a maximum of 29 words. The median title length is 12 words.

6.  **Is there a noticeable relationship between the length of a news title and its source, or the day of the week it was published?**
    * **Finding:** Sources like **Wccftech** (29 words), **Hindustan Times** (23 words), and **Daily Mail** (22 words) tend to have significantly longer titles on average. Average title lengths by day of the week are relatively consistent across Tuesday, Wednesday, and Thursday (around 12-13 words).

7.  **Beyond just individual words, can we identify common phrases or significant keywords that frequently appear in the news titles?**
    * **Finding:** The overall most frequent words in the titles (including common English words like 'the', 'to', 'in', 'a', 'of' due to limitations in stop word removal) provide a general sense of topics.

8.  **Do certain news sources exhibit patterns in the *types* of news they report, based on the keywords in their titles?**
    * **Finding:** Even with raw word counts, we observed source-specific patterns:
        * **The Daily Galaxy:** Focus on scientific discoveries and space (e.g., 'reveals', 'mysterious', 'tiny', 'electron').
        * **The New York Times** & **Politico:** Strong focus on politics and international relations (e.g., 'russian', 'trump', 'iran', 'weak', 'dnc').
        * **NPR:** Specific news events ('missile', 'moths').
        * **ScienceAlert:** Scientific and biological terms ('dragon', 'human', 'axolotl').

### Additional Analysis:

1.  **Publication Volume Trends Over Time:**
    * **Finding:** Visualizing daily publication volume (as shown in `daily_publication_volume.png`) confirms varying news activity, with Thursdays and Wednesdays generally showing higher publication counts.

2.  **Unique Keyword Identification per Source:**
    * **Finding:** Our simplified 'uniqueness score' identified words more characteristic of individual sources, reinforcing their thematic focus (e.g., 'reveals' for Daily Galaxy, 'russian' for NYT, 'weak' for Politico).

3.  **Analysis of Missing Image Data:**
    * **Finding:** Out of 195 entries, **16 articles are missing image URLs.** These missing images are most frequently associated with sources like **Politico** (4), **Axios** (3), **The New York Times** (3), and **Barron's** (3). A significant majority of these (11 out of 16) were published on **Thursdays**.
