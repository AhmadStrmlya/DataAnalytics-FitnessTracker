##### a case study recommended from google data analytics course

**The information below is just an overview** of what the case study is about and what recommendation I come up with. Check out the full analysis on the pdf that I've prodided, it's called "FitnessTrackerAnalysis.pdf"

## Case Study Scenario

You are a junior data analyst working on the marketing analyst team at Bellabeat, a high-tech manufacturer of health-focused products for women. Bellabeat is a successful small company, but they have the potential to become a larger player in the
global smart device market. Urška Sršen, cofounder and Chief Creative Officer of Bellabeat, believes that analyzing smart device fitness data could help unlock new growth opportunities for the company. You have been asked to focus on one of Bellabeat’s products and analyze smart device data to gain insight into how consumers are using their smart devices. The insights you discover will then help guide marketing strategy for the company. You will present your analysis to the Bellabeat executive team along with your high-level recommendations for Bellabeat’s marketing strategy.

### Recommendation:
### For Marketing Team
- **The best time to run the marketing campaign**

    - **People tends to be most active between 17:00 - 19:00**, so doing a marketing campaign during that time might be benefitial. With an assumption that there will be more people out there (who's not a user of bellabeat yet) at that spesific time that's currently doing exerices and try to look for an app that can track daily acitivies.
    - **More active people** happends to **start waking up between 04:00 - 07:00**. we run the campaign here with an assumption that we will get more active people at this time that might catch interest for the product.
- **Who to target**

    - Target **people who have interest in running** The app will track on your daily activities and have a detailed info for walking/running activity. 
    - **People who's looking to lose weight** can also be our marketing campaign target.
    - **Gym Member** will also catch interest in our product, so they can track progress of their workout routine.
    - The data that the app has can help **Someone that have a sleeping problem**. we can give them reccomendation on what to do to improve sleep quality.
- **Educational content topics**

    - **Topics related to running**
        - do atleast 5k steps a day (this is what average adults do daily) to have a better health or to achieve atleast 1,5k calories.
        - The intensity of the walk/run is more important than distance, if you're looking to lose weight
    - **Topics related to sleeping**
        - Waking up early leads to more active day
        - more sedentary activity will make you sleep worst from the duration point of view.
        - 6-8 hours of sleep to have a more active day
    - Make a content that **promotes what the app can do**. Since one of our target is active people that already done workouts and wanted to track their result. promoting what our app can track will also be able to catch their attention.
    
    
### For Product Team
- **Users are not only burning their calories through walking/running.** It's indicated from some user with almost no total active minutes can have more than 1.5k calories burn. So if it's possible we can detect other activities such as swimming, muscle building workouts, dancing/yoga, etc.
- **Improve the data collection method for heart rate data**, it can be done by improving the heart rate monitoring system or encourage the user to monitor it. Heartrate monitor is one of the way to check how healthy a user is. With this data collected we can know wether a user needed to see a doctor or not just by looking at their resting heart rate. And by improving the data collection for this feature, it might save some life. We can have a notification system for wether we don't recieve their heart rate data trough their phone, maybe the product is not fitted well to the user so the hardware can't detect heartbeat.
- Weight info have the same problem with heartrate, we need to **Improve the data collection method for Weight data**. Because with this data, we can track on a user weight loss journey. And the bellabeat main target audience is women, and women tends to have concern about their weight than men. If we can collect more data about user weight, we market the product even better! we can do this by giving the user notification that the system doesn't receive any weight data yet for the day.

### For Data Team
- **Consider having naming convention for both table and column name**. there's a table called `sleepDay`, but the column that hold the date is called "SleepDay" and it store the data with a datetime format "4/12/2016 12:00:00 AM", but on the other daily updated table, they all have the same column name called ActivityDay with a date format "4/12/2016". For table name, only 1 table naming is different, it's heartrate_seconds. All the other table name is using camel case naming convention.
- **Consider choosing a representitive column name**. For this, I notice there's a column called **"Value"** from `heartrate_seconds` and `minuteSleep` table. for `heartrate_sconds`, I know that the value represent what is the user current heartrate at the time. But for minute `minuteSleep`, the value is from 1-3 and I have to do further research for what it means. And i found that the value 1 means the user is asleep, but what about 2 and 3?. My suggetion is change the column name from value to heartrate for `heartrate_sconds` table, and whatever the value in `minuteSleep` table represent.
