# Intership-Suvidha-Foudation
Contain work done at Suvidha foundation as an Intern ; Data Preparation, learning about Pegasus, Bert etc. applying then on a CNN datatset to create a summarization model
## In This one Month long Intership I performed 3 Major tasks:-(This is about Data Preparation Task) 
Data preparation- Extract data from Times of India website (Date, Headline, Article), process them using an LLMs and submit the results in a google form.
 we were asked to manually submit this info 1000 times but since it was cumbersome i designed a web scraper that does the job for me.
 I have divided my task into 3 parts:-
 1) Extract Data from Times of India Archives.
 2) Send relevant extracted data to an LLM in this case Gemini using an API with custom prompt. Restructure the Response check if it doesnot contain any errors.
 3) Upload final information to a google form.<br>
<br>
On this Endevour the language of choice is python using libraries like Selenium and google genai library.<br>
To perform the first task:-<br>
I searched for patterns in Times of India Article Page and i found one : If I have a link to an article i can change the word : "articleshow" to "articleshowprint" to get data into a much nicer format free of any ads and excess junk making it easier to extract info.<br>
Then use of Selenium Library to extract info using Xpaths of the generated html page those Xpaths were consistent in all articles.<br>
To Perform the second task :-<br>
I generated an API key from ai.dev.com to use gemini model with an api and automate it via my code.<br>
used a custom prompt to generate summary of provided article and get which topic it belongs to also since gemini tended to hallucinate in response i also added a check using semaphore in this step.<br>
To perforn the third task:-<br>
I used Selenium once again to access the google form and use xpath of various field to input information and click submit this was looped a thousand times.<br>

For Testing and Replication purposes i have recreated the form you can make a copy of the form on your device and use as you see fit i have also provided the code to do the same.\n

