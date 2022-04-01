Unit 8: Group Mileston
===
# Gathr.ly

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)

## Overview
### Description
Scheduling outing app. Users can set dates that they are available and app will find a time/day that everyone/most people are available

### App Evaluation
- **Category:** Social Networking
- **Mobile:** This app would be primarily developed for mobile but would perhaps be just as viable on a computer in the future.
- **Story:** Find the time and day that everyone/most people are available for an event.
- **Market:** Any individual could choose to use this app. Can specifically be targeted to young adults who have responsibilties such as school, work, etc. that may make it difficult to align schedules with others around them.
- **Habit:** This app could be used as often or unoften as the user wanted depending on event frequency.
- **Scope:** Start with only schduleing feature. May expanded to a somewhat larger scope including Chat system in the future version.

## Product Spec
### 1. User Stories (Required and Optional)

**Required Must-have Stories**

* Login/Sign Up page - User logs in to app if they have an account, otherwise they will sign up for an account.
* Add a friend - user can add a friend to contact list
* Invite a friend using a code 
* User can add availability
* User can create event
* User can edit event
* User can delete event
* User can view all events
* User can view overlapping available times for everybody/most people
* Users in same event can chat together

**Optional Nice-to-have Stories**

* Reschedule events from a “past events” list
* Chat system for each event

### 2. Screen Archetypes

* Login/Signup - User signs up or logs into their account
* Friend list
    * Add a friend button
    * Can remove friends
    * See friend requests
* Events list
   * Create an event button
   * See incoming event requests after tapping on a different button?
   * Can edit and delete events
   * Event detail screen after tapping on an event in the list
   * Can use Google Maps to add event location
   * (Optional) Sorting/searching list

### 3. Navigation

**Tab Navigation** (Tab to Screen)

* Login/signup activity
* Main Activity fragments
    * Events List as default fragment
    * Friends List
* Event detail activity


**Flow Navigation** (Screen to Screen)

* Login Screen/Sign up screen => Event list
* Create event button on event list => Create event screen 
* Create event screen => Event List
* Create friend button on friend list => Create friend screen
* Create event => google maps screen
* Google maps screen => create event
* Create event => event list
