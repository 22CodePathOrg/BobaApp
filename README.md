# Boba Rating App
Original App Design Project - README Template
===

# Boba Rating App

## Table of Contents
1. [Overview](#Overview)This is going to be a fun and interactive app. The user will be shown list of drinks offered and ratings associated to it. The user can login to app and rate the drinks..
2. [Product Spec](#Product-Spec) 
3. [Wireframes](#Wireframes)
4. [Schema](#Schema)

## Overview
This is going to be a fun and interactive app. The user will be shown list of drinks offered and ratings associated to it. The user can login to app and rate the drinks.
### Description
Going to keep two login profiles one for Quiz creator and one for quiz player. Going to user back4app for backend and creator can create a quiz and player can select quiz and play them.


### App Evaluation
[Evaluation of your app across the following attributes]
- **Category:** Checkout and Rating (Sell)
- **Mobile:** Using Camera, Audio and user profiles are saved.
- **Story:** I think rating the drinks will be interesting and will attract users
- **Market:** As I said earlier we can create different types of drink ratings and attract customers
- **Habit:** If we update quizes drinks offered regularly there will be growth. As people drink bearages atleast once per day
- **Scope:** Hopefully we can complete this app by the end of this program. But this a big app so will try to complete required stories

## Product Spec

### 1. User Stories (Required and Optional)

Required Must-have Stories

- [*] Dashboard with trending today items from api.
- [*] Show ratings for drinks.
- [*] Settings for the app
- [*] Selection of drink in a recycler view to show the details
- [*] Hide the details from Dashboard
- [*] Descriptions for the selected view along with ratings

**Optional Nice-to-have Stories**
- [] Adding filters for cheap, favourite and top rated for drinks.
- [] Login by Facebook
- [] Try audio type for product description


### 2. Screen Archetypes
* Login
* Signup
* Homepage
* Promo Page
* Search Page

### 3. Navigation

**Tab Navigation** 

Search
Profile
Home

**Flow Navigation** (Screen to Screen)

Dashboard -> Gets all the drinks
Drink Selection -> Jumps to promo page
Search drink
Promopage and checkout


### [BONUS] Interactive Prototype

### App gif

Have to join login and tea dashboard as we did them seperately by 2 people

<img src="gifsimpledo.gif" width=600>

## Schema 
## Model

   | Property      | Type     | Description |
   | ------------- | -------- | ------------|
   | objectId      | String   | unique id for the each drink |
   | description       | String| about drink |
   | image         | File     | image of drink|
   | rating | Number   | rating of each drink |
   | ratingdisplay    | Number   | sum of ratings |
   

### Networking
    - Home Feed Screen
      - (Read/GET) Query all drinks where user is logged in
      - (Create/POST) Create a new rating on a drink
      - (Create/POST) Create the drinks selected list
   - Search Screen
      - (Read/GET) Query all top rated drinks that has rating greater than 4 
   - Promo Screen
      - (Read/GET) Query all selected drinkss
   - Profile Screen
      - (Read/GET) Query logged in user object
      - (Update/PUT) Update user profile image
- [OPTIONAL: List endpoints if using existing API such as Yelp]
