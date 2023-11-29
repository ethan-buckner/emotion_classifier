# Group 1 - Project 3, Identifying Emotion from Audio Data

## Table of Contents
- SRC:
  - This folder contains all of the source code for our project. This folder contains all code used to load and combine the  data as well as structure the final model for training.
- DATA:
  - This folder is where we store all datasets being used for this project.
- Figures:
  -  This folder contains exploratory plots looking into the distribution of data. 

## SRC
### Installing/ Building our code
- It is recommended to run the notebook files in an IDE that supports both Jupyter Notebooks and R markdown files such as Pycharm.
- These files use the 'tidyverse' and 'dplyr' R libraries and the json, re, pickle, numpy, pandas and sklearn Python libraries
- File paths may be incorrect on your machine, you are recommended to check all file paths before running.
  
### Notebook Files
| Notebook Name | Decription |
| -------- | -------- |


### Usage
- To use this model, first unpickle it. Then call the sklearn method predict(data) to get predictions.

## DATA
### Dataset Dictionary
NOTE: We are only using speech files that are in audio-only format. Therefore, these two indicators were removed from the data dictionary. If they were included, audio-only files are denoated by "03" and speech is indicated by "01".

| Column Name | Definition | 
| -------- | -------- |
| Audio | Wave encoding of the original, clean audio |
| Emotion | 01 = neutral, 02 = calm, 03 = happy, 04 = sad, 05 = angry, 06 = fearful, 07 = disgust, 08 = surprised |
| Emotional intensity | 01 = normal, 02 = strong (NOTE: There is no strong intensity for the 'neutral' emotion.) |
| Statement | 01 = "Kids are talking by the door", 02 = "Dogs are sitting by the door" |
| Repetition | 01 = 1st repetition, 02 = 2nd repetition |
| Actor |01 to 24. Odd numbered actors are male, even numbered actors are female |

## Figures
| Figure | Takeaways | 
| -------- | -------- |
|  ![Figure 1](Figures/P3-Confusion_Matrix.png) | This figure is a confusion matrix of our results of the classification model created for this project. As you can see, this model shows that we were able to accurately classify emotion 67% of the time for top one accuracy on the validation data by the last epoch. For the top two accuracy, we were able to predict emotion 81% of the time. |

## References
[1] S. R. Livingstone and F. A. Russo, "The Ryerson Audio-Visual Database of Emotional Speech and Song (RAVDESS): A dynamic, multimodal set of facial and vocal expressions in North American English," in PLoS ONE, vol. 13, no. 5, May 2018, Art. no. e0196391. doi: 10.1371/journal.pone.0196391.

### Previous Work
- MI-1: https://docs.google.com/document/d/18hC13QO4HtA7PaNARlzhyyeMSJZ7ZLVqHICdxkPT2h4/edit?usp=sharing
- MI-2: https://docs.google.com/document/d/1QfDnBwpLKD_atXqpSJ4NKJr6VZ0uZYJAn7gy7dUlSFQ/edit?usp=sharing

### Acknowledgements
We would like to thank Professor Alonzi and Harsh Anand for supporting us throughout this project. We greatly appreciate all of the feedback and guidance they have provided and owe part of our success in completing this assignment to them!
