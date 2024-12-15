### **(1) Project Title**  
Analyzing MMA Fight Data for Performance Insights and Safety Trends

### **(2) Team Members**  
Kyndra Nelson - CSCI 4502
Spartak Mikayelyan - CSCI 4502
Varun Cheela - CSCI 4502
Khushbu Adhikari - CSCI 4502
Brody Frankovich - CSCI 4502 

---

### **(3) Brief Project Description**  
Mixed Martial Arts (MMA) has become one of the fastest-growing sports globally. As the sport evolves, fighters and coaches increasingly rely on data to inform strategies and improve performance. Our project aims to analyze MMA fight data to gain insights into fighter performance, techniques, and trends over time. This can contribute to enhancing training methods and ensuring safety in the sport.

**Key Questions/Inquiries**:
- Orthodox vs Southpaw vs Switch with win ratio  
- Career trajectory after fighting (if data is available)
- Comparing 2023 data vs all-time data since 1994   
- Success by age: Comparing fighters under 20 vs over 20
- Common injuries with the sport and what causes them 

---

### **(4) Dataset(s) to be Used**  
- [MMA Dataset 2023 (UFC)](https://www.kaggle.com/datasets/remypereira/mma-dataset-2023-ufc/data)  
- [MMA Differentials and Elo](https://www.kaggle.com/datasets/danmcinerney/mma-differentials-and-elo?select=masterdataframe.csv)  

---

### **(5) Tool(s) Used**  
- **Software**: Kaggle, Jupyter, GitHub  
- **Coding**: Pandas, Python, R, pyplot
- **Communication**: GroupMe, Outlook, Zoom
  
---

### **(6) Milestones**
- Milestone 1: Data acquisition and cleaning (Weeks 1-2)
    Obtain datasets and clean them for analysis
- Milestone 2: Data analysis (Weeks 3-5)
    Analyze win ratios, statistics, strike hit percentages, and success by age 
- Milestone 3: Visualizations and insights (Week 6-7)
    Generate visualizations 
- Milestone 4: Report writing and presentation (Weeks 8-9)
    Compile the final report with key findings, insights and recommendations for fighter training and strategy. 

---

### **Introduction**  
[To be written based on your project introduction.]

### **Related Work**  
Previous research has extensively analyzed sports data to uncover performance insights across various disciplines, including boxing, wrestling, and football. However, limited attention has been given to Mixed Martial Arts (MMA), particularly in the areas of safety trends and performance optimization. 

While some studies have explored the relationship between fighter stances and winning outcomes, few have delved deeper into key variables such as strike locations, age, and punch differentials. Our project not only builds on these foundational studies but also introduces new dimensions, such as using machine learning to predict which fighters are most likely to have injuries in the future.

Example works:  
- "Analysis of UFC Fight Statistics and Models for Fight Results and Over/Under Prediction" by Sanjiv Pradhanang analyzed UFC fight statistics to build models for predicting fight results. This work provides insights into key variables like fighter stance, strike accuracy, and win percentages, laying the groundwork for our MMA data analysis.

- "UFC Fighters Statistics" on Kaggle is a dataset of UFC fighter statistics, focusing on various fighter metrics like height, reach, and fight outcomes. This dataset informs our analysis of key performance indicators such as strike differentials and fighter win ratios.

- "Scraping and Analyzing UFC Fight Data" by Shajon Islam involved scraping UFC fight data and conducting statistical analysis to understand fighter trends. This work helps inspire our data collection and analysis methods for MMA fight data.

### **Proposed Work**  
In order to determine the role age had in winning fights in MMA, fighters were grouped into 10 equal buckets based on their age, and then a bar graph was constructed based on these age buckets and their corresponding win ratio. This method accounted for the issue with extreme age values having few data entries and provided a more robust understanding since each bucket had enough samples to give proper insight. Age grouping also gave the ability to get granular insight on how win ratios change throughout the stages of a fighter's career.

Strike patterns were also analyzed across weight divisions and genders, in order to determine the influence that different classes had on fight strategies. This analysis was done to observe whether striking tendencies-head strikes, body strikes, and leg strikes-are very different between the groups, providing valuable insights for fighters and coaches to use in developing their strategies within the division-specific trends.

Correlation analysis was done for a fighter's physical attributes, such as their height, weight, and reach and their win ratio in order to determine whether a fighter's physical features play a role in a fights outcome. K-means clustering was also done for the fighters height, weight, and reach for win ratio. The number of clusters was decided upon by using the elbow method where a k- means was run for cluster numbers between 1 and 11, and calculating their within cluster sum of squares. The cluster number was chosen to reduce the within cluster sum of squares, but not too many to the point of diminishing returns. Correlation analysis was also done on the number of knockdowns, which happens when a strike puts any part of the opponent other than their feet onto or touching the ground, and win ratio to determine whether knockdowns should be prioritized by fighters.

The number of knockdowns was also put in correlation with the win ratios so as to assess whether fighters should focus on knockdowns. A knockdown is classified as a strike that puts any part of an opponent (other than the feet) onto the ground and very often is really what dictates the decisive moments within the fight. The correlation to the victory rates speaks highly of high-impact activities that change outcomes.

Other fighter attributes and fight actions, such as stance and win methods, were also analyzed in an attempt to show their influence on win ratios. The analysis looked at these factors to find less obvious strategic advantages that would help fighters improve their approach in the octagon.

### **Evaluation**  
In our findings, younger fighters generally seem to do better than older fighters. Most fights in MMA are determined by the judges decision, either unanimous, or split. The judges score fights based on strike effectiveness, strike power, and strike accuracy, as well as ground control. It was also revealed that fighters should prioritize being on the offensive, focussing on landing as many strikes as possible, attempting smaller strikes even if they don’t always hit, throwing significant strikes only if they are sure they will land, knockdowns, and hitting the opponent's head as frequently as possible. Chokes and other submissions were also shown to be effective ways of winning, but should not be prioritized over dealing significant strikes. They should only be used when the opportunity presents itself. An open stance also seems to be the most effective stance in comparison with the more common orthodox stance.

Safety trends and insights were analyzed using statistical analysis in order to find ways to minimize injury risks while maintaining competitive performance. It was noted that fights with longer control times and fewer high-impact strikes tend to have fewer injuries, suggesting a balance between aggression and defense is required for long-term fighter health. Fighters with a strategic emphasis on ground control and effective defense showed the lowest rate of injury, underpinning the importance of involving more defensive drills in various training programs. Furthermore, age-group analysis has brought out the fact that injuries are less severe in younger fighters while older fighters take longer recovery periods and more concentrated safety measures due to loss of physical resilience. These findings can be used to refine safety protocols, optimize fighter longevity, and promote sustainable career development in MMA.

The project is considered successful for generating actionable insights, providing statistically validated trends, and offering tools for data-driven MMA training and strategy. 
