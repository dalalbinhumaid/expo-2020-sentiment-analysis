# Expo 2020 Sentiment Analysis
 
## Introduction
The aim of this project is to conduct a sentiment analysis using python and twitter's API. The project is approached through five phases which are analogous to the data analytics life cycle.The following is a brief introduction to the topic

### What is Expo 2020?
> Initiated in London 1851. It is a global gathering aimed to find solutions to challenges imposed by the current times. Aims  to create enriching and immersive experience. World expo traverses through different cities each time. It also revolves around certain themes. Currently, World expo is taking place in Dubai, UAE. Between Oct, 2021 and Mar, 2022. For more information please visit [expo2020dubai](https://www.expo2020dubai.com/)

### Project Goal
> As discussed above the main goal is to conduct a sentiment analysis and learn the basics of data science and big data projects. Since Expo 2020 is considered an educational exhibition that revolves around modern day problems and is hosted currently in the middle east. The goal is to measure the awareness of the arab society - *By arab society we mean anyone who posts their opinions in arabic* and their view on Expo 2020

## Project Structure
### Phase One: Discovery
This part is about discovering and collecting as much data as possible that is relating to the topic at hand. I will be needing tweets that are written in Arabic. This phase is in [`tweets-collection.ipynb`](tweets-collection.ipynb) notebook. The phase's documentation can be found [here](Docs/Group8_SWE486.pdf).

### Phase Two: Pre-processing
In this phase we first explore the dataset in detail and then we clean and preform pre-processing techniques. This phase can be found in the [`tweets-cleaning.ipynb`](tweets-cleaning.ipynb) notebook. 

### Phase Three: Data Analysis and Model Building
Here we conduct a statistical analysis and observe the general characteristics and distribution of the dataset which is provided in this notebook [`tweets-statistics.ipynb`](tweets-statistics.ipynb). Then, we move on to model building and we perform a sentiment analysis by evaluating three different models and fine-tune the best one. But prior to starting the analysis phase we need our dataset to be classified. Thus, we used mazajak's API to do so, the code can be found here [`tweets_labeling.ipynb`](tweets-labeling.ipynb). The model building notebook can be found here [`tweets-analysis.ipynb`](tweets-analysis.ipynb) and the documentation can be found [here](Docs/SWE486_Phase3_Group8.pdf)

### Phase Four: Findings
We finally link our results back to our initial hypothesis and summarize our findings in this notebook [`tweets-visualization.ipynb`](tweets-visualization.ipynb).

### Phase Five: Presentation
The following is the final course presentation [expo_2020_presentation](https://www.canva.com/design/DAFA2NMvgSU/fbhKPCGXxeDi2ssdvM6oZw/view?utm_content=DAFA2NMvgSU&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink)

## Data Dictionary 
In the [`Tweets`](Tweets/) folder you can find all the dataset used and preprocessed according to each phase. The following table summarizes each file. 

| File                                                                        |                                                                Description                                                                |
| :-------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------: |
| [`Excel/tweets.xlsx`](Tweets/Excel/tweets.xlsx)                             |                    The full dataset of collected tweets. You will find **7767** entries. Converted to an excel sheet.                     |
| [`Excel/dirty_tweets_updated.xlsx`](Tweets/Excel/dirty_tweets_updated.xlsx) |                  The dataset before preforming any preprocessing techniques. You will find a total of **14837** entries.                  |
| [`Excel/final_tweets_cleaned.xlsx`](Tweets/Excel/final_tweets_cleaned.xlsx) |                           The full dataset of cleaned and preprocessed tweets. You will find **7975** entries.                            |
| [`Excel/tweets_classified.xlsx`](Tweets/Excel/tweets_classified.xlsx)       |                                                            Classified dataset                                                             |
| [`tweets[x].xlsx`](Tweets/tweets1.csv)                                      | Where x is any random integer. This the dataset pulled from twitter's API. Each pull generate a new file with a random number at the end. |
| [`tweets.xlsx`](Tweets/tweets.csv)                                          |                                              All the pulled raw tweets combined in one file.                                              |
| [`dirty_tweets_updated.csv`](Tweets/dirty_tweets_updated.csv)               |                  The dataset before preforming any preprocessing techniques. You will find a total of **14837** entries.                  |
| [`final_tweets_cleaned.csv`](Tweets/final_tweets_cleaned.csv)               |                           The full dataset of cleaned and preprocessed tweets. You will find **7975** entries.                            |
| [`tweets_classified.csv`](Tweets/tweets_classified.csv)                     |                                              The classified dataset by using `Mazajak API `                                               |
| [`final_tweets_classified.csv`](Tweets/final_tweets_classified.csv)         |                                              The manually classified dataset in .csv format                                               |

