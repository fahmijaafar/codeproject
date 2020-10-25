# codeproject

HOW TO INSTALL AND RUN

1. Download the files and open using any web browser(Please! dont use mobile).
2. insert topic and/or language in their respective input box to start searching the repositories.
3. I've also included the file on my website at https://fahmijaafar.com/github to save your time.

COMPROMISES

- I've decided to include simple admin report for the test which is only for front end, due to time contraint.
But, I may be able to explain on how I'd probably done it.
1. create dependencies to mySQL, add a log table
2. for every button clicking on the search, php script will run POST method of the input and store in the database.
3. Admin can get report from the log table, which contains the search query and the result should be the same if were to put the input into the API's url.
4. As an example, if the log table have 2 column SearchTopic and SearchLanguage, one user input Ruby as a topic and left the language blank.
5. Then, the result will certainly return data from https://api.github.com/search/repositories?q=topic:ruby
