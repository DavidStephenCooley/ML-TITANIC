# ML-TITANIC

This repository contains Titanic passenger data for machine-learning project

## Files

- `Titanic-Dataset.csv` - the extracted dataset.
- `archive.zip` - the original archive containing the dataset.
- `TitanicModel.ipynb` - the Notebook containing information and source code that loads the data and runs models + evaluations
- `requirements.txt` - the requirements file

## Insturctions (windows)

Create python venv running version specified in environment table

- py -3.12 -m venv .venv
  install requirements from requirements.txt to this venv
  .\.venv\Scripts\python.exe -m pip install -r requirements.txt

Set python kernel to venv kernal
Run each block of code in notebook in order

## AI disclosure

My entire chat history with claude is present in the prompts.txt file.
I mainly used claude for validation of my ideas both prior to implementation and post implementation. Usually framed as "I am thinking of doing X do you see an issue" or "I have implemented Y do you see any problems" in this way claude acts as a second set of eyes on major design decisions.

Additionally claude created code snippits which I based my notebook design off, but I ensure that I understand each and every line in context.

Overall Claude is a great help for finding things I may have missed such as ticket number being a shared asset among groups (I was fully expecting to drop this column prior to this being pointed out) which massively helps with my Parch SibSp problem. I will tackle this further in the next few milestones. However, Claude suffers from an knowledge gap in that it often over complicates the current requirements such as in saying "Your logistic regression scores 0.800 and the sex rule scores 0.787. That 1.3-point gap is well within your fold spread of ±0.022, so the notebook doesn’t yet show the model is better than that one rule. Your markdown’s “clear headroom for improvement” isn’t supported either." this milestone is more about building a baseline so comments around my test code not beating the baseline are ill placed.
