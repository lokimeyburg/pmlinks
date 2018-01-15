---
layout: post
title:  "Managing Your Product Development Around Orthogonal Epics"
date:   2016-10-31 10:18:00
---

Almost every project starts the same: with a clear vision of what you’re about to build. When you close your eyes you can perfectly picture what you’re building and everyone feels charged with excitement to start building the new product. The first few weeks go well as everyone is inspired by the blank canvas in-front of them: designers are creating mockups and developers are laying the foundation. Everyone has “new product infatuation”. 


I always remember the first “oh fuck!” moment in every new product. After the first few weeks important details stampede over the product team. When one edge case is presented, the others come along in droves. Things you never thought about are now important matters you need to address! 


In which country are we releasing the app?
Can we launch without this feature?
[add more examples of edge cases]


Now, the product that once started with such excitement and clarity is a mess! It’s become difficult for you as the product manager to understand the progress of various parts of your product and also you’re struggling to prioritize upcoming features. There are people from your team coming to you on a daily basis with small edge cases that you need to consider, plus 


In this article I’m going to show a method that I’ve found has worked for me over the last few years and has helped me get a better picture of my overall product’s development, helped me confidently prioritize my roadmap and made me sleep much better at night.


Below is a preview of what we’re going to aim for. (At the end of this article I will provide Jira workflow templates so you can implement this in Jira, even though the ideas and philosophies are what’s most important and could be implemented in most project manager tools).


Managing features not tasks


One mistake I’ve seen people do is organize their projects around responsibilities. For example:


[insert picture of design, development, qa]


Here’s the problem with such an approach: it’s not a clear way of visualizing how far away each feature is from being finished. Instead, what you want to do is list everything required to complete each feature like this:


[show image]


Isn’t that much better? Now, at a glance, you can look at each list and quickly get an idea of how far away each feature is from being completed. Now, as a product manager, you just need to worry about checking off each feature one-by-one. Finish each feature as soon as possible. Done, done and done. The momentum feels good and shipping feels better. This sounds like such a “obvious” way to manage product development, but you’ll be surprised at how many product managers make this fundamental mistake. I even see product managers create “epics” for “design work” before starting a product.


From here, you can manage your product at the “feature” level. You’re managing at the week and month level, not at the day-to-day level. This is a much better way of seeing progress towards of your product


[ show Jira image of the columns I use ]


At the end of this article, I will include information on how to manage your products 


Orthogonal Epics (or how to create the right “Epic”)


Most product managers will call these “epics” in agile product development, and they’d be right. But here I’d like to spend a little time talking about the right epic. Firstly, an epic needs to be small’ish (shouldn’t take longer than 2 months to complete) and have a clear finish. I’ve seen “epics” such as “Refactoring” never get completed. 


Also, new issues or tickets that are created as a result of the work being done on the “epic” but do not directly contribute to the completion of the “epic” should not go under the original epic and instead be moved to the backlog and not be. For example, while working on a “Sign Up with Facebook” feature, an engineer realizes that they can improve the experience by [ something ] and quickly creates a ticket for the improvement and proceeds to put the ticket under the same epic. At first this makes sense, and it does help group tickets and organize the backlog. Unfortunately, it’s now more difficult to estimate when the “epic” will be completed as it has become bloated with improvements. Bugs, on the other hand, should be included and dealt with.


Epics should strive to be orthogonal to one another. Orthogonal means “isolated or partitioned”. This means that you can have people work on one epic over there and it won’t affect work being done on another epic. This is a great way to break your team into smaller 2-4 people strike teams and work independently of one another. 


As much as possible, try to avoid having two teams work on epics that are closely related. For example: it might be tempting to improve the file uploading experience of your application and break your teams up into “upload with dropbox” and “upload with drive” teams and have them parallelise their work. The problem you’ll run into is that they’re closely related and cross-team dependencies are very likely going to happen (things like talking about third party security, tracking third party apps, etc). It would be better to have one team solely work on the “uploading” feature while the other strike team works on something completely unrelated. It feels unnatural at first - work getting divided this way, teams working on different problems - but it’s much more efficient, reduces dependencies, and people like working in smaller teams.


Roadmapping 


Almost always it’s not a matter of whether you should build something, but rather when you should build it. Having a list of features and prioritizing them can be one of the most challenging responsibilities of a product manager. I’m a big believer in managing a product’s roadmap from market evidence. When somebody comes to you with a feature request, create an epic and in the epic, write down the evidence. If you’re talking to a potential customer and they mention similar problems, record it and link to the interview notes from the epic. The epic should also be a place of discussion. 


[ show an example of an epic with discussion ]


Roadmapping is about 80% just prioritizing epics by market evidence. It’s that easy. Epics are worked on one-by-one, just taking one-off the top of the stack each time. The other 20% of the time is that sometimes you may end up building right feature, right problem, but not at the right time. It’s important to keep pace and direction with the company as a whole and not overstep when you shouldn’t. Perhaps a feature should be timed with other product releases or business activities? If your company is experiencing cash flow issues, perhaps it’s better to focus on quick-win features that will result in a burst of revenue, instead of working on that feature that’s good for the long-term, but won’t see a return on investment for a while.


At some point an epic has collected enough market evidence that it’s time to begin thinking about when you will begin working on it. At a very high-level and with the help of my lead engineer, we create a few “stub” tickets under the epic to begin defining our MVP. The engineer estimates the work at a very high-level. (Will it take 3 weeks or are we looking at 2 months).  Now, you should have a collection of epics, full of evidence, discussion and a high-level idea of how much effort is involved in completing the epic. Since you know your team’s average velocity you can get a rough idea when you might be able to release a feature into the market. 


[ Show picture of stubbed epic ]


I like to arrange my roadmap in quarters (3 months) up to a year and then have a “future” category (something we’ll probably do). Brand new epics usually start as feature request and end at the bottom of the pile and slowly begin collecting evidence and start working their way up the priority ladder. I wish JIRA had a better way to visualize swimlines, but below you’ll see what it typically looks like:


[ show jira with quarters ]


Whole product management and Epics


Whole product management is the idea that a product is more than just the bits and bytes of the software you sell. A product is the marketing, customer support, documentation, and anything else that backs/supports/elevates your product. This means, it’s important to also manage other business activities to support your product. I usually use a different colour for these epics to separate them from engineering activities. The reason it’s important to include these supporting activities are that often times they’re for features that are about to be released in the coming months. For example, knowing that you will release a feature around June, you can get marketing to help you create blog content, ebooks or whitepapers weeks before to peak the interest of your market. Sales needs to know about the new feature and have their sales decks updated. Partners need to be trained on the new feature too. All of these are 



Managing epics instead of user stories


If a developer is a few days late or maybe even a week late. If you’re working at the month level and trying to align things for 4 months from now, the slip seems trivial.




