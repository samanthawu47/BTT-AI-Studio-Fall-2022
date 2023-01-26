# Break Through Tech AI @ Cornell Tech | AI Studio Project Fall 2022

### Project Statement

USA for UNHCR is an organization that facilitates aid, which may be in the form of donations, from the public to refugees. Since monetary contributions are a way to bring visible, tangible change, it is important to observe the behavior of actual donors, possibly encouraging different public outreach techniques. The objective of this project is to predict which subscribers on an email list will become donors using email-related data and previous contribution history.

### Approach

Our approach is to utilize binary classification models to predict who will become a donor and to visualize the behavior of subscribers chronologically to understand the actions that lead to donations. We leveraged resources, including packages such as pandas, scikit-learn, NumPy, and matplotlib, and Google Colab for exploratory data analysis, data cleaning, and model training. More specifically, we trained logistic regression and decision tree models due to their interpretibility among a variety of audiences. 

### The Dataset

For this project, there were five tabular datasets obtained from the organization. Each dataset contained information regarding:
- Donations: contributions and their corresponding campaign within the past year.
- Clicks: when and what types of links (i.e. donation, action, awareness URLs) were clicked in emails
- Opens: when emails were opened
- Sent: when emails were sent
- Bounces: when and what type of bounces (hard, soft, block, etcetera) occurred

We merged each dataset according to each email's contact ID, which is a identifying string unique to each individual. Due to the nature of the selected models, features containing strings were removed. The label was binary, indicating whether someone would become a donor. Overall, the dataset was sparse, meaning that a significantly small percentage of users had donation data, requiring scaling. Because of this, the accuracy of the models was poor.

### Impact

The data has shown that there is a correlation between those who precede donations with actions, which include gaining awareness and signing petitions. However, a very small fraction of subscribers are donors. Since the performance of the models was low, future steps may include addressing this issue while delving deeper into more complex models and more heavily considering time features.
