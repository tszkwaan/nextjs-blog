---
title: 'Fly2me - a flight order management platform'
date: '2021-03-03'
---

![list of flight order](../images/projects/list.png)

## Background
From 2017 to 2019, I became a frequent flyer and took 1-2 trips every month.

I found there may be something that technology can help to make my life easier - saving me the manual effort to manage the flight & hotel orders.

So I cooperated with Jeremy to build a flight & hotel order management platform.

## Work breakdown

Me:
- Product feature design
- Product UI & UX design
- Frontend development

Jeremy:
- Backend development
- Architecture design
- Setup of CICD

## Status
Completed

- implemented the basic CRUD for flight & hotel management
- incorporated with user-friendly design:
    1. when the user enter a flight number that already has a record in DB, we automatically fill in the flight arrival & departure time & airport for the user
    2. mobile responsive
    3. allow users to skips entering detail & update later
    4. Split the form into stepper form, keep the UI clean & easy to use in each step
    5. Separate the flight order to history & future flight & displayed it in a specific order
        - future flights are displayed in ascending order by date => allow us to focus on upcoming trip easier
        - historical flights are displayed in descending order => allow us to followup with the latest trips' insurance issues if needed

- did not continue to develop advanced features since we did not need to fly frequently anymore

## Screenshot

![list of flight order](../images/projects/list.png)

![empty list of flight order](../images/projects/future.png)

![adding new flight order](../images/projects/add.png)

![adding new flight order](../images/projects/calendar.png)

![adding new flight order](../images/projects/add2.png)

![adding new flight order](../images/projects/add3.png)


## Product Backlog

### Basics
- [x] CRUD to manage our flight & hotel order information

### Advanced
- A calendar view that indicates all our confirmed flight schedule
- Auto share of flight/hotel information after create/update records to a list of recipients
- Remind us to reserve for a hotel if hotel reservation information is not supplied before x days of a trip
- Record the public holiday of the two countries
- Get the real-time flight information through external API - to get the most up-to-date flight information without the need for manual update
- Allow batch input of flight/hotel record
- Allow import order detail by uploading PDF (by OCR techniques)
- Manage list of event subscribers (notify the create/update of order to the list of people) & allow customizable notification means (e.g.: Whatsapp, email, Telegram...)
- Manage the receipt of bookings (allow upload the flight/hotel order receipt)
- Remind before the trip (remind before the trip for luggage packaging, transportation planning)
- Allow exporting the trip to other calendars (e.g.: Google Calendar, Apple Calendar)

## Business opportunities
- Since it was built for personal usage, the product backlog was mostly about how to enhance the user experience and reducing the manual effort needed.

- For business opportunities of a more general version of the system that is open for public usage, here's some basic idea:

    - Scaling up to become a trip planning & collaboration platform, the flight & hotel order management feature became a sub-part of it
    - Allow users to share their travel history + diary in blog format
    - Cooperate with flight companies for the promotion of flight tickets
    - Cooperate with hotels for the promotion of hotel reservation
    - Cooperate with travel agencies for different travel packages
    - Cooperate with insurance companies for travel insurances packages
    - Localization is needed
