# Online Store Category Management API

This project is a RESTful API for managing categories in an online store. It utilizes Laravel's nested set model for category organization and stores the data in a MySQL database. The API responses are in XML format.

## Installation

1. Clone the repository:

git clone <repository-url>



2. Install the dependencies using Composer:

composer install


3. Create a MySQL database named "online_store".

4. Configure the database connection in the `.env` file. Set the appropriate values for `DB_HOST`, `DB_PORT`, `DB_DATABASE`, `DB_USERNAME`, and `DB_PASSWORD`.

5. Run the database migrations to create the necessary tables:

php artisan migrate


6. Start the development server:

php artisan serve


The API will now be accessible at `http://localhost:8000`.

## API Endpoints

- `GET /categories`: Retrieve all categories in XML format.
- `GET /categories/{id}`: Retrieve a specific category by its ID in XML format.
- `POST /categories`: Create a new category. Accept XML request payload with name and parent_id fields. Return the created category in XML format.
- `PUT /categories/{id}`: Update an existing category by its ID. Accept XML request payload with name field. Return the updated category in XML format.
- `DELETE /categories/{id}`: Delete a category by its ID. Return a success message in XML format.

## Error Handling

The API handles invalid requests and returns appropriate error responses in XML format. Ensure to validate the request data and handle exceptions to provide meaningful error messages to the clients.

## Unit Tests

Unit tests are included to cover the functionality of the API endpoints. You can run the tests using the following command:

php artisan test


## Sample Categories

Sample categories have been created in the database for testing purposes. You can use them as a starting point or modify them according to your requirements.


