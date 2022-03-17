# Data Analyst, Data Scientist: Who is Who? 🤌🏼 🤷🏽‍♂️
A Data-Related Labour Market Analysis

## Why this project ❓❓❓
I am a Psychologist transitioning to the Data world, and I'm having a bit of an identity crisis when it comes to choosing between a Data Analyst and a Data Scientist role.


## How did I do it? 🔧 ⚙️

### 1. LinkedIn & Glassdoor Web Scraping using Selenium 🌐
I created a bot with the Selenium library in Python that scraped LinkedIn's jobs page and Glassdoor to extract all Data Analyst and Data Scientist job offers published in the last month in Barcelona. From there, I obtained:
- The job title
- The job description
- The company
- The location of the job (remote, on-site or hybrid)
- The company's industry

Doing Web Scraping on LinkedIn is not easy, since they carefully design their webpage to avoid it, but with some patience and effort, it was done! 💪🏽

### 2. Natural Language Processing with Python & NLTK 💬 💻
Once I gathered all the data, consisting of 210 job offers, from which 57% belonged to Data Analyst positions and 43% to Data Scientist ones, I used NLP tools to transform it to meet my needs. These transformations consisted, mainly, in the general cleaning of the descriptions (including some translations), feature extraction, tokenization and lemmatization.  

Once my data was tokenized and cleaned, I proceeded with the keyword analysis. I selected keywords related to the education level and the majors, tools, hard and soft skills currently demanded for each position. This selection was based on information gathered from the Internet and some exploration around the descriptions to catch some keyword patterns.

With these keywords at hand, I proceeded to obtain the count frequencies of appearance of the keywords in the description. I did that using the TfidfVectorizer from sklearn, which allows scaling down the impact of tokens that occur very frequently in a given corpus and that are hence empirically less informative.

### 3. Visualization in Tableau & Presentation 📊
The next step of the process was to visualize the insights extracted in a simple way through Tableau. You can check my work in my Tableau Public [profile](https://public.tableau.com/app/profile/marcsoler/viz/FinalProjectPlots/ed_level_1) and in this very [repository](https://github.com/marc-soler/Ironhack_final_project/tree/main/Tableau%20Plots).

After all this work, it was time to present it to a non-technical audience. I used these [slides](https://github.com/marc-soler/Ironhack_final_project/blob/main/slides.pdf) as a visual support.

## Key Takeaways ‼️
- Education level required for Data Scientists is significantly higher than that of Data Analysts.
- Machine Learning is almost entirely a job for Data Scientists.
- Data Analysts mostly do Visualization, Reporting and Business Intelligence, and use SQL as their main tool.
- Apart from that, roles are not that differentiated, so apply to every position that appeals you, especially if it's an entry level or a Junior one!

Hope you've enjoyed it,

Marc
