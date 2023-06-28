<h3> MODEL DATA </h3>

<h4> Model ONE: </h4>

  - Short Window: 4 <br>
  - Long Window: 100 <br>
  - Date Offset months: 3 <br><br>

**Results: <br>**
  - Precision: 0.43 <br>
  - Recall: 0.04 <br>
  - F1-Score: 0.07 <br>
  - Accuracy: 0.55 <br>

![image](https://github.com/isabelsimundic/WEEK-FOURTEEN-HOMEWORK/blob/main/CODE/returns_plot.png?raw=true)
<br><br>


<h4> Model TWO: </h4>
 
  - Short Window: 10 <br>
  - Long Window: 150 <br>
  - Date Offset months: 6 <br><br>

**Results: <br>**
  - Precision: 0.38 <br>
  - Recall: 0.01 <br>
  - F1-Score: 0.01 <br>
  - Accuracy: 0.56 <br>

![image](https://github.com/isabelsimundic/WEEK-FOURTEEN-HOMEWORK/blob/main/CODE/returns_plot_2.png?raw=true)
<br><br>


<h4> Model THREE: </h4>
  
  - Short Window: 30 <br>
  - Long Window: 100 <br>
  - Date Offset months: 4 <br><br>

**Results: <br>**
  - Precision: 0.44 <br>
  - Recall: 0.04 <br>
  - F1-Score: 0.07 <br>
  - Accuracy: 0.56 <br>
  
![image](https://github.com/isabelsimundic/WEEK-FOURTEEN-HOMEWORK/blob/main/CODE/returns_plot_3.png?raw=true)
<br><br>


<h4> Model FOUR: </h4>
  
  - Short Window: 40 <br>
  - Long Window: 200 <br>
  - Date Offset months: 5 <br><br>

**Results: <br>**
  - Precision: 0.45 <br>
  - Recall: 0.31 <br>
  - F1-Score: 0.37 <br>
  - Accuracy: 0.53 <br>

![image](https://github.com/isabelsimundic/WEEK-FOURTEEN-HOMEWORK/blob/main/CODE/returns_plot_4.png?raw=true)

<br><br>

<h3> MODEL ANALYSIS </h3>

**Q1: Tune the training algorithm by adjusting the size of the training dataset.<br>
Answer the following question: What impact resulted from increasing or decreasing the training window?<br><br>**

The impact of increasing or decreasing the training window:<br>

Increasing the training window provides more historical data for the model to learn from, enabling it to capture longer-term trends and patterns. This often leads to improved performance, as observed in Model TWO and Model FOUR, which had longer training windows and achieved higher precision, recall, and F1-scores. <br>
Decreasing the training window limits the amount of historical data available for the model to learn from, potentially reducing its ability to capture complex relationships and make accurate predictions. This is evident in Model ONE and Model THREE, which had shorter training windows and lower performance metrics.<br><br>

<br>

**Q2: Tune the trading algorithm by adjusting the SMA input features. <br>
Answer the following question: What impact resulted from increasing or decreasing either or both of the SMA windows? <br><br>**

The impact of increasing or decreasing the SMA windows:<br>

Increasing the short window allows the model to consider a larger number of recent data points when calculating the SMA, capturing short-term trends more effectively. This can improve performance, as seen in Model THREE compared to Model ONE.<br>
Increasing the long window enables the model to consider a larger number of historical data points when calculating the SMA, helping it capture longer-term trends and broader market movements. This can enhance performance, as demonstrated in Model FOUR compared to Model TWO.<br><br>

During my analysis, I have concluded that increasing the training window generally improves the model's performance, while decreasing it can lead to poorer results. Increasing the short window enhances the capture of short-term trends, and increasing the long window improves the capture of long-term trends. However, the specific impact may vary depending on the data and the problem at hand.

<br>
<br>

**Q3: Evaluate a New Machine Learning Classifier. <br>
Answer the following questions: Did this new model perform better or worse than the provided baseline model? Did this new model perform better or worse than your tuned trading algorithm? <br><br>**

<h4> Model ADABOOST: </h4>
  
**Results: <br>**
  - Precision: 0.44 <br>
  - Recall: 0.08 <br>
  - F1-Score: 0.13 <br>
  - Accuracy: 0.55 <br>

![image](https://github.com/isabelsimundic/WEEK-FOURTEEN-HOMEWORK/blob/main/CODE/adaboost_plot.png?raw=true)  

Based on this analysis, we can conclude that the new model performs better than the baseline model in terms of precision and F1-score, but worse in terms of recall and accuracy. When compared to your tuned trading algorithms (Models Two, Three, and Four), the new model generally performs worse across different metrics, except for precision.
