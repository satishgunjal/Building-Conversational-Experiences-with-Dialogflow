# Building Conversational Experiences with Dialogflow
* This course provides a deep dive into how to create a chatbot using Dialogflow, augment it with Cloud Natural Language API, and operationalize it using Google Cloud tools.
* [Coursera Link](https://www.coursera.org/learn/conversational-experiences-dialogflow/)

# Course Slides
* [Course Intro](course_slides/0_%20Course%20Intro.pdf)
* [Building Conversational Experiences with Dialogflow](course_slides/1_%20Building%20Conversational%20Experiences%20with%20Dialogflow.pdf)
* [Defining Intents and Entities](course_slides/2_%20Defining%20Intents%20and%20Entities.pdf)
* [Maintaining Context and Taking Action](course_slides/3_%20Maintaining%20Context%20and%20Taking%20Action.pdf)
* [Taking your Chatbot to Production](course_slides/4_%20Taking%20your%20Chatbot%20to%20Production.pdf)
* [Additional Functionality](course_slides/5_%20Additional%20Functionality.pdf)
* [Summary](course_slides/6_%20Summary.pdf)

# Week 1
* Graded Quiz
  - [About Dialogflow](/images/Graded_Quiz_About_Dialogflow.png)
* Qwiklabs- Define intents and entities for your pizza ordering conversational agent
  - Build a conversational agent for a fictional pizza shop that will let users place orders
  - Define intents for a pizza-ordering use case to match typical user queries
  - Identify entities to extract data from user queries
  - [Agent source](qwiklabs/PizzaBot_Lab1.zip)
* Graded Quiz
  - [Intents and Entities](/images/Graded_Quiz_Intents_and_Entities.png)
* Qwiklabs – Setup fulfilment and adding context for your pizza ordering agent
  - Add input and output context to the order.pizza intent to maintain continuity
  - Setup fulfilment as Cloud Functions code for the agent to be able to store orders in Datastore
  - [Agent source](qwiklabs/PizzaBot_Lab2.zip)
  - [Function source](qwiklabs/function-source_Lab2.zip)
* Graded Quiz
  - [Context and Fulfillment](/images/Graded_Quiz_Context_and_Fulfillment.png)
  
# Week 2
* Qwiklabs – HR Chatbot : Setup knowledge base for your agent in Cloud Datastore
  - Use Cloud Datalab, Python, data science libraries, and Google Natural Language API machine learning technology to transform an unstructured text document into a structured knowledge base in Cloud Datastore
  - Use Dialogflow to build a conversational agent that can respond to questions about the HR manual
  - Populate entities from Datastore into your Dialogflow agent
  - [Agent source](qwiklabs/HR_ChatBot_Lab3.zip)
  - Pre-Processing Notebooks
    Let's first review the purpose of each of the notebooks. They are used to extract information from the HR Manual and create a knowledge base that is used by the chatbot to answer questions. Each of them will be run one time in the order listed here:
    - [ProcessHandbook.ipynb](qwiklabs/ProcessHandbook_Lab3.ipynb) performs "semi-structured" analysis on the HR Manual text file. It alternately extracts topic "headings" and associated "policy text" from the file and stores these as key-value pairs in Cloud Datastore to give the chatbot a basic vocabulary.
    - [ProcessSynonyms.ipynb](qwiklabs/ProcessSynonyms_Lab3.ipynb) uses several Python data science libraries and the Cloud Natural Language API to generate synonyms for topics, which gives the chatbot an expanded vocabulary.
    - [DialogFlow.ipynb](qwiklabs/DialogFlow_Lab3.ipynb) uses Dialogflow's "Entity" API to write the topics to Dialogflow's Entity module, which makes these words available to the chatbot as a data type.
  
