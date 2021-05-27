# Description

Please check the README file to find an in depth overview of the project, as well as instructions on how to get everything set up locally. There are no frameworks or libraries necessary that deviate from our instruction and all necessary imports are found in the included pipfiles.

The roadmap for the release can be found here: https://www.notion.so/Roadmap-Human-Rights-First-Blue-Witness-Labs-34-b4f3e3ac33d042f8a6c228571d18671a
The DS-Flow Chart found in the root directory shows how the different aspects of the project work in conjunction with each other.

Here is a breakdown of the folders and their contents found in this repository:
    BERT-The folder containing the Google BERT model and the notebooks containing videos and documentation on how the model works and is implemented.
    Notebooks-A collection of notebooks from previous cohorts detailing their work and studies on the project
    App-Where the other functional components of the project reside and where most work will be done. This includes:
         create_db_tables.py-The file that creates the table when connected to the database
         db.py-The file that establishes connection to the database
         helper_funcs.py-The file that contains functions called throughout the rest of the application
         main.py-The file that establishes the application using FastAPI
         reddit.py-The file that returns reddit data
         scraper.py-The file that adds scraped data that has been ranked to the database
         textmatcher.py-The file that contains NLP text matching data (used for ranking purposes)
         training_data.py-The file containing the keywords used for classification of rank
         twitter.py-The file that returns twitter data

# Steps For The Future

Looking forward, there are some great opportunities to improve the work already found in this project. They include, but are not limited to:

Establishing functionality for the twitter scraper (aka Twitterbot) to respond to tweets that could be valuable to the project but require more information. Unfortunately, we were unable to establish a way to do so that fits the criteria of:
    1) Professional-Showcasing HRF in a positive light is of the utmost importance
    2) Concise-Twitter's character limit of 280 characters is a natural constraint
    3) Informative-Explaining why more information is necessary
    4) Compelling-Overcoming the natural human aversion to interacting with an unsolicited automated responses is a challenge
This would help to improve the quantity of applicable data to be catalogued.

Reducing the number of false positives in our data. This could present itself in more robust training data, fine tuning of the keywords used for ranking or through other means. This would help to improve the quality of applicable data to be catalogued.