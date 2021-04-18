# Neural Net Charity Analysis

For this analysis, we review the likelihood of a charity appropriately allocating the money they receive. The intent is to make sure funds aren't given to charities that spend the bulk of their donations on administrative costs with little going to the intended recipients. We ultimately want to create a model that can predict to at least 75% accuracy. 

The model that we hope will attain that desired accuracy is a neural net. A neural net is a machine learning model that consists of three key components. 

1. An input layer, i.e columns of a csv file
2. A hidden layer with a certain number of neurons
3. An output layer which gives our predictions. 

---

### Resources
[Source Data CSV File](https://github.com/carlosjennings1991/Neural_Network_Charity_Analysis/blob/main/charity_data.csv)
<br>
[Code File](https://github.com/carlosjennings1991/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity.ipynb)

### Tools Used
- [x] sklearn
- [x] pandas
- [x] tensorflow
- [x] support vector machines
- [x] jupyter notebook

## Results
### Step 1: Preprocess our data
This is typically the first step for any machine learning model. We fed in a csv file that contained a few parameters that would have no affect on our data, i.e the 'EIN' (employee identification number) and 'NAME' columns. We drop these columns. 

<img src="https://github.com/carlosjennings1991/Neural_Network_Charity_Analysis/blob/main/columns_highlighted.png">

### Step 2: Bin the values of the Application and Classification Columns
What we do here is bin all the small, uncommon values into a category called 'other'. This reduces the noise in the model. 

<img src="https://github.com/carlosjennings1991/Neural_Network_Charity_Analysis/blob/main/other_highlighted.png">

### Step 3: Run our first neural net. 
This neural net consists of an input layer 80 neurons and a hidden layer of 30 neurons. The activation algorithms of layer 1 and 2 are Rectified Linear Units 'ReLu', and the output layer algorithm is sigmoid. 

<img src="https://github.com/carlosjennings1991/Neural_Network_Charity_Analysis/blob/main/NN_1_Summary.png">

After running the model through 100 epochs, the model generates a 72.6% level of accuracy, which is not good enough for our purposes. 

<img src="https://github.com/carlosjennings1991/Neural_Network_Charity_Analysis/blob/main/NN_1_Evaluation.png">

#
## Summary
