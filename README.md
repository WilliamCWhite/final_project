# Overview
With this project, I wanted to determine how variables relating to a students' AI use were important for determining how a student perceives their AI usage to impact their grade. I wanted to go beyond simply finding correlation coefficients, especially because they were super insignificant for my dataset. I decided to train machine learning models to predict the perceived grade impact, and then use SHAP analysis to see how each variable impacted the predicitons. In the end, I found that students with less extreme grade impacts were far easier to predict. A student's use cases for AI weren't very important, but a student's major and daily usage was, although directionality wasn't super consistent. The most consistent factor was whether professors allowed AI usage; if yes, students generally perceived it to have a better impact on their grades.

# Replication Instructions
If you do not already have the setup outlined in lab00 of this course, follow the instructions below. Otherwise, skip to Opening the Project.
## Setup from Lab00
You will need Python 3 and a bunch of Python libraries. In particular, download and install Miniforge for your OS.
Clone this repository. CD into it in the terminal, and run the following command:
$ conda env create -f environment.yml

Next, activate the new environment:

$ conda activate ml

Now register the ml conda environment to Jupyter. From the Terminal (or Miniforge Prompt):

$ python3 -m ipykernel install --user --name=ml

If you do not do this, you must select the kernel in the “Kernel > Change kernel…” menu in Jupyter every time you open a notebook, so that the correct packages are loaded.

That’s it! You can now start Jupyter from Terminal (or Miniforge Prompt) using:

$ jupyter lab

## Opening Project
If you already had the installed dependencies, simply run the following commands:
$ conda activate ml
$ jupyter lab
Open "Real Final.ipynb". The other notebook has older, less refined experimentation with the data.
Restart the kernel if you want to train all the models I've set up for yourself, but note that it will take a while.

# Future Directions
I believe a different dataset that somehow tracks the concrete impact on a student's grades instead of the perceived impact would have more interesing and potentially more significant conclusions. Trying different methods on this problem would've been interesting too. If I had time, I would've wanted to see if I could generalize the students into similar groups and identify traits of those groups. I also think more professional SHAP analysis could be fruitful. However, the largest obstacle and largest stride for answering questions about this topic is better data (especially considering how late in the project I've started to suspect my dataset is generated).

# Contributions
I'm the only one who worked on this project, and here's what I believe the time contirbutions were:

4 hours - Data Preprocessing and Correlations:  (got caught up in some weird categorical variable correlation method in the deprecated notebook)

1 hours - Setting up Mean Models, Linear Regression, and Random Forests

2.5 hours - PyTorch FNN and hyperparameter tuning (left in deprecated notebook)

2 hours - Keras FNN and hyperparameter tuning (lots of overfitting reduction and long model training periods)

1 hour - Writing throughout jupyter notebook (in deprecated notebook)

1.5 hours - Initial poster

3.5 hours - Full refactor of project, with better performance metrics, designed around error analysis with many dataframes, much more coherent and articulate jupyter notebook descriptions

1 hour - Keras FNN hyperparameter experimentation

3 hours - programming, analyzing, creating visuals, and writing about SHAP for random forest models

1 hours - outlining many-epoch keras model and programming/writing SHAP for it

1 hour - cleaning up jupyter notebook and adding context

2 hours - Creating project poster

23.5 hours total



