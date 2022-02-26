# Car Comparisons

## Purpose
*The main purpose of this project is to demonstrate back-end skills. While the main features of the website are relatively simple, it will be **cloud-native, scalable, API Exposed and use CI/CD***

The purpose of this website is to allow users to easily access pricing data between the most popular brands of new cars available today. The website only contains data on the following brands due to supply, features, reliability and popularity:
- Mazda
- Hyundai
- Kia

This could potentially be a microservice of a more complete website. The target audience for this app is people who are looking at purchasing a new car. It will allow them to budget correctly and decide between make and models of different carmakers.

*(Note Toyota was left off the list due to supply shortages)*

Future plans are to have the app return pricing for bicycles and motorbikes.

## Features
- Drop down menus to select Make and Model of car
- Displays minimum, maximum and average price of selected car
- Hosted on AWS
- Uses Serverless
- CI/CD
- Lambda functions
- Scalable
- Event driven

## Tech Stack
![](/docs/techstack.JPG)

## Data Flow Diagram
![](/docs/dfd.JPG)

## Architecture Application Diagram
From the Devs perspective, the Architecture will resemble the following. By doing this it will allow the dev to write functions in their preferred IDE, push to GitHub, and by using webhooks automatically deploy to Lambda for testing and deployment. Once deployed the Lambdas will be accessed by the API gateway to communicate with the database to retrieve the data.

!["Dev Architecture App Diagram](/docs/devaap.JPG)

This is what it will look like on the users end. User will view the webpage. API will communicate with the lambda functions to select a Make and Model of car. A function will then retrieve these results from the database, which will be passed to another function to calculate the results and display on a separate webpage.

!["User Architecture App Diagram](/docs/useraap.JPG)

## Wireframes

Keeping the wireframes and UI very simple as the focus of the project is back end.


!["Homepage"](/docs/wireframes1.JPG)

!["Results Page"](/docs/wireframes.JPG)

## User Stories

**Rob**

As a father, I want to be able to compare car prices when purchasing a car for my kids so we can get great value out of it.

**Sarah**

As someone who is currently selling their car, I want to know what cars are going for at the moment so I can price mine to sell quickly

**Max**

As a teen, I like to look at the prices of cars so that I can plan to save up and buy one soon.

**Leigh**

As a city-dweller, I want to look at the average prices of small cars and ensure I don't get price gouged.

**Jeremy**

As a Queenslander, I'd like to see the prices of cars nationwide to ensure we get a fair price here.

**Stella**

As a lover of all things luxury, I like to see the price difference between bottom and top of the range and decide whether it is worth it to upgrade.

## Trello
My Trello board implemented agile strategies. First iteration uses two simple labels. Green for anything relating to planning, and blue relating to coding.

!["First Trello"](/docs/trello1.JPG)

As I went through creating my diagrams more "Next Up" tasks were made to keep track of where I was.

!["Second Trello"](/docs/trello2.JPG)

!["Third Trello"](/docs/trello3.JPG)

!["Fourth Trello"](/docs/trello4.JPG)

!["Fifth Trello"](/docs/trello5.JPG)