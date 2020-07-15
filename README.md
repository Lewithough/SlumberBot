# SlumberBot
In the .zip slumberbot there is a python backend for the SlumberBot project. I used this backend to hardly control the chatbot conversation. The chatbot is built in Google Dialogflow and intergrated into the Facebook Messenger.


## Main Functions
Connecting to the Google Dialogflow platform through webhook, this backend can:
1. read users' everyday Fitbit data
2. read users' replies to the chatbot
3. know users' position in the conversation flow
4. trigger the corresponding chatbot questions
5. save users' replies in Data Foundry for further use

You may found these functions in the main code "app.py". Some parts of the codes (e.x. participants unique Facebook ID) were anonymised. Here are some tutorials that I referred to when building this backend:
1. Collect Fitbit data with python: https://towardsdatascience.com/collect-your-own-fitbit-data-with-python-ff145fa10873
2. Python webhook to Dialogflow: https://medium.com/analytics-vidhya/dialogflow-chatbot-with-webhooks-using-python-c1e7fc46faf6
3. Another tutorial for Python webhook to Dialogflow: https://chatbotslife.com/api-ai-lets-create-a-movie-chatbot-in-minutes-f68d8bb568f9


## Virtual Environment
This code should run under a virtual environment with all libs installed (read requirements.txt). You can do this by typing these commands in your commandline:
1. cd (path of the document)
2. python3 -m venv env
3. source env/bin/activate
4. pip install -r requirements.txt (you only need to do this for one time.)
Then you can run the code by typing "flask run".


## Ngrok
To publish your local environment to the public for webhook, you can try ngrok. You may find a clear tutorial here: https://medium.com/@antonyharfield/dialogflow-web-hooks-how-to-develop-locally-and-deploy-to-cloud-functions-48839919e998

# Others
## Dialogflow Codes
In .zip Dialogflow there are all the intent used in this chatbot. I downloaded them as JSON file for further use.

## Web Report
The web report is a web page that provided to the users at the end of the chatbot conversation. I wrote some javascript codes to read the data from Data Foundry and visualize the data.

