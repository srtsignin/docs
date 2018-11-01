# Overview

## Week 9

**Chris and Collin**

- Determined that couchdb was the best fit for our data model based on queries need to be ran
  - Fits well because of nesting document nature of data model
- Determined that the dataservice needed to be written in a fast language due to the massive amounts of data manipulation
- Setup Data-service to expose new REST endpoints for writing data and reading data out as a csv
  - Need to connect a piece to the CSV endpoint for learning Center

**Maya**

- Attached webapp to active user service REST endpoints
- Investigated npm for modularizing the code to be deployed as a native app and a web app
  - This allows us to deploy on multiple platforms trivially

**Connor**

- stuff?

## Week 8

**Chris and Collin**

- Completed endpoints on data service for storing
- Refactored services for adhere to headers for authorization
- Deployed active users service

**Maya**

- Re-wrote frontend to adhere to new namespaces

**Connor**

- Configured new namespaces

## Weeks 6 and 7

**Chris and Collin**

- Implemented Rethink integration
- Configured production Rethink
- Attempted to fix the Card Reader configuration
- Implemented and deployed Cardfire
- Began working on data service

**Maya**

- Deployed web app components as NPM libraries
- Updated tutor page to include option to checkoff students
- Attempted to fix the Card Reader configuration

**Connor**

- Created a UWP app with Ionic
- Deployed web app componenets as NPM libraries

## Weeks 6 and 7

## Week 5

**Chris and Collin**

- Added Redis and Rethink pods to kubernetes
- Created Schema for active user service
- Created Schema for distributing course materials
- Created and migrated spike for distributing course materials
- Moved active user spike endpoints into real active user service
- Started CardFire service integrating with Redis (Not in cluster yet)

**Maya**

- Extracted the web app services and components as libraries into the UI repo
- Published the new UI libraries as npm packages in the @srtsignin organization
- Improved the UI the tutor page that displayed student courses
- Updated the student page to work with the new course schema

## Week 4

**Connor**

- Deployment and build pipelines
- Web app architecture
- Talking to clients and communicating feedback

**Chris and Collin**

- Database and backend services
- RESTful interfaces
- Dockerizing backend

**Maya**

- Initial user interface
- Splitting modules into components and services
- Tweaking UI based on feedback