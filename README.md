# Twitter_API_week6
## Twitter Introduction
This assignment teaches me how to interact with twitter API. I also learned and get used to with twitter developer account.
first I created that account and generate some API keys then I've stored it for future purposes.This assignmnet is about posting new tweet and deleting the tweet with authentication and app permissions.
## Setup Instructions
 Step1: I've created twitter developer account with email credentials.
 Step2: Then I,ve generated API including client Id and token seceret and save it for referenece.
 Step3: After that, I've set environment variables so that no one can access my seceret token. 
 Step4: I wrote logic for posting new tweet and deleting the tweet.
 Step5: I ran the program and faced so much errors.
## Progaram Details
I created two functions with posting tweet and deleteing tweet.then, I wrote code for setting environment variables and wrote code for OAuth1 setup.After that, set headers and created http requests also wrote logic for reading response body.
for delete the tweet, I defined tweetid and sent the request for delete the tweet.I created multiple tweets and delete one specific tweet with Id.
In main function, I called the both function and ran for loop for posting tweets.
Example of API requests: POST https://api.x.com/2/tweets
{
  "text": "Hello from the Twitter API!"
}
## Error Handling
I faced too many errors by running the program. I faced errors like 401 unautorized access, then I checked OAuth1 setup documentation on twitter then wrote code according to that.
I also got 403 forbidden error and got to know that twitter doesn't allow same content while posting new tweets.
error was like this: Posting tweet: Hey There!
Error with posting your tweet: failed to post your tweet%!(EXTRA int=403, string=Forbidden, []uint8=[123 34 100 101 116 97 105 108 34 58 34 89 111 117 32 97 114 101 32 110 111 116 32 97 108 108 111 119 101 100 32 116 111 32 99 114 101 97 116 101 32 97 32 84 119 101 101 116 32 119 105 116 104 32 100 117 112 108 105 99 97 116 101 32 99 111 110 116 101 110 116 46 34 44 34 116 121 112 101 34 58 34 97 98 111 117 116 58 98 108 97 110 107 34 44 34 116 105 116 108 101 34 58 34 70 111 114 98 105 100 100 101 110 34 44 34 115 116 97 116 117 115 34 58 52 48 51 125])
Posting tweet: How are You All
Error with posting your tweet: failed to post your tweet%!(EXTRA int=403, string=Forbidden, []uint8=[123 34 100 101 116 97 105 108 34 58 34 89 111 117 32 97 114 101 32 110 111 116 32 97 108 108 111 119 101 100 32 116 111 32 99 114 101 97 116 101 32 97 32 84 119 101 101 116 32 119 105 116 104 32 100 117 112 108 105 99 97 116 101 32 99 111 110 116 101 110 116 46 34 44 34 116 121 112 101 34 58 34 97 98 111 117 116 58 98 108 97 110 107 34 44 34 116 105 116 108 101 34 58 34 70 111 114 98 105 100 100 101 110 34 44 34 115 116 97 116 117 115 34 58 52 48 51 125])
Posting tweet: Hetvi Paaatelll
I alos got 400 bad request error many times and didn't find problem intially.Then I checked https://developer.x.com/en/support/x-api/error-troubleshooting#invalid-request website for finding the error and resolved it.
