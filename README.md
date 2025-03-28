# Lecure 8 - CLASS ASSIGNMENT - GROUP WORK

Hi, this is our last lecture and today, you will work with Human evaluation of the LLM models. With Eskil we designed longer exercise, and first, you will be split in different groups. 

## OVERALL TASK

You are given an existing pipeline, which collects news articles from DR.DK about foreing news. You can access the news via API (**script: get_data_api.py**). As it stands, the script (ollama_call_translate.py) sends this articles to Ollama server (to custom model) and return articles translated in English. 

You will then exectue (**ollama_call.py**) four times, by changing the model (listed bellow). This will create 4 different reports. 

You will print out the reports and design evaluation instructions, which will be handed in to next group. After receiving thier feedback, you as a group work together again and find out, which evaluation got the best results. It is important to define some Benchmark strategy, and based on the result you choose the best performing model. Provide a clear explanation why. 


## MICRO STEPS:

- one of the group member clone the Repo (and adds other members: SETTINGS -> GENERAL -> COLLABORATORS)

- review the whole Repository together, so you uderstand everything

- SIT down, put head together and design Evaluation strategy. Create different benchmark other group will use to review your products.

- RUN SCRIPTS ONE BY ONE. Some might take a bit longer... 
    -   Script one: **get_data_api.py** creates file **raw_articles.json** in /data/
    -   Script two: **ollama_call_translate.py** (might take a few minutes) creates file **translated_articles.json** in /data/
    -   Script three: (run 4 times) **ollama_call.py*** creates reports in /reports/

- Print reports and print your Evaluation instructions, and give them to the "partner" group's reports 

- When you receive back your reports and evaluations, review results and decide which model to use! Write clear explanation. 



## List of available models
/work 
[ 11:01:54 ] ➜  ollama list
NAME               ID              SIZE      MODIFIED          
gemma3:1b          8648f39daa8f    815 MB    24 hours ago         
gemma3:4b          a2af6cc3eb7f    3.3 GB    24 hours ago         
gemma3:27b         a418f5838eaf    17 GB     24 hours ago         
gemma3:12b         f4031aab637d    8.1 GB    24 hours ago         


# Backup

In case that something goes wrong with any of the server, there will be folder **BACKUP** with reports for each group. 