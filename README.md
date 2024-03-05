# Talent-Match - команда skibidi_MISIS
## ⌛ Task
Nowadays, the number of vacancies is growing exponentially. To do this, companies hire HR managers to recruit people, specialists. But it is difficult and slow to sort through thousands of resumes. To solve this problem, we have proposed our own algorithm for matching resumes with vacancies in the [Talent Match hackathon](https://ml-talentmatch.ru/);

💰 The first place prize was 75.000 rubles. Second and third got 50.000 and 25.000 rubles.


## 💾 Data
We have received 2 datasets with marked up and unmarked data. "__case_2_data_for_members.json__" contained structured data in the form of a dictionary, where there were 5-30 suitable and unsuitable resumes for each vacancy. 
Resume columns: __uuid__, first_name, last_name, birth_date, country, city, about, key_skills, experienceItem, educationItem;
Vacancy columns: __uuid__, name, keywords, description, comment;


## Technologies 

We trained and tried several detection models, but YOLOv8m turned out to be the best. We also used SAHI technology👽 for inference.

🎯 The best scores **(~0.78 mAP50)** after the private session. As a result, after the performance, we took the 3rd place🥉;
![image](https://github.com/timur612/insulator_defect_detection/assets/86769332/a19e8d5d-2b9b-4449-93c5-ae30b6a82d7a)
