# pandas-challenge

# Overall, this assignment when pretty well with the exception of two minor roadblocks

# The first problem I encountered was finding a method by which to calculate the per-capita spending of each school using total budget and total number of students. I ended creating a new column within the school_data_complete dataframe.

# The second hurdle was overcoming the fact that the data type for the calculations of certain variables (per_school_budget, per_school_capita) came out as 'object' instead of 'int64'. This turned out to be the result of my use of the .unique() funtion. On the advice of one of the fine individuals in our class slack chat, I ran the same code using the .first() function and all was solved. 

# The reason for this difference was made clear to me upon learning that because the .unique() function returns data as an array, it connot contain multiple data types and therefore defaults to the most general data type when multiple data types appear (at least in Pandas).
