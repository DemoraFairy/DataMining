Running the Code
==========

The code is split into different functions. This allows separate parts to be run without needing to run the whole thing every time, meaning that it can be quicker to test certain parts. 

To run the whole thing, use the function run(). This function takes as a parameter the number to be used when determining the number of frequently used words - the number is between 0 and 1, the higher the number the more words are used. A higher number means the classifier should, in theory, be more accurate, but will create a much longer running time. 

The prepare() function prepares the Reuters dataset - it runs the preprocessing steps on it and outputs a data frame that has a list of articles, and for each article a count of frequently used words, and columns for each topic with TRUE or FALSE as the values for each of these columns depending on whether or not the article has that topic. 

classify() takes a data frame as the parameter (the one returned by prepare()) and attempts to run the classifiers on it. test() and measure() would be used to test the classifiers and measure the accuracy, but have not been updated since the previous problem sheet as I wasn’t able to get the classifier to work. 
