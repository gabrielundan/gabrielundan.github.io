---
layout: essay
type: essay
title: Ad-Astra
# All dates must be YYYY-MM-DD format!
date: 2021-10-14
labels:
  - Javascript
---

## Links
* [AstrUHoids GitHub Organization](https://github.com/astruhoids)
* [Ad-Astra GitHub Page](https://github.com/astruhoids/ad-astra)
* [Ad-Astra Project Page](https://astruhoids.github.io/)  

## Development stack
* Meteor
* React
* Bootstrap 4
* MongoDB
* Amazon S3

## About the project
Ad-Astra is an application that my group and I created to warm up and familiarize ourselves with our tech-stack in
preparation for the Meteor Hackathon and the Hawaii Annual Code Challenge. To do that, we had to create a simple clone 
of [Lumisight UH](https://uh.campus.lumisight.com/), a COVID-19 symptom tracker for the University of Hawaii.  

We had to replicate the following features:
* Log the days a user is or is not feeling symptomatic via a questionnaire 
* View the user's past questionnaire answers
* Allow the user to input their vaccine card information and a photo

## My contributions
For this project my main contributions were tied to the daily questionnaire. I had the responsibility of making the
questionnaire functional and transact with MongoDB whenever the user selects an option. Additionally, I also had to
create a React component that notifies user if they had not yet filled out the questionnaire for the day. If they had, 
the component would alternatively notify the user if they are cleared to set foot on campus.

I was also in charge of doing some style translation into Bootstrap 4 since the styling of the template is
in Semantic UI. A couple of my group members had no previous experience with Bootstrap, so some of their components
also needed to be converted to make use of Bootstrap styling and keep our pages looking similar.

## Takeaways
Overall I think this was a good experience to refresh my memory on how to use Meteor, React, and MongoDB. However,
I did think that this project was on the simpler side, aside from setting up and dealing with file upload with Amazon 
S3. There were only two simple forms we had to create, both with minimal data processing. Also, there was little
complexity with the UI. Though I dislike working with UI and styling, I do want to be better at it. So, I would have liked if this assignment involved replicating a more robust UI.

Returning to the topic of Amazon S3, it was very hard and confusing to set up permissions when attempting to upload or
access files. Since this was just an assignment, we settled on just allowing anyone to upload and view files. However,
in an actual production environment, this should not be the case. Ideally, only upload or view requests referred by 
our app should be allowed. Additionally, viewing should be further restricted to the user who uploaded the image.