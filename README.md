Unit 8: Group Milestone
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
- **Market:** Any individual could choose to use this app.
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
*
### 4. Wirerame
[![Gathr-ly-wireframes.png](https://i.postimg.cc/pX3jGJZ9/Gathr-ly-wireframes.png)](https://postimg.cc/sv911Sby)

### 5. Schema

**Models**
## Schema //TODO
### Events
| Property         | Type          |Description                                     |
| ---------------- | ------------- | ---------------------------------------------- |
| objectId         | Int           |unique id for each event (default field)        |
| Events Name      | String        |name of the event                               |
| Events Details   | String        |description of the event                        |
| Events Location  | String        |location of the event                           |
| Events Time      | DateTime      |when this event happens                         |
|Author            |Pointer to User|who create this event                           |
|Participants   |Pointer to User|who participate this event                      |
|createdAt	       |DateTime	     |date when post is created (default field)       |
|updatedAt	       |DateTime    	  |date when post is last updated (default field)  |
| datesFree        | DateTime        | date when user is available; will be used to calcualte event time|


**Networking**

<b> List of network requests by screen </b>

  * Event Screen
    * (Read/GET) Query all events where user is involved in
    * (Create/POST) Create dates you are free
  * New event screen
    * (Create/POST) Create a new event 
    * (Create/POST) Create event details 
   * Friends screen
      * Read/GET) Query all people user is friends with 
      * (Read/GET) Query all people that match user's name and user's id
   * Profile Screen
     * (Read/GET) Query logged in user object
     * (Update/PUT) Update user profile image
    
  

