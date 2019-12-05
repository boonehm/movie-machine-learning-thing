# movie-machine-learning-thing

IMdB project for machine learning.

# Contact information

Sam Knight

Justin Reel

Christopher Wilson

Data Source - https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset

# Introduction

When we were coming up with an idea for a project, we wanted to take on something that would be more “fun” and enjoyable. We weren’t really pursuing anything that would change the world because we wanted to use our knowledge in a way that didn’t require non-stop google searches for concepts that we didn’t understand. So we resorted to a topic that we all love: movies! 
The idea of our system is to take in a set of actors, a director, and some other data and out put the set of words that would represent the plot line of the movie. The dataset we chose has a column, plot_keywords, that exemplify this idea. For example, on a row representing Harry Potter, the plot_keywords column might say “wizards|magic|Dumbledore|fantasy”. We wanted to predict something similar to this column in a light-hearted manner!
The dataset we chose was a list of 5000 movies with columns describing some of the attributes of the film, the genre of the film, its budget, information on the actors and director, and more. A lot of the information was discarded as it added too much complication than was worth taking on for this simple of an idea.

# Data Preparation

This dataset was really fun to preprocess. Because of the format of the target column (plot_keywords) and the genre column, there was a need to parse the strings held therein and split them into separate words. This then caused the need to create new columns where those columns had only one target. Because of the nature of this task, we moved our data size from roughly 4800 usable rows to about 701000 usable rows. 
This was not a difficult task, conceptually, but the original two designs took roughly 30 minutes to create the necessary rows. This wasn’t acceptable because we really needed to work with this data regularly and we wanted it to be more readily usable. To solve this conundrum, we had to read in the data to a python data frame. Then, we iterated through all of the rows with iterrow(). We then copied all of the data to a new primitive-style array (this was the key to efficiency). A standard array takes up much less space than a new Pandas Dataframe, Sries, or Numpy array object so it was much faster to instantiate 701000 new rows. 
# Mining / learning from the data

o Describe the process you used to mine the data, or learn patterns from it. What algorithms did you try, why did you try them? What parameters did you use and why?

o Make sure to discuss different things you tried along the way, even if they resulted in dead ends.

o Highlight challenges you faced and how you overcame them.

# Results

o Present the results that you obtained from the work done in the previous sections.

o Include graphs and charts to support your findings. (Don't forget to include proper titles, axis labels, etc. for all graphs)
Conclusions (including business takeaways and action items)

o Describe why your results could be of value to a business or stakeholder in your area. What would they know or what could they do differently as a result of your work.

o Explain why your results constitute something "interesting."

o Don't forget to discuss potential limitations or ethical issues.

# Lessons Learned

o What did you learn from this project?

o What would you do differently if you could start this project again?

