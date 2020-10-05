# EC601_Project2

* Introduction

In this project, the student are going to be trained to use Twitter API and Google Cloud Platform to be familiar with API concept.

Google Cloud Platform, offered by Google，is a suite of cloud computing services that runs on the same infrastructure that Google uses internally for its end-user products, such as Google Search, Gmail, file storage, and YouTube. Besides, it also provides a series of modular cloud service including computing, data storage, data analytics and machine learning. Google Cloud API is the key element of this project. It ensure the developers implement the power of everything from storage access to machine-learning based image analytics to their Cloud Platform applications. To start a project, there are many google tutorial docs so that the developer can read and follow to get a quikstart of their project.  

## Phase 1 (a) Twitter API

Running the tweetexample.py, the code output a json file. The code could get the most recent 3240 tweets and save them in the json file. 

## Phase 1 (b) Google NLP

In this case, we are focus on the sentiment analysis, which requires Natual Language API. The Google Cloud Platform reconmaned to use the Cloud Natual Language with providing client libraries. 

Firstly, the users need to install the client library. The users can choose different language development environment such as C, Go, Java, Node.js, PHP, Python, and Ruby. In this case, I choose to use Pyhton. Then the client library can be installed using pip: 

pip install --upgrade google-cloud-language

Second step is to set up authentication. the developers are required to set up authentication by creating a service account and setting an environment variable to run the client library. Follow the instruction, the developer can creat a service account key which is a JSON file downloads to local computer.

Thirdly, the user need to provide authentication creadentials to the applicaition code by setting the environment variable GOOGLE_APPLICATION_CREDENTIALS using:
export GOOGLE_APPLICATION_CREDENTIALS="/home/user/Downloads/my-key.json"

After the three step finished, the user may creat their python file and develope the code. 

Sentiment Analysis inspects the given text and identifies the prevailing emotional opinion within the text, especially to determine a writer's attitude as positive, negative, or neutral. Sentiment analysis is performed through the analyzeSentiment method.

In the code, there are score and magnitude. Sore is the score of the sentiment range from -1.0(very negative) to 1.0(very positive). Magnitude is the strength of sentiment and ranges from 0 to infinity.

In the begining of the code, it import the Google Natural Language library.

<img width="300" alt="Screen Shot 2020-09-28 at 9 49 33 PM" src="https://user-images.githubusercontent.com/70667153/94480616-23972000-0209-11eb-97d1-03eddf8fee6b.png">

In this code, the text to analyze was 'Hello, world". Then, the code detects the sentiment of the text by  

sentiment = client.analyze_sentiment(document=document).document_sentiment, which output the sentiment score and magnitude as the figure shows.

<img width="430" alt="Screen Shot 2020-10-05 at 10 00 08 PM" src="https://user-images.githubusercontent.com/70667153/95090125-7e73ce80-0757-11eb-9cd4-43cdb7485c69.png">

## Phase 2 Build your own social media analyzer

* User stories
** As a product owner, I want to know how people like or dislike about the product in social media such as Twitter.

* Define MVP 

* Translate user stories to a modular design
* Who is your user?
* What are the basic user stories?






