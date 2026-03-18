# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
import seaborn as sns
import matplotlib.pyplot as plt

df=sns.load_dataset("iris")
corr_matrix=df.select_dtypes(include=["float64"]).corr()
sns.heatmap(corr_matrix, annot=True, cmap="coolwarm")
plt.show()

sns.jointplot(x='sepal_length',y='sepal_width',data=df,kind='hex')

sns.jointplot(x='sepal_length',y='sepal_width',data=df,kind='reg')

sns.pairplot(df)

sns.pairplot(df,hue='species')

sns.distplot(df['sepal_width'])

sns.distplot(df['petal_length'],kde=False,bins=10)

sns.countplot(x='species',data=df)

sns.countplot(y='species',data=df)

sns.barplot(x='sepal_length',y='sepal_width',data=df)

sns.boxplot(x='sepal_length',y='sepal_width',data=df)

sns.boxplot(x='sepal_length',y='sepal_width',data=df,palette='rainbow')

sns.boxplot(data=df,orient='v')

sns.boxplot(x='sepal_length',y='sepal_width',data=df,hue='species')

sns.violinplot(x='sepal_length',y='sepal_width',data=df,palette='rainbow')

```
<img width="837" height="480" alt="Screenshot 2026-03-18 155433" src="https://github.com/user-attachments/assets/af146c13-d38d-401b-9b3a-aea86a638682" />
<img width="823" height="708" alt="Screenshot 2026-03-18 155443" src="https://github.com/user-attachments/assets/f167c01c-e61c-46fc-9772-a453e2585a71" />
<img width="827" height="699" alt="Screenshot 2026-03-18 155454" src="https://github.com/user-attachments/assets/792357b2-9f58-425a-8d4b-daa42625bc22" />
<img width="769" height="579" alt="Screenshot 2026-03-18 155711" src="https://github.com/user-attachments/assets/d12026f1-47a8-474d-b07c-cc8e7298e1e1" />
<img width="771" height="600" alt="Screenshot 2026-03-18 155703" src="https://github.com/user-attachments/assets/813f2b64-a718-4722-93ad-2c3cc96f52e6" />
<img width="877" height="563" alt="Screenshot 2026-03-18 155656" src="https://github.com/user-attachments/assets/95bc9353-7673-4b0b-9b2f-85572c71a1c0" />
<img width="819" height="588" alt="Screenshot 2026-03-18 155644" src="https://github.com/user-attachments/assets/3573a494-a541-45d1-b969-e65d3985c46e" />
<img width="813" height="588" alt="Screenshot 2026-03-18 155635" src="https://github.com/user-attachments/assets/1877f72e-c000-4087-8b38-fe2aa4528c5a" />
<img width="841" height="584" alt="Screenshot 2026-03-18 155627" src="https://github.com/user-attachments/assets/329fa125-7354-492d-a50b-3bd145f0ba4a" />
<img width="813" height="590" alt="Screenshot 2026-03-18 155615" src="https://github.com/user-attachments/assets/733368ec-c217-479b-a459-496ff2978db9" />
<img width="817" height="590" alt="Screenshot 2026-03-18 155608" src="https://github.com/user-attachments/assets/e7703a08-e92f-45fe-b1e6-37c2ff9fd28f" />
<img width="820" height="578" alt="Screenshot 2026-03-18 155600" src="https://github.com/user-attachments/assets/438abad1-61bf-4d4a-9666-bb2459ad91ca" />
<img width="828" height="586" alt="Screenshot 2026-03-18 155550" src="https://github.com/user-attachments/assets/8b9eb930-66d6-4b69-85d2-42875ef5f489" />
<img width="901" height="833" alt="Screenshot 2026-03-18 155536" src="https://github.com/user-attachments/assets/dd5020fe-e862-4964-af37-3d278e7efe4c" />
<img width="894" height="839" alt="Screenshot 2026-03-18 155521" src="https://github.com/user-attachments/assets/9cc1f752-75cb-42bf-92b8-eb0975fafe67" />



# Result:
 Include your result here
