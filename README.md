# twitter-readability
Does Trump Tweet Like a Fifth Grader? An Analysis

Assuming you have experience with Git and cURL (or Postman, or whatever to retrieve API responses):
1. Clone the repo
2. Sign in with [dev.twitter.com](https://dev.twitter.com) and create the required authentication objects to authenticate with OAuth 1.0a
3. Request a user's Tweets with your application, in JSON form (I use Postman)
4. Save the Tweets to the same folder as index.html
5. Edit line 487 of index.html: you are looking for fetch('trump.json') and will replace it with fetch('{NEW-SAVED-TWEETS-FILENAME}.json')
6. Serve index.html (well, really, the entire folder) (I recommend browser-sync)
7. You will note that most of the content is hard-coded; however, the mean, standard deviation, IQR, 5 number summary, histogram, and calculations are live and will change. When in doubt, read the code and look for variables. They were somewhat well named.

To add to the spaghetti at the bottom of the page:
1. Retrieve the mean and standard deviations of the {NEW-SAVED-TWEETS-FILENAME}
2. Add to the array beginning on line 637 of index.html
