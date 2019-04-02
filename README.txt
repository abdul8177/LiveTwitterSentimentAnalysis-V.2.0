Live Twitter Sentiment Analysis - Dash Application
This is the second version of my Live-streaming sentiment analysis application .
It is created using Python and Dash.



Repo Contents:

    • DashLayout.py - This is currently the main front-end application code. Contains the dash application layouts, logic for graphs, interfaces with the database...etc. 
    • TwitterAnalysis.py - This should run in the background of your application. This is what streams tweets from Twitter, storing them into the sqlite database, which is what the DashLayout.py file interfaces with.
    • requirements.txt - Contains all the libraries required for the project.
    • error.txt - maps the errors and notes them. (if any)

Quick start:

    • Clone repo
    • install requirements.txt using pip install -r requirements.txt
    • Fill in your Twitter App credentials to TwitterAnalysis.py. Go to apps.twitter.com to set that up if you need to.
    • Run TwitterAnalysis.py to build database
    • If you're using this locally, you can run the application with the dev_server.py script. If you want to deploy this to a webserver, see my deploying Dash application tutorial
    • You might need the latest version of sqlite.

Todo List:

    • Improve the layout so that multiple analysis can be shown at a time for different topics.
    • Host the application to web server using dash.
    • Create a system so that the database automatically truncates after certain size limit is reached.
    • Improve the front end UI of the web server .
    • Add suggested tweet topics section pulled from the trending section.
