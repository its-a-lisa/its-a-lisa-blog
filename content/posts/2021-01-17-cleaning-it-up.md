---
template: post
title: Making the move to Twitter lists
slug: cleaning-it-up
socialImage: /media/012-safety.png
draft: false
date: 2021-01-19T17:04:49.197Z
description: Cleaning things up a bit, starting with Twitter
category: blogging
---

# Making the move to Twitter lists

## Problem Statement:
- Don't engage the way I want to engage
- Not seeing threads from people
- Feel like I am staying in my bubble too much
 
## Approach:
- Extract who I am following now
- Group into lists
- Automate it so I can easily add to it later

## Considerations

- Public or Private Lists

| Visibility | Pro | Con |
| ---------- | --- | --- |
| Private | --- | - Can't share list with others |
| Public | - Easy to share with others | - People on list get notified |

## Execution

### Extract who I am following now

Wow, this is proving to be a lot harder than I thought. 

#### Here are all of the things that failed:
- **Using Postman** Not sure what happened here. I swear I was using the authorization tokens appropriately, but I kept on getting 404 errors. Nothing seemed to work, but I am not going to give up forever, but after trying for a little over an hour, I have to give up for now. 
- **Using Twit** So promising, but no luck. Seems like this would have worked for just about everything that it is meant to do, _except_ for what I am trying to do. Womp Womp :(
- **Writing code with Tweep** This would have worked if I had done it properly, I'm pretty sure. But I didn't, so it is getting added to this list of failures. I had played around with this the last week when I was starting to use python; but completely forgot that it wasn't a command line tool so I thought it was trash because I had just tried using Twit, so when it didn't work like that, I figured it didn't work either. Aka -- this was completely user error and I'll probably go back some day and use this method. 
- **Chrome Extenstion - Webscraper.io** I didn't put too much effort into it. I followed the instructions and it wasn't obvious how it should work, so I moved on pretty quickly. I'm about 56% positive that it might have worked, but I just didn't know where to look to see the results.
- **A sketchy Google Sheets with scripts** Ya know... when you get to that point, where you just want it to work, to _just freaking work_ !? Ya, that is what happened here -- there is a good chance that I even got to it from another articles that was like, "Hey! You, ya, here look at this thing! It's sketchy!!" but I only read the first sentence. 
- 
#### Here is what eventually worked:
- https://medium.com/@SamSchmir/a-guide-to-the-twitter-api-and-twurl-8711466a0635
- https://dev.to/twitterdev/how-to-use-twurl-to-quickly-test-the-twitter-api-4n48

- https://gist.github.com/JamieMason/7580315
## What I learned
- How to use jq
- API Rate Limit
- API Paging
- 
## Conclusion

| Hypothesis | Expected Result | Actual Result |
| ---------- | --- | --- |
| Difficulty | Easy | Hard |
| Level of Effort | Low | Moderate |
| Learning | Low | Moderate |

## Resources:
[How to Set Up and Use Twitter Lists: 9 Great Ideas](https://blog.hootsuite.com/twitter-lists-new-follow/)