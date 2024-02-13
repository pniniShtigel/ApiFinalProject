
README for Diet Club API
Description:

This project is a three-tier API system that simulates a diet club system. The system allows for:

User Authentication: Users can log in to the system using a username and password.
Client Management:
Create new client profiles, including name, height, and weight.
View and edit client details.
Delete a client.
Club Card Management:
View the points balance on a client's club card.
Add points to a client's club card.
Redeem points for rewards.
Architecture:

The system is built using a three-tier architecture:

Presentation Layer: A simple and easy-to-use user interface for managing clients and club cards.
Service Layer: This layer is responsible for the business logic of the system, such as user authentication, client data management, and club card management.
Data Access Layer: This layer is responsible for storing and accessing data using a SQL interface.
Technologies:

Programming Language: Python
Framework: Flask
Database: SQLite
Requirements:

Python 3.7 or above
Pipenv
Installation:

Clone the source code:
git clone https://github.com/bard-ai/diet-club-api.git
Install dependencies:
pipenv install
Run the system:
pipenv run flask run
Usage:

Login endpoint: /api/login

HTTP method: POST
Request body: JSON with username and password
Response: JSON with authentication token (JWT)
Create client endpoint: /api/clients

HTTP method: POST
Request body: JSON with name, height, and weight
Response: JSON with the new client details
Get client details endpoint: /api/clients/{client_id}

HTTP method: GET
Path: client_id - the client identifier
Response: JSON with the client details
Edit client details endpoint: /api/clients/{client_id}

HTTP method: PUT
Path: client_id - the client identifier
Request body: JSON with name, height, and weight
Response: JSON with the updated client details
Delete client endpoint: /api/clients/{client_id}

HTTP method: DELETE
Path: client_id - the client identifier
Response: Empty response
Get points balance endpoint: /api/clients/{client_id}/points

HTTP method: GET
Path: client_id - the client identifier
Response: JSON with the points balance on the club card
Add points endpoint: /api/clients/{client_id}/points

HTTP method: POST
Path: client_id - the client identifier
Request body: JSON with the number of points to add
Response: JSON with the updated points balance
Redeem points endpoint: /api/clients/{client_id}/points/redeem

HTTP method: POST
Path: client_id - the client identifier
Request body: JSON with the number of points to redeem
Response: JSON with the updated points balance and the redeemed reward
Testing:

The system includes unit tests and integration tests to ensure its functionality. To run the tests, use the following command:

pipenv run test
Deployment:

The system can be deployed to any Python web hosting platform that supports Flask.

Documentation:

For more detailed documentation, please refer to the API documentation: [[כתובת URL לא תקינה שהוסרה]]([כתובת URL לא תקינה שהוסרה]).

Contributing:

Contributions to this project are welcome. Please refer to the contributing guidelines: [[כתובת URL לא תקינה שהוסרה]]([כתובת URL לא תקינה שהוסרה]) for more information.
