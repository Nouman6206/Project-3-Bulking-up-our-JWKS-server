# Project-3-Bulking-up-our-JWKS-server
Setup Environment:

Make sure you have Python installed on your system. You can download Python from the official website: https://www.python.org/downloads/
Additionally, ensure that you have the required libraries installed. You can install them using pip:
Copy code
pip install Flask flask-limiter passlib argon2-cffi cryptography pyjwt
Database Setup:

The code uses SQLite for the database. No additional setup is needed as SQLite comes bundled with Python.
The code automatically creates the necessary tables (keys, users, auth_logs) if they don't exist.
Environment Variable:

Set up an environment variable named NOT_MY_KEY with a secret key value for encryption and decryption. This key should be kept confidential.
Run the Server:

Navigate to the directory containing your Python script (main.py) using the command line or terminal.
Run the Python script to start the server:
css
Copy code
python main.py
The server will start running on http://localhost:8080.
Interact with the Server:

Once the server is running, you can send HTTP requests to it using tools like cURL, Postman, or by writing your client code.
Example routes:
GET /example: Returns a simple message.
POST /auth: Handles authentication requests (modify as per your requirements).
POST /register: Handles user registration (modify as per your requirements).
Testing:

You can test the functionality of the server by sending requests to the defined endpoints and checking the responses.
Make sure to handle exceptions and errors appropriately in your client code.
Shutdown the Server:

To stop the server, you can either press Ctrl + C in the terminal where the server is running or send a shutdown request to the server endpoint.
Additional Notes:

Ensure that your system allows incoming and outgoing connections on port 8080 to run the server locally.
Modify the server code (main.py) as needed for your specific application logic, such as handling user registration, authentication, logging, etc.
