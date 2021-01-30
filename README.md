# Incident API Endpoints PHP 7.4 Laravel
Incident API Endpoints

What is Incident Management?



An incident is an event that could lead to loss of, or disruption to, an organization's operations, services or functions. Incident management is a term describing the activities of an organization to identify, analyze, and correct hazards to prevent a future re-occurrence.



Application



Design and develop simple Incident Rest API endpoints with GET and POST requests. Using the Laravel or SLIM framework & Symphony components. Php Unit framework needs to be used for Unit testing of the APIs



Routes

GET /incidents - Retrieve Data

POST /incidents - Store JSON Data
Json Input Parameters



- Location Geocode ( Object Lat and Long ) 



- Incident Title ( String )



- Category of Incident.

Category ID => 1 = Security

Category ID => 2 = Health & Safety

Category ID => 2 = Loss Prevention



- People Involved ( Object )

 - Name

 - Type ( staff, witness )

 

- Comments ( Text String )

- Incident Time ( Date Time )

- Update Time ( Date Time )

- Create Time ( Date Time )



Project Requirements

Incident Json format POST
https://run.mocky.io/v3/c840350a-b9a9-4dd5-8645-f572e81fea96

Incident Json format GET
https://run.mocky.io/v3/58e7aa93-39ab-4360-88cf-d2242a0dbc80

POST endpoint should create a new incident

Validations:
If Location details are empty or invalid throw error response
Category ID is empty or invalid throw error
incident time is invalid throw error response
Update time and Created time if empty pick the current time.

GET endpoint should retrieve a list of incidents

Dependency Injection - Use Symfony dependency injection for locating controllers for Development and production environment.

Dependency Injection - for setting parameters for the Dev and Production environment.

Storage MYSQL or Redis

DB architecture of your choice

Migrations to seed data & setup DB
Deployment

Github Repo for code
Composer install
Readme File with instructions on how to run the project
