🌐💲# GNI-per-capita-Developing-countries-vs-Developed⏫⏬


📖Description:

The goal of this project is to create a model that predicts the GNI (Gross National Income) per capita in PPP (Purchasing Power Parity) in developing countries (Latin America) versus developed countries (Europe). 
For this project I used the data from the World Bank Group, more specifically, the data base on World Development Indicators.
I asked myself 3 questions that I wanted to answer within this project: 
> What are the characteristics most influential towards the GNI per capita ?

> Are there any differences between developing countries and already developed countries ?

> What is most influential towards the GNI per capita, Import or Export ?

📚[Data](https://github.com/G-dhlg/GDP-per-capita-Developing-countries-vs-Developed/blob/main/project.ipynb#assess): 

Here you can look at the steps that I took to process the data. I wanted to change the rows for the columns as I didnt see the years as an appropriate column name and my target was one of the columns.
I removed all the nulls in the following sections, see [here](https://github.com/G-dhlg/GDP-per-capita-Developing-countries-vs-Developed/blob/main/project.ipynb#clean)
I also divided the data set into two as I wanted to create a model specific to each type of country. Also this would help me answer my questions

🔬[Analisis](https://github.com/G-dhlg/GDP-per-capita-Developing-countries-vs-Developed/blob/main/project.ipynb#analyze):

I proceeded to look at how the data looked and what would be my expectations of the results. Wanted to see what columns had the most correlation with my target. 
Surprisingly, the values were different for the two data sets. As I expected, but it was still interesting what the correlations were. 

⚙️[Model](https://github.com/G-dhlg/GDP-per-capita-Developing-countries-vs-Developed/blob/main/project.ipynb#model):

I decided to do a gradient boosting regressor and I divided the data into train and test. 
The results for my model of European countries was a MSE of 1998732.61634141 which makes sense cause it is looking at the GNI which is in the millions if not billions of dollars. And a R2 score of 0.9675409761570172
The model for the developing countries had a MSE of 362483.6410773012 which also makes sense as they have a lower GNI. The R2 score for this model was 0.9470195819717997

✔️[Results](https://github.com/G-dhlg/GDP-per-capita-Developing-countries-vs-Developed/blob/main/project.ipynb#importance-of-each-variable):

👍After some graphs to look at the results, I proceeded to look at the answers for my 3 questions. 
> for the first one, I found out the most influential column towards the GNI per capita is Gross capital formation and industry for developed countries. For developing countries it was school enrollment and high technology export.

> As seen in the previous answer, for the second question of is there a difference? Yes there is, the economies are completely different.

> In terms of export or import for the exconomy, the most beneficial and influential is export as it ranks second for developing countries and fifth for the developed countries. 
