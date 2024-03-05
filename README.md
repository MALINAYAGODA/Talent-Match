# Talent-Match - команда skibidi_MISIS
## 🕙 Task
Nowadays, the number of vacancies is growing exponentially. To do this, companies hire HR managers to recruit people, specialists. But it is difficult and slow to sort through thousands of resumes. To solve this problem, we have proposed our own algorithm for matching resumes with vacancies in the [Talent Match hackathon](https://ml-talentmatch.ru/);

💰 The first place prize was 75.000 rubles. Second and third got 50.000 and 25.000 rubles.


## 💾 Data
We have received 2 datasets with marked up and unmarked data. "__case_2_data_for_members.json__" contained structured data in the form of a dictionary, where there were 5-30 suitable and unsuitable resumes for each vacancy. 
- __Resume columns__: uuid, first_name, last_name, birth_date, country, city, about, key_skills, experienceItem, educationItem;
- __Vacancy columns__: uuid, name, keywords, description, comment;


## Technologies 

We tried several methods and models🌎, but stopped at the [article](https://arxiv.org/abs/1908.10084), the Siamese model👽. How our solution works:
1) Preprocessing, lemmatization, tokenization
2) Sending data via __distil-roBerta__ to receive embeddings
3) Training a __Siamese__ neural network with 2 branches and the last layer of the classifier
**Сonclusion**: a good model, a core that gave Precision=0.33, Recall=0.8, Validation loss=0.68;

We created a base NN for further upgrades and in the end we took the 2nd 🥈place;__ 
(One job description and the top 2 suitable resumes that the model issued🔎)
![image](https://github.com/MALINAYAGODA/Talent-Match/blob/main/picture/photo_waifu2x_photo_noise1_scale.png)
