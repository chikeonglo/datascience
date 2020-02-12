<a href="../">Back to Index</a>

# Data Processing
What is data processing? Why do we need to process the data? Coming from the data science angle, the typical answer would be to "prepare the data for modelling" but is that truly the purpose?  

***Reminder to myself:*** We process the data to
* understand what is contained within the data
  * summary statistics
* visualise the distribution of the data
* examine the problematic areas
* identify potential relevant data / datasets that can be joined to the existing data
* define the objective of the dataset, the outcome we are interested in
* etc...

Remember data processing has been around for quite some time (excel, etc...) 

## <a href="./loading.md">Loading</a>
When it comes to loading data, there is basically only one goal, ensures that the data is loaded either as a `NumPy array` or `Pandas Dataframe`. It is best to be very familiar with both of these, including their intricacies, you will likely be working on these more than 90% of the time. 

There are other "niche" formats (eg. XGBoost - dmatrix, text - sparse matrix, ...) but they are either built on or can be converted into `NumPy array` or `Pandas Dataframe`.

## <a href="./visualisation.md">Visualisation</a>
We all know that visualisation is simply using a graph to demonstrate the relationship between 2 or more variables. Let's take a pause there. What exactly are the 2 variables? Will any 2 variable work?

Quick check (examples):
* Numerical + Numerical (eg. scatter, line, etc...)
* Numerical + Categorical (eg. boxplot, barplot, etc...)
* Categorical + Categorical (???)

Hmm... seems like there is some restriction on the variable type, one of it must be numeric (perhaps there is actually something but nothing comes to mind immediately).

## <a href="./processing.md">Cleaning / Manipulation</a>
This section is what we typically think of when the topic of data processing comes up. It is also quite straightforward, and perhaps we can think of this in 3 distinct parts
* Tidying data
* Joining data
* Cleaning data

Ensures that the data is properly setup, add additional data if necessary and finally clean the values as necessary.

