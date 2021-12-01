---
layout: project
type: project
image: images/holoholona-home.png
title: Holoholona
permalink: projects/holoholona
# All dates must be YYYY-MM-DD format!
date: 2021-11-30
labels:
  - Javascript
  - React
  - Meteor
  - Bootstrap 5
  - MongoDB
  - HACC
summary: Web application to assist the Hawaii Dept. of Agriculture when checking-in pet owners. Created for HACC 2021
---
## Links
* [HACC 2021 DevPost](https://devpost.com/software/astruhoids)
* [Holoholona GitHub Page](https://github.com/HACC2021/astruhoids)

## About the project
Holoholona is a check-in application that my group and I created as a submission for the 2021 Hawaii Annual Code Challenge (HACC).
The application was created for the Hawaii Dept. of Agriculture's (HDOA) "Pet Pickup" challenge. Their problem was 
straight-forward -- they needed an application to check-in people that are waiting to pick up their pet/animal
after completion of the quarantine and inspection process that comes after flying in from another state/country.
Due to their current infrastructure and COVID guidelines, it is hard for the HDOA to check-in and communicate clients.
Additionally, checked-in persons must wait outside the animal quarantine office, which is lacking in publicly-accessible
amenities and shade, making for an inconvenient and uncomfortable experience.

Holoholona was created to help alleviate these problems while maintaining the lowest cost possible given the HDOA's
claims that they are lacking in budget.

## Contributions
For this project I mainly worked on the `/view` page, where users could confirm that they are checked-in. It also provides 
a method of checking if one's pet is ready for pickup, alongside receiving an email notification. A user can see if they
are checked in if their "Check-in ID" is listed on the page. To help alleviate privacy concerns, this ID mainly consists of 
a user's first name and last initial. We also do not keep user information longer than needed -- it is deleted after
they pick up their pet/animal.

The `/view` page also doubles as a management interface for logged-in admins (i.e., HDOA staff). From this page, the admins
are able to mark animals as ready-for-pickup, which sends an email to the pet-owners and updates their status on the `/view` page.
This way, clients know when it is their turn to retrieve their animal without having to wait directly outside the inspection office
to hear their name being called. After a client picks up their animal, admins can also delete the check-in entry from `/view`.

## Experience and Takeaways
Overall I thought participating in the HACC was a good experience since groups are coding towards a specific real-world goal.
However, it did feel a little limiting given the requirements, at least for our group's chosen project of Pet-Pickup.
We stayed true to the project requirements of being solely a check-in app and being as low budget as possible.
So, instead of integrating with a platform like Twilio for communication between HDOA workers and clients,
my group and I chose use email since it doesn't cost anything. We also stayed away from being flashy and chose to
omit any features that were irrelevant to the app's main purpose of managing check-ins.
Perhaps we should have chosen a different project or should have just coded those features in anyway to show
what is possible.

An important takeaway I've seen is that presentation is very important. Some groups that I thought did well enough
to be top contenders did not place in the top 3. At the same time, one team from the top 3 placed 
even though their application was non-functional, and in my opinion, it has some features that did not belong.
In spite of that, they still placed as they did a good job of selling their application.
