# Fundamentals
Understanding these basic knowledge will allow one to better understand the intricacies of certain processes in data science.

## <a href="./prob_stat.md">Probability & Statistics</a>
It is **very** important to understand this section. This affects how we 
* Process the data 
* How models are built 
* Assumptions behind models 
* etc...

## <a href="./excel.md">Excel</a>
Think of excel as your first entry point and fallback. The most common file types you will deal with will likely be `.csv / .txt / .xlsx` , which means it can be open in excel. 

*Use excel for*
* To open the file first to see what it contains first
* To preprocess the file using excel first, making it easier to load into python. 

## <a href="./sql.md">SQL</a>
In some sense, knowing SQL is more important than knowing python. Data for organisations are all likely stored in relational databases, this requires you to know how to retrieve the data. The most important command is 
```
SELECT cols, cols, ... FROM table;
``` 
All other commands are extension of this. (pshh... bad advice but if you don't know how to work other commands... just load everything into python for processing)

## <a href="./python.md">Python</a>
Python is the way to go for applying machine learning I believe (#myownopinion). Having learnt and applied R for machine learning before moving to Python, this is why I prefer python
* Standardisation - one package to rule them all
  * eg. Scikit-learn is basically use to apply all python models, R has many different packages to apply a model (eg. rpart, party, etc... just to apply decision tree, each with different assumptions)
* More support available
* Faster and new updates
* Easier to branch to other areas (eg. moving into web development)
* Other reasons I've forgotten

***Note that this is a completely bias view***

