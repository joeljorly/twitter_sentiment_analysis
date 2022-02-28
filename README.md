# Twitter Sentiment Analysis using Azure

Azure Logic Apps is a cloud service. Using Logic Apps defines the workflow at ease consuming a range of APIs exposed as Connectors. These Logic App connectors will perform the sequence of actions defined in the workflow whenever the trigger gets fired.


# ms-latd-livedemo-backend

This is the backend of the Logic App Twitter Demo, it does the following:
* logic app twitter trigger - when new tweet is posted (certain hashtags) 
* logic app detect sentiment - text recognition api, 1 positive 0 negative
* logic app post to backend
* backend (this stuff) gets the message and publish it to topic on redis

When starting this docker instance you need to provide the following parameters
* process.env.REDIS_URL
* process.env.REDIS_PASSWORD
* process.env.REDIS_TOPIC

You can start this instance with the following command:
* docker run -d -p 3000:3000 -e REDIS_URL="[YOU REDIS URL]" -e REDIS_PASSWORD="[YOUR REDIS KEY]" -e REDIS_TOPIC="[YOUR REDIS TOPICNAME]" REPO/NAME_OF_YOUR_DOCKERIMAGE

It will start with the following command: swagger project start


## Prerequisites required:
1. Need a twitter account
2. Create an app https://developer.twitter.com/en/apps, from where you can generate credentials like ACCESS_TOKEN,ACCESS_TOKEN_SECRET,CONSUMER_KEY,CONSUMER_SECRET


## Deployment In Heroku:
You just have to create an account in Heroku, connect your github repository with it that you wish to create a server for.

Create two additional things before you deploy in heroku-
 - Create a profile which you can view in this repository , in which you will need to add your app name which in my case it is Twitter_app and the other thing is you need to specify the name of flask object that you have created. In my case, For example: Twitter_app : app, my "app" is the flask object which is created.
 - Requiremnts file where you have to specify all the libraries that you have imported , along with its versions. The same can be found in this repository. If you want to know the version installed in your ,machine of differnt libraries, open your anaconda prompt and just type.
 
            
            pip Freeze

This project can be viewed at https://twittersentimentanalysis-app.herokuapp.com/

