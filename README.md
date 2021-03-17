# Source Code Monitor

This code is designed to notify you of code changes that may affect SEO, Google Analytics tracking, or any other reason you'd want to keep an eye on the code behind a site. It creates a new source code file for each page every day. The file from two days ago gets delete so you'll only have today's and yesterday's file at any given point. 

Create a Google Sheet containing the URLs you want to monitor and drop them in column A. Make that sheet shareable to anyone with link, and add that link to the code. 

Any comments in ALL CAPS also require your own input for email credentials, site structure, etc. One critical variable to pay attention to is the line skipper list titled 'words' at line 83; this allows you to specify lines containing strings in the source code that you don't want to compare, for example Akamai creates a unique ID in the source code every single time a page renders, so it would always return a 'no match' in that case. 

It's recommended that you set this up to run in Task Scheduler (or similar automation method). 
