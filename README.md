# GenIAinProjectmanagement

# Problem Statements

Consider the scenario where it would be time consuming for the project manager to **find a summary for all risks** for a portfolio, which spans over 200 projects and raised more than 600 risks in unstructured and free form text. This needs to be accounted for upcoming projects to be prepared better.
If we need to present summary of risks across the projects in portfolio, mining such volume of risk descriptions would again be a resource intensive task which could take considerable effort to summarise. 
Again, if we need to search for specific type of a risk(s) which impacted a technology among 600 risks, it would be a resource intensive task to find such summarised information.
Similarly, the use case applies for mining issues as well.
Now, consider a scenario where you need to present a summary of  ~600 Lessons learnt from 200 projects and identify meaningful actions which needs leadership attention. This would again become a resource intensive task to summarise such volume of lesson learned documented in unstructed free form text.
Next, consider you need to present the summary of reasons  projects were on RED or AMBER status during the year and identify the actions to prevent such situations. Again, mining such volume of information across projects and summarizing for them for corrective action would be resource intensive.
# Solution 
I used Generative AI, **huggingface transformer pre-trained models** which could reasonably summarise large volume of unstructured data written in natural language like risk description, lesson learnt description, Red RAG reason descriptions. This data could be in a tabular format in an Excel Workbook, database, in CSV or Microsoft Word files. 
I researched using the Python generative AI model to summarise unstructured free form risk data. The python code given below can summarise small chunks of paragraphs just the way we summarise our thoughts reading paragraphs and then consolidate the summarised information within say 100 to 200 words. This could be great time saving exercise to find meaningful information from a large volume of unstructured free form risk data.
I also researched using Python generative AI that if we could pass in a specific natural language question  like “what is the trouble with particular technology”,  we could return a summarised text which matches few of the risks documented based on that technology. 
So using a summarise model and a question answer model of mining project risk data, I was able to get meaningful information provided by generative AI which in reality could have been a labour intensive exercise.
I have provided the code in the section below where I have used an excel spreadsheet with the risk description data which was summarised by the code in chunks of 500 characters and produced an output within 100 to 200 characters using huggingface transformer python library. A pre-trained model gets downloaded from huggingface to your local machine and based on the processing ability of the model, we could get reasonably accurate summary. 
I have also provided the code in the section below where I could pass a question in natural language and obtain a relevant summarized answer. 
If we further develop a trained model and the summary will be accurate. An out of the box pre-trained model to start with a few lines of code you should be able to summarise to a good extent as I have experienced using the huggingface transformer library.This section describes the specific results (outcomes) that the business wants to achieve within a specific point in time.  
1.	I have attempted to load the risk description to summarise the risks and find meaning information about what risks were encountered across all projects for the entire year. 
1.	Now, the same code can be repurposed as is to summarise the risk mitigations across risks in all projects across the entire financial year.
1.	Again, the same code can be repurposed to summarise the issues as above.
1.	I could pass in a specific natural language question  like “what is the trouble with particular technology”,  and return a summarised text which matches few of the risks documented based on that technology.
All of the above information empowers the organisation to take meaningful actions to minimise the impact of such risks or even eliminate the chances of  such risk in future projects.

# Step 1 – load the Python libraries

**pip install transformers** – This will install the huggingface transformer library
**pip install sentencepiece**
# Step 2 - Load the data file from Excel | Word | CSV
# Step 3 - Use Hugging Face Python Transformer Library for summarisation


