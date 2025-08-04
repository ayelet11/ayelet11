# Hi there, I'm Ayelet 👋

👩‍💻 **Data Scientist | M.Sc. Student**  
Specializing in **Time Series Analysis** and **Computer Vision**  
Currently pursuing my Master’s degree and passionate about uncovering insights from data.

## 🛠️ Skills & Tools
- **Languages:** Python, SQL
- **Expertise:** Data Exploration & Modeling, Machine Learning, Deep Learning
- **Libraries:** pandas, NumPy, scikit-learn, TensorFlow, PyTorch

## 🚀 Projects
*Coming soon!*  
Stay tuned for highlights of my favorite work in Data Science, Time Series, and Computer Vision.

## 🎓 About Me
- Always learning and growing in the field of data science
- Enjoy translating data into actionable insights and innovative solutions

> “Once I was an amateur now I am a professional (thanks bro for getting me to ponder this).”

## 📫 Connect with Me
[![LinkedIn](https://img.shields.io/badge/LinkedIn-ayelet--garber-blue?logo=linkedin&logoColor=white&style=flat-square)](https://www.linkedin.com/in/ayelet-garber-bb3b2b58/)

---

*Let’s connect, collaborate, and explore the world of data together!*

&#x202b;הסבר המטריקה demographic_parity_ratio: מחשבים את קצב הבחירה (הקצב שבו פרט מתוך הקבוצה הרגישה נבחר להיות 1) לכל קבוצה רגישה. 
&#x202b;לוקחים את **היחס** בין הקטן ביותר לבין הגדול ביותר מבין הקבוצות.  
&#x202b;שם אחר ל demographic parity הוא group fairness.  
&#x202b;יחס הוגן נחשב בין 0.8-1.0.  
&#x202b;הסבר המטריקה  equal_odds_ratio: מחשבים את true positive rate לכל קבוצה רגישה,  
&#x202b;ואת היחס בין הקטן לגדול ואת ה false positive rate לכל קבוצה רגישה ואת היחס בין הקטן לגדול.  
&#x202b;לוקחים את היחס עם הערך המינימלי בתור המדד ל"סיכויים שווים".  
&#x202b;יחס הוגן נחשב בין 0.8-1.0.  

&#x202b;אימנתי כמה פעמים את המודל כדי לחזות את מקבלי השכר הגבוה.  
&#x202b;בכל פעם הרצתי על גבי המודל המאומן משפר הוגנות הנקרא Threshold Optimizer לשיפור הוגנות של קבוצה רגישה אחת  
&#x202b;אשר דואג להוגנות ע"י קביעת סף אחר לכל קבוצה.  
&#x202b;המטריקה שבחרתי לכיוונון ההוגנות היא demographic_parity.  
&#x202b;הנוסחה המדויקת של השימוש בסף לפי קבוצה היא הסתברותית,  
&#x202b;ומשתמשת בהסתברות p0 על מנת לקבוע בחירה של 1 אם הפלט הגולמי של המודל עובר את הסף הגבוה לקבוצה זו - operation0,  
&#x202b;ובהסתברות המשלימה p1 לקבוע בחירה של 1 אם הפלט הגולמי עובר את הסף הנמוך יותר - operation1.   

&#x202b;הוספתי פיצ'ר is_older לציין עובד מבוגר - מגיל 50 ומעלה.  

&#x202b;אנו רואים בפלט התוצאות בקובץ results_before_after_threshold_optimizer.html  ששימוש ב threshold optimizer על כל הקבוצות הרגישות, כל פעם על קבוצה אחרת,  
&#x202b;מגדר, גזע, מצב אישי, ארץ מוצא, וגיל מבוגר בחלק מהמקרים למצב של הוגנות לפי demographic parity,  
&#x202b;כלומר היחס בין ה selection rates הקבוצתיים (החיזוי של להיות עם משכורת גבוהה עבור פרט מקבוצה זו) היתה מעל 80%,  
&#x202b;עבור הקבוצות הרגישות **מגדר ועובד מבוגר**, ועבור הקבוצות גזע ומצב אישי ההוגנות מאוד השתפרה והיא כמעט נחשבת הוגנת.  
&#x202b;רק עבור קבוצת ארץ מוצא ההוגנות לפי מדד זה נשארה  0.  
&#x202b;לפי קובץ פילוח המשכורות הגבוהות בנתונים המקוריים לפי ארץ מוצא,original_native_country_counts.html ,  
&#x202b;רואים שבחלק מארצות המוצא יש קצב בחירה של חצי או שליש אבל יש קבוצה עם קצב בחירה של 5% בערך -  
&#x202b;מה שמטה את המודל המקורי באימון המקורי שלו לנבא רק 0 עבור קבוצה זו.   
&#x202b;שיטת ה threshold optimizer לא מיועדת להתגבר על כך.

&#x202b;אנו רואים בפלט התוצאות שלפי equalized odds ratio ה threshold optimizer לא הצליח להביא אף לא קבוצה אחת למצב של הוגנות.  
&#x202b;הקבוצה שכמעט נחשבת במצב הוגן היא קבוצת העובדים המבוגרים.  
&#x202b;אולי היתה הצלחה גדולה יותר אם ה threshold optimizer היה משתמש במטריקה זו לכיוונון ההוגנות.  

&#x202b;לסיכום מודל שיאומן עם מודל LogisticRegression ללא תיקון של post processing יסבול מהטיות לגבי כמה קבוצות רגישות.  
&#x202b;השתמשתי ב:Grimoire (ChatGpt), Gemini (from browser), Perplexity.AI  
&#x202b;וב:   
[https://iamrajatroy.medium.com/evaluate-model-fairness-with-fairlearn-97a8985074fd] (https://iamrajatroy.medium.com/evaluate-model-fairness-with-fairlearn-97a8985074fd)  
[https://fairlearn.org/v0.10/quickstart.html] (https://fairlearn.org/v0.10/quickstart.html)  
&#x202b;יצירת דו"ח ה md בעזרת חוקים מ:
[markdownguide] (https://www.markdownguide.org/basic-syntax/)
