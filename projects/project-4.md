---
layout: project
type: project
image: images/nebula-project-page.png
title: Nebula
permalink: projects/nebula
# All dates must be YYYY-MM-DD format!
date: 2021-10-22
labels:
  - Javascript
  - React
  - Meteor
  - Semantic UI
  - MongoDB
  - Amazon S3
summary: Web application to assist advisors of the FIRST robotics program in managing their robot's construction. Created as a submission to the 2021 Meteor Impact Hackathon.
---
## Links
* [AstrUHoids GitHub Organization](https://github.com/astruhoids)
* [Nebula GitHub Page](https://github.com/astruhoids/nebula)

## About the project
Nebula is an application my group and I created as a submission to the 2021 Meteor Impact Hackathon. It was intended to be
used by advisors of the FIRST robotics program during the building phase. During this time, communication among advisors
as well as between advisors and students can be inefficient due to the use of email and paper documents. Thus, it can be
inconvenient to track the robot's progress, which student was assigned to machine a particular part, or if a particular part is done or still needs to be reviewed. The idea behind Nebula was to make these tasks easier.

Screenshots and more information about the project's background can be found on its
[README](https://github.com/astruhoids/nebula/blob/master/README.md) page.

## Contributions
For this project my main contribution was getting our database to track when a project board card was dragged into a different
column (e.g., moving from "To Do" to "In Progress"). I also had to track the cards' indices, or their place in their column
whenever a user updated the board. I found the latter difficult and it took me a lot of thinking to come up with an
elegant and concise solution. I also wanted to come up with a way to make it work well whenever the cards were filtered, but I
couldn't think up a good way to do this. Though the feature worked well enough without having to add special cases for filtering, 
improving it further didn't seem to be worth the time during this five day code period.

Other than the aforementioned features, I feel like I was mostly fixing or adjusting styling, 
putting the finishing touches on features that were mostly completed, or fixing bugs.

## Takeaways
Though this is tied to the React framework, I did learn that setting a state (`this.setState({})`) was not instant. For example, 
one can print the state after calling `setState()` on the previous line and not have their new changes printed.
During my attempts to update the project board cards' indices based on their new states after being dragged and dropped into a 
different spot, I noticed that somehow my code was fetching old states. The solution to this was to pass a callback function
into `setState()` which looks something like this:
```js
this.setState({ "key": newValue }, () => this.someFunction());
```
This callback function is executed after the state is updated, making it easier to accomplish what I needed to.
I didn't realize this prior and I think it's good to know about when working with React.  

Taking a step back from anything directly code related, I think my group and I could have planned better. There were some
instances where some of us were working on the same feature or working on a feature that we didn't need due to miscommunication.
Next time we can make sure that everyone is on the same page to cut out on wasted time and make the development process smoother.

Additionally, we were all unsure of what our app would look like. Our app was pretty short and simple so in the end I don't think 
this affected us too much. However, I think it would help if everyone knew how the app looked like and how it should operate
so that there is a clear goal in mind on what to create. It is harder to work with and code for a more nebulous idea.
