# The Wonderful Backend Developer Challenge
The purpose of this challenge is to gauge a backend engineer's ability to interpret and implement the provided project specifications. In this document, you are presented with a scenario that is intended to help showcase your engineering talents and spark creative thinking and problem solving. We will be watching both the journey and the final product.

## Expected Delivery
- A public API to view your execution
- A reviewable copy of the codebase
- Any relevant documentation

## The Rules
- There is no time limit. You are done when you are satisfied - but the client is eager.
- You can use any resource or library that you think is *best for the product*. However, you must be able to justify and attribute any external resource.
- We are great resources! Ask as many questions of the Wonderful team as you would throughout any project. We have been working with this client for many years and can provide feedback or validate any assumptions.

## You will be graded on:
- The elegance, clarity, scalability, and organization of your code
- Your understanding of best practices
- Development Speed v.s. Quality Deliverable
- How easy it would be for another developer to hop into the project and work with you
- Our understanding of the quality of your development process

## Requirements

Our team is being tasked with generating an API that supplies geospatial airport data to an iOS application that helps users map and geographically compare airports around the world. 

Assume that the application is “read heavy”, and does not need to often update the stored airport data (as airports are not often added)
Assume that the API will need to serve an average of 500 requests/second, but that the usage could fluctuate +/-300 requests/second, depending on the time of day.

Assume that the stack for this project is left to your authority, and that any choice of technologies (including database) is up to your discretion.

A CSV document with airport data has been included with this document.


**Problem 1:**

Provide a detailed description of the full stack that you would choose to build this API, complete with descriptive strategies for the following:

- Hosting
- Language
- Framework (if applicable)
- Storage
- Performance
- Misc (anything not covered above)

Also, provide estimates on the scalability and monthly costs of this environment.

**Problem 2:**

Write and document an endpoint that is able to efficiently return a JSON-formatted response of airports within a given radius of a specific coordinate. The iOS-supplied information should be:

- Latitude
- Longitude
- Radius


**Problem 3:**

Write and document an endpoint that is able to return a JSON-formatted response with the distance between two supplied airport id’s. The iOS-supplied information should be:

- Airport 1 ID
- Airport 2 ID


**Problem 4:**

Write and document an endpoint that is able to return a JSON-formatted response with the geographically closest airports between two countries. For example, if tasked to compare the airports in the United States and Mexico, the endpoint would find the 1 airport in each country that is the shortest distance from the airport in the opposite country. The iOS supplied information should be:

- Country 1 Name
- Country 2 Name

**Problem 5:**

Write and document an endpoint that is able to return a JSON-formatted list of instructions as to how to fly the shortest possible route (in terms of airport stops) from one airport to another. When generating these instructions, assume that an airplane can only travel 500 miles before requiring a stop to refuel. Therefore, the returned instructions should read as a list of airport stops, and the distance between each stop. The iOS supplied information should be:

- Airport 1 ID
- Airport 2 ID

✨ Thanks! Good luck!