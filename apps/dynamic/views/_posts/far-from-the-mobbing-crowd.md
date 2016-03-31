---
layout: post
author: matt
title:  "Far from the mobbing crowd"
date:   2016-03-31 00:00:00
nav: blog
---

A few weeks ago, Steve Tooke and I gave a [talk at QCon London](https://qconlondon.com/presentation/far-mobbing-crowd) about the culture at Cucumber, and I decided to write up the talk as a blog post. Here it is! You'll learn about our values as a company, the way we work together, and specifically what we love about mob programming.

Cucumber is an open source project, and now also a company. We've got no idea how many people use Cucumber, because it's freely available. People can just download it and use it and they never have to get in touch with us unless they want to. Aslak, who likes spreadsheets, reckons there may have been five and a half million downloads last year, which is double what he thinks there were two years before that.

This post is about our journey to try and build a business around this accidentally popular tool that we love.

## Our business plan

Aslak has [already written about our business plan](https://cucumber.io/blog/2014/04/16/cucumber-limited), and nothing much has changed since then. Cucumber is getting more and more popular (we can't help it!). That means more demand for our training and consulting, and by delivering on that demand we get revenue, which then makes more time for working on the open source, which is what we love to do. Then, because we make it more awesome, it gets even more popular, and so we get this beautiful virtuous cycle.

In spending so much time visiting our users in our consulting practice, we noticed that there was a need for something more polished than the open source tool. When you're trying to adopt BDD in an organization where there's some resistance, the tools need to be user-friendly and slick, especially for the non-technical folks. We saw an opportunity for a product that might also give us a different kind of revenue.

## Cucumber Pro v1

We started to build Cucumber Pro in our spare time while we were traveling around the planet delivering training. At the same time, we all started having families. I had a house to renovate as well. It was exciting, but also stressful, trying to bootstrap this product on the side as well as doing all this other stuff.

We built the first version of Cucumber Pro, and we got some people to start using it. But all the traveling was taking a toll on our family lives. We saw this product as something that could save us from that, so we started to put pressure on ourselves: it had to work.

If I'm honest, I think we also had an attitude that because we're all experienced programmers, we could afford to cut corners and just iterate fast on what the customers needed, telling ourselves we'd be able to refactor ourselves out of a mess later. Ever heard that one before? Yeah, it doesn't end well.

In [The E-Myth Revisited](http://www.amazon.com/E-Myth-Revisited-Small-Businesses-About/dp/0887307280), Michael Gerber talks about how most people who start their own businesses discover they're the worst boss they ever had. It started to feel a bit like that.

So this rushing, this hunger, this almost-desperation led us to the point where we had product that just wasn't fitting. There was a need, but what we had didn't fit the need - it wasn't resonating with the users. And at the same time, we had grown to hate the code. It wasn't working for anyone. So we decided to take a step back, take a bit of a break, and focus on other things for a while.

## The Reboot

During the summer of 2015, the whole company (including our families) met at Aslak's family summer cabin on the coast of Norway. We worked together, ate together, played together, and some of us stayed up far too late drinking whisky together. We talked a lot about the product, what had gone wrong, and what we would do differently this time. Mostly, it came down to slowing down, being patient, paying attention to quality, and listening to our users.

We're all extreme programmers, so nobody needs to convince us about the benefits of pairing. In practice, however, a lot of the old codebase had ended up getting built solo, by people in hotel rooms and on planes and so on. So we didn't have that shared consciousness about the code. We wanted to fix that too.

We strengthened the team, and resolved to reboot the product by committing the month of October to the product. No one would travel, no one would do any consulting. We had a brand new codebase and a new tech stack, and we added Steve Tooke and Romain Gérard to the team. This was daunting - we had toand figure out a way to work together and learn together, but still make real progress. 

It was a great opportunity for us to try something that we'd been hearing a bit about.

## The mob

We decided to try mob programming. In case you don't know what it is, here's [Woody](https://twitter.com/WoodyZuill) explaining:

> All the brilliant people work on the same thing, at the same time, in the same space and on the same computer.

Steve describes it like this: -- you know the thing about XP that Kent Beck says, where we wanted to take all the good things that we did and turn them up to 11? Mobbing is like turning pairing up to 11. All of the good stuff you get about learning from each other, bringing the quality of the code up to the standard that everybody's happy with, all of that is accentuated by mobbing.

Another XP practice, collective code ownership, gets turned up to 11 as well, because everyone owns every line of code. Everyone's had a chance to have their say about every line of code that's written, so everybody's concerns about the code get shared. You can resolve issues either by helping people understand why they don't need to worry, or by actually factoring that concern in with a change.

So far, so good.

We do have a bit of a challenge with mobbing, however.

We're a remote team. I live up in the wilds of the Scottish Highlands. Steve is in Southampton. Aslak's in London. Julian and Romain are just outside Brussels. It's hard to work on the same computer in the same space at the same time.

But we've taken the decision that we want to be able to live where we want to. There are benefits to being in your own space, being comfortable in your surroundings, being near your family. Here's Steve working with his three-month-old daughter Primrose, making her first commit. Here's Aslak with his four-month-old daughter Aurelia. There's something really special about being in an environment where you can do that.

But the challenges of being a remote team mean we have to find new tools. We use Slack for team chat, and Screenhero to enable multiple people to share the same computer at the same time. Everyone gets their own pointer. When it's your turn to type at the computer, you share your desktop with everybody else, so you work in the tools you're comfortable with. Usually we have a second screen, either a phone or a tablet or just a second monitor with a Google Hangout so we are all looking at each other, talking to each other using Google Hangouts. And that's how we code everyday.

## STFU

It can get pretty intense and stressful. It's much more difficult to communicate when you're not in the same room. We have to work hard to understand when someone is uncomfortable with what's going on, and to communicate about what's working and what isn't.

It doesn't always go well.

At the end of October, after we'd done this experimental month of mobbing on the product, we had a big retrospective. One of the big issues was that we needed to be more _kind_ to one another. We came up with a rule that you can only heckle on green. If the tests are failing, you can only speak to help the mob get the test to pass.

If there's one thing we've learned about mobbing, it's the important of shutting up. Sometimes you need to bite your tongue and let them get on. Some of us even use a push-to talk mic to help us stay quiet. If you can offer something supportive, something encouraging - great, help them. But if you've got a thought about how it could be even better than what they're doing right now, write it down. As soon as you get to green, you can share it. It's surprising how often it comes up in the natural flow anyway.

## Continuous Retrospection

This big retrospective at the end of October was so valuable that we asked ourselves: why did we leave it this long? We came up with a new habit to hold a short retrospective every day. At the end of every mobbing session, we stop 15 minutes early and ask ourselves a series of questions like: _What did we do? What did we learn? Did we decide anything? Did we make any new working agreements? What are we puzzled about?_ A puzzle is a positive way of framing anything you can't agree on.

We log our retrospectives in a text file in the master branch of the main repo. This helps those of us who are traveling around the world, because we still have a training business to run. When I was in the States last week, I could read the retrospectives and catch up on what I'd been missing.

## The routine

Every morning, the mob convenes at 8:30 on a Google Hangout. We code or research or explore the problem domain as a group until 11:45. Then we have our retrospective, and stop for lunch at noon.

So what do we do in the afternoons? Well, we've still got a business to run. It might be things like tweaking the website, answering email, taking sales calls, writing sales proposals. It's a chance for us to work independently, to give us a break from that intensity of sharing a computer and working together. Sometimes we'll do solo work on the product too. Maybe we'll tackle a refactoring, or create a pull request that the mob can review in the morning.

Four hours feels about the natural amount of work we can accomplish. Because the mob runs pretty fast, it makes a lot of decisions quickly, and after four hours it's not exactly that the mob's run out of energy, it's more that we're out of certainty, that we could productively continue to grind through problems. You need space to ponder, experiment, do a bit of divergent thinking.

Mostly, the mob is converging: building code and working code, but that has to be fed with good ideas that have come from divergent thinking, which is something you often need to do in private.

## Can't decide? Do both

Occasionally, the mob gets stuck. There's a problem we haven't come across before, and nobody knows what to do. How are we going to move on? Sandy Metz once told me that when conversations are going round and round, it's an indicator that there's not enough information in the room. What we do at that point is something called Set-based problem solving.

Instead of arguing about which one is best, we'll list all the various options. Then we'll split up into pairs or small groups and spend a time-boxed period - maybe half an hour - writing some throwaway code to explore those options. We bring the results back to the mob and share what we've learned. Every single time we've done this, none of the options that we've investigated alone are the best solution. We all bring new information into the conversation, and we end up with something better than any of the original ideas.

I'm sure it's a good pattern for handling conflict generally. I want to go this way, you want to go that way. Well, I'll tell you what, why don't we go both ways for now? Then we'll meet back here and talk about what we learned.

## Resilience

The other thing that amazes me about the mob is its resilience. Suppose I have to take a phone call. I disappear for 15 minutes, I come back. The mob's been rolling on, writing high-quality code. I can easily pick up what's going on and start to contribute within minutes. Pretty amazing.

On a larger scale, if I have to go away for a few days of training, maybe in a different time zone, the mob carries on. We're swapping different people out each week to deliver the training courses, but the consciousness is still there and the code is moving forward all the time. It's powerful.

Im my crazy moments, I imagine building a team where there were enough people in enough timezones that the mob could keep going 24 hours a day.

# Symbiosis

Running and growing this business is an adventure. Being a business owner and a developer at the same time is amazing. It's so good for you on both counts. Mike Feathers has [been writing recently](http://www.r7krecon.com/#!provocation/gfqa5) about the Symbiosis between code and organisation, and this is something we live and breathe every day. Most of the development team are also major shareholders in the business, so we're literally stakeholders in our own project. I wish there was a way for bigger organizations to experience this fusion of commercial and engineering perspectives.

# Play

Because we get to build our product in the way we know works well, that feels like play. Fun alone isn't an objective, but I think it's possible to find joy in almost anything, even writing a sales proposal. What we really love to do is to learn and improve ourselves - developing our [mastery](http://deliveringhappiness.com/the-motivation-trifecta-autonomy-mastery-and-purpose/). I think we develop our mastery best through play, and mobbing feels playful. If you've done pairing and worked in an XP team, you'll know how playful that can feel. When you're playful, you're relaxed. When you're relaxed, you make your best decisions.

Kent Beck, at the beginning of the first XP Explained book, talks about two different cultures.

> In the mountains,
resources were scarce and people were always on the brink of
starvation. The culture they evolved was horrific. Mothers abandoned
babies to roving packs of feral children as soon as they had any
chance of survival. Violence, brutality, and betrayal were the order of
the day.
> In contrast, the forest had plenty of resources. A person had only to
spend half an hour a day providing for their basic needs. The forest
culture was the mirror image of the mountain culture. Adults shared in
raising children, who were nurtured and loved until they were quite
ready to care for themselves. If one person accidentally killed another
(deliberate crime was unknown), they were exiled, but they only had
to go a little ways into the forest, and only for a few months, and even
then the other tribespeople brought them gifts of food.
> XP is an experiment in answer to the question, "How would you
program if you had enough time?"

So maybe Cucumber Ltd is our experiment in answer to the question - _how would you run a software company if you had enough time?_
