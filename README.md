# Twitter_Analytics1
Analysis on how twitter affect High School Students
from textblob import textblob
import system, tweepy
import matplotlib
def % (part, whole):
return 100* float(part)/float(whole)


consumerKey= ""
consumerSecret= ""
accessTokenKey= ""
accessTokenSecret= ""

auth = tweepy.OAuthHandler(consumer_key = consumerKey, consumer_secret = consumerSecret)
auth.set_access_token(accessToken, accessTokenSecret)
API = tweepy.API(auth)
search_term = input("Inser the Keyword to search: ")

NoOfSearchTerms = input (input("insert total tweets to analyse:"))
tweets = tweepy.Cursor( api.search, r=SearchTerm, lang = "Enl").items(noOfsearchTerms)
positive = 0
negative = 0
neutral =0
for tweet in tweets;
analysis = textblob(tweet.text)
results += analysis.sentiments.results
print (tweet.text)

 if (twitterAanlysis.sentiment.positive<0.00>):
 positive +=1
elif (twitterAanlysis.sentiment.negative<0.00>):
negative +=1
elif (twitterAanlysis.sentiment.neutral<0.00>):
neutral +=1
elif (twitterAanlysis.sentiment.results<0.00>):
results +=1

positive = % (positive, noOfSearchTerms)
negative = % (negative, noOfSearchTerms)
neutral = % (neutral, noOfSearchTerms)
results = % (results, noOfSearchTerms)

positive = format(positive,'.2f')
negative = format(negative,'.2f')
neutral = format(neutral,'.2f')
results = format(results,'.2f')


print ("effect of twitter on students" +searchTerm+ "analyzing" +str(noOfsearchTerms)+ "tweets posts")
if (positive == 0)
print( "no effect")
elif(polarity <0):
print("negatively affected")
elif(result>0):
print(possitively affected")

labels = ["positive['+str(positive)+'%]',neutral['+str(neutral)+'%', 'negative['+str(negative)+'%]']
sizes=[positive, neutral, negative]
colors =['green', 'gold', 'red']
patches, texts =plt.pie(sizes, colors=colors, starangle ==90)
plt.legend(patches, labels,loc="good")
plt.header("what are the effects of twitter on students" + searchTerm+' "analyzing"+str(noOfsearchTerms)+' tweets post,')
plt.axist('same')
plt.tight_layout()
plt.show()

DataSet = create dataset(search_term)
print(tweepy_api.VerifyCredentials())
def create dataset(search_keyword):
    try:
        tweets_fetched = tweepy_api.GetSearch(search_keyword, count=80)
        print("Fetched " + str(len(tweets_fetched)) + " tweets for the term " + search_keyword)
    except:
        print("something is wrong..")
        return None
    
        
        
