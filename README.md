# Twitter Sentiment Analysis using Azure

Azure Logic Apps is a cloud service. Using Logic Apps defines the workflow at ease consuming a range of APIs exposed as Connectors. These Logic App connectors will perform the sequence of actions defined in the workflow whenever the trigger gets fired.


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

