# Reddit Research Analysis Plan

## Overview
Частка новин пов'язаних з виборами та можливими гострими темами, щодо них → два графіки

**Total Expected Outputs:** ~29 questions + visualizations

---

## 1. EDA (Exploratory Data Analysis)

### 1.1 General Activity Metrics
- **Скільки загалом постів було кожного тижня?** *(1 visualization)*
  - Weekly time series plot of total post volume
  - Shows overall Reddit activity trends over time

### 1.2 Election-Related Content
- **Який % сабмішинів/коментарів стосувався виборів або довкола виборчих тем** *(3 visualizations)*
  - Weekly ratio of election-related submissions over time
  - Weekly ratio of election-related comments over time
  - Overall proportion comparison (pie charts for submissions and comments)
  - Results: ~35% of both submissions and comments are election-related

### 1.3 Engagement Analysis
- **Скільки коментарів в середньому мали сабмішини пов'язані з виборами у порівнянні з усіма** *(2 visualizations)*
  - Weekly average comments comparison (line plot)
  - Monthly average comments comparison (grouped bar chart)
  - Compares election-related vs. all submissions

- **Середній скор овертайм для сабмішинів** *(2 visualizations)*
  - Weekly median score over time (election-related vs. all)
  - Weekly mean score over time (election-related vs. all)

### 1.4 Subreddit Popularity
- **Які були найпопулярніші сабредіти** *(3 visualizations)*
  - Top 15 by submission count (horizontal bar chart)
  - Top 15 by comment count (horizontal bar chart)
  - Top 15 by total upvotes/score (horizontal bar chart)
  - Top subreddits: r/canada, r/CanadaPolitics, r/onguardforthee

- **Скільки кожен сабредіт приносив постів до даних овертайм** *(1 visualization)*
  - Weekly time series for top 10 subreddits showing submission trends

### 1.5 User Analysis
- **Топ 10 користувачів які генерують найбільше сабмішинів і які у них погляди** *(2 visualizations)*
  - Top 10 users by submission count (bar chart)
  - Political leaning distribution of top contributors (stacked bar chart showing Liberal/Conservative/Centrist percentages)
  - Top user: u/Worldly_Effective679 with 1,679 submissions

### 1.6 Political Score Analysis
- **Середній скор сабмішинів за політичним ухилом овертайм** *(1 visualization)*
  - Weekly average score by political category (Liberal/Conservative/Centrist)
  - Text-based categorization using keywords

**Subtotal: 15 visualizations**

---

## 2. Настрої (Sentiment Analysis)

### 2.1 Political Wing Classification
*Праві/ліві (виділити правих та лівих, перетини прибрати якщо ділитиму по ківордах)*

### 2.2 Wing-Based Engagement
- **На самбішини якого крила реагували найбільше** *(1 visualization)*
  - Compare reaction metrics by political wing

- **Сабмішини якого крила мали більшу кількість коментарів** *(1 visualization)*
  - Mean amount of comments per submission over time

- **Сабмішини якого крила мали вищий sentiment скор з часом** *(1 visualization)*
  - Sentiment trends by political wing

### 2.3 Subreddit Political Leaning
- **Чи існують суб-реддіти з чітким політичним ухилом, де домінують лише ліві або лише праві погляди?**
  - Identify politically homogeneous communities

**Subtotal: 3+ questions + visualizations**

---

## 3. Щодо Людей (Entity Analysis)

*Note: Дропнути країни і міста*

### 3.1 Entity Mentions in Election Content
- **Хто найчастіше з'являвся в постах, що election related** *(2 visualizations)*
  - Overtime trend
  - Bar plot summary

### 3.2 Political Context of Key Figures
- **Де частіше з'являвся Trudeau, Trump, Mark Carney та Pierre Poilievre** *(1 visualizations)*
  - Presence in left/right/centrist discussions

### 3.3 Sentiment Toward Political Figures
- **Який сентімент був у лівих, правих та центристів щодо:** *(10 visualizations)*
  - Trudeau (overtime + bar plot)
  - Trump (overtime + bar plot)
  - Mark Carney (overtime + bar plot)
  - Pierre Poilievre (overtime + bar plot)

**Subtotal: 15 questions + visualizations**

---

## 4. Causal Inference

### 4.1 Event Impact Analysis
*Методологія: t-test на сентимент для дат до і після події*

#### Key Events to Analyze:
1. **Американські вибори**
   - Чи вплинули на зміни настроїв та активність лівих/правих та центристів?

2. **Тарифи**
   - Чи вплинули на зміни настроїв та активність лівих/правих та центристів?

3. **Дебати**
   - Чи вплинули на зміни настроїв та активність лівих/правих та центристів?

4. **Відхід Трюдо**
   - Чи вплинув на зміни настроїв та активність лівих/правих та центристів?

5. **Прихід нового прем'єра**
   - Чи вплинув на зміни настроїв та активність лівих/правих та центристів?

### 4.2 Comparative Analysis
- **Що вплинуло найбільше з цих гіпотез на зміну?** *(1 visualization)*
  - Compare effect sizes across all events

**Subtotal: 6 questions + analyses**

---

## Summary

| Section | Number of Questions/Visualizations |
|---------|-----------------------------------|
| EDA | 15 |
| Настрої | 3 |
| Щодо Людей | 15 |
| Causal Inference | 6 |
| **Total** | **~39** |
