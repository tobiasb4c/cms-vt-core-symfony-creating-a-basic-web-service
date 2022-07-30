# CMS-VT | CORE | Symfony - Creating a basic web service

## Overview
The Philosophical Apprentice Circle (PAC) is a club consisting of people who enjoy discussing philosophical questions. They approached your company to create a web service as basis for their own and the publics philosophical discussions on time travel.
For this purpose, users should be able to retrieve a random scenario from the web to discuss it. Specific administrators should have the possibility to add, edit and remove resources. As the PAC wants to remain very open for custom client implementations, they want you to generate this scenario as a web service.

## User Story 1
*As an ADMINISTRATOR I want to be able to add new time machine resources to the database, so that the public can query for them later*

### Acceptance Criteria
- A model for a time machine entry exists
  - Name
  - Resource URL
- A controller and according route which stores a new entry exists
  - The controller accepts POST requests
  - The controller accepts a JSON object as parameter which is auto converted to a time machine entry
- An authentication check is not mandatory at this point in time.

## User Story 2
*As an ADMINISTRATOR I want to add test entries to the persistence layer, so that I can test querying entries later.*

### Acceptance Criteria
- Two demonstration entries exist in the database
  - XKCD Comic – Kill Hitler: https://xkcd.com/1063/ 
  - YouTube Song – Time Machine: https://www.youtube.com/watch?v=8zwEnNJumQ4 

## User Story 3
*As a USER I want to retrieve a random entry from the database, so that I can start a philosophical discussion on it.*

### Acceptance Criteria
- A controller and according route which retrieve a random time machine entry exists
- The response is returned as JSON object

#### Links
https://my.skilldisplay.eu/en/skillset/116
