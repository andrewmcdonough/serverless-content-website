# Hello World

This is the first post in a series where I describe why I am building a serverless content management system, and my journey in building it.  Eventually, I hope that the software, which hasn't been written yet, will power the website where this lives.

## Day 1

I've checked into [Roam](http://roam.co), a 'coliving' space in Ubud, Bali.  I want to work on a personal project for the next week.  After considering a bunch of other options, I've decided the 'serverless content' engine is what I will be working on.  I plan for this platform to run on Github and AWS lambda, where anything merged into the master branch of a website gets built by a lambda function and deployed on AWS S3/Cloudfount.

## Ghost

I've been spending some of today looking at Ghost, and the way they handle site templates.  Templates are stored as handlebars files, with all templates extending a default template.  I like the idea of letting people use Ghost templates out-of-the-box, so I'm considering using their template format.

## Step 1

Putting templates aside for some time, I think the first step should be for the app to:

* Watch a github repo
* Copy an index file from the repo to an S3 instance
* Serve that file over cloudfront

If I manage to get that done by the end of the day, I'll be happy
