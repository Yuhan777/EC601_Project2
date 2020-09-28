# EC601_Project2

In this project, the student are going to be trained to use Twitter API and Google Cloud Platform to be familiar with API concept.

Google Cloud Platform, offered by Google，is a suite of cloud computing services that runs on the same infrastructure that Google uses internally for its end-user products, such as Google Search, Gmail, file storage, and YouTube. Besides, it also provides a series of modular cloud service including computing, data storage, data analytics and machine learning. Google Cloud API is the key element of this project. It ensure the developers implement the power of everything from storage access to machine-learning based image analytics to their Cloud Platform applications. To start a project, there are many google tutorial docs so that the developer can read and follow to get a quikstart of their project. 

In this case, we are focus on the sentiment analysis, which requires Natual Language API. The Google Cloud Platform reconmaned to use the Cloud Natual Language with providing client libraries. 

Firstly, the users need to install the client library. The users can choose different language development environment such as C, Go, Java, Node.js, PHP, Python, and Ruby. In this case, I choose to use Pyhton. Then the client library can be installed using pip: 
#pip install --upgrade google-cloud-language
Second step is to set up authentication. the developers are required to set up authentication by creating a service account and setting an environment variable to run the client library. Follow the instruction, the developer can creat a service account key which is a JSON file downloads to local computer.
Thirdly, the user need to provide authentication creadentials to the applicaition code by setting the environment variable GOOGLE_APPLICATION_CREDENTIALS using:
export GOOGLE_APPLICATION_CREDENTIALS="/home/user/Downloads/my-key.json"
After the three step finished, the user may creat their python file and develope the code. 

Sentiment Analysis inspects the given text and identifies the prevailing emotional opinion within the text, especially to determine a writer's attitude as positive, negative, or neutral. Sentiment analysis is performed through the analyzeSentiment method. 
