# Data for 'What Makes Tweetorials Tick'

This repository contains the data associated with the paper 'What Makes Tweetorials Tick: How Experts Communicate Complex Topics on Twitter'. You can also browse the collected tweetorials on our website [TechTweets](http://language-play.com/tech-tweets/annotations).

If you use this data, please cite our paper:

**ACM Reference Format:**

Katy Ilonka Gero, Vivian Liu, Sarah Huang, Jennifer Lee, and Lydia B. Chilton. 2021. What Makes Tweetorials Tick: How Experts Communicate Complex Topics on Twitter. *Proc. ACM Hum.-Comput. Interact.* 5, CSCW2, Article 422 (October 2021), 26 pages. https://doi.org/10.1145/3479566


**Bibtex**

```
@article{10.1145/3479566,
	author = {Gero, Katy Ilonka and Liu, Vivian and Huang, Sarah and Lee, Jennifer and Chilton, Lydia B.},
	title = {What Makes Tweetorials Tick: How Experts Communicate Complex Topics on Twitter},
	year = {2021},
	issue_date = {October 2021},
	publisher = {Association for Computing Machinery},
	address = {New York, NY, USA},
	volume = {5},
	number = {CSCW2},
	url = {https://doi.org/10.1145/3479566},
	doi = {10.1145/3479566},
	journal = {Proc. ACM Hum.-Comput. Interact.},
	month = oct,
	articleno = {422},
	numpages = {26},
	keywords = {tweetorials, science writing, twitter, science communication, social media}
}
```

## Tweetorial Data

`tweetorials.json`

This file contains a json array of all tweetorials. Each tweetorial is a single object in the array, and contains the following keys:

```
{
      "all_twt": array of strings, where each string is a tweet,
      "all_txt": string of entire tweetorial text, with tweets separated by '~tweetbreak~',
      "author": username of author,
      "date_posted": date in format like "Thu Nov 21 14:51:32 +0000 2019",
      "first_tweet": string of just first tweet text
      "first_tweet_favorites": integer, at time of collection,
      "first_tweet_retweets": integer, at time of collection,
      "last_tweet": string of just last tweet text,
      "num_tweets": integr, numeber of tweets in tweetorial,
      "title": string, researcher assigned title,
      "topic": string, researcher assigned topic,
      "user_followers": integer, at time of collection
    }
```


## Annotation Data

`annotations.csv`

This file contains all the tweetorial annoations reported in the paper. Annotation columns contain either 1 (tweetorial contains that content) or 0 (tweetorial does not contain that content). The columns are as follows:

### Columns about tweetorial content

* Author: twitter handle of author
* Date Posted: date first tweet was posted
* Title: researcher assigned text string for ease of reference
* Topic: researcher assigned topic
* Link: link to first tweet on Twitter
* First Tweet: text of first tweet
* Last Tweet: text of last tweet 
* All Tweets: text of all tweets, separated by '~tweetbreak~'

### Lede annotations


* Correct the Record
* Counterintuitive
* Time Peg
* Appeal to Authority

### Conclusion annotations

* Significance statement
* Refers to lede
* Where to learn more
* Summarizes info
* Call to action

### Body annotations

* Narrative
* Analogy 
* Nonexamples
* Signposting
* Subjectivity
* Informal language humor
* Engage Conversationally
* Credibility
* Media
