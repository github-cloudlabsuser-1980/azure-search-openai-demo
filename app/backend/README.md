API Overview
This API is built using Flask, a popular Python web framework. It provides the following functionality:
•	Serving static files: The API allows users to access static files such as HTML, CSS, and JavaScript files.
•	User authentication: The API supports authentication using Azure Active Directory. Users can log in and access protected routes.
•	File upload and deletion: Users can upload files to the server and delete their uploaded files.
•	Chat-based interactions: The API provides endpoints for performing chat-based interactions using different approaches.
Routes
The API exposes the following routes:
•	/: This route serves the main HTML file for the application.
•	/redirect: This route is used for login redirect purposes.
•	/favicon.ico: This route serves the favicon file.
•	/assets/<path:path>: This route serves static assets such as images, CSS, and JavaScript files.
•	/content/<path>: This route serves content files from blob storage. It supports access control based on user authentication.
•	/ask: This route is used for performing chat-based interactions using a specific approach.
•	/chat: This route is used for performing chat-based interactions using different approaches.
•	/auth_setup: This route provides MSAL.js settings for the client UI.
•	/config: This route provides configuration options for the client UI.
•	/upload: This route allows users to upload files to the server.
•	/delete_uploaded: This route allows users to delete their uploaded files.
•	/list_uploaded: This route lists the files uploaded by the user.
Dependencies
The API relies on several dependencies, including:
•	Azure SDK: The API uses various Azure SDKs for interacting with Azure services such as Blob Storage, Data Lake, Key Vault, and Search.
•	OpenAI: The API integrates with OpenAI for chat-based interactions.
•	Quart: Quart is a Python web framework based on Flask. It is used to implement the API.
•	Quart-CORS: This package provides Cross-Origin Resource Sharing (CORS) support for Quart.
Configuration
The API requires the following configuration settings:
•	Azure Storage Account: The name of the Azure Storage Account used for storing files.
•	Azure Storage Container: The name of the Azure Storage Container used for storing files.
•	Azure User Storage Account: The name of the Azure Storage Account used for storing user-specific files.
•	Azure User Storage Container: The name of the Azure Storage Container used for storing user-specific files.
•	Azure Search Service: The name of the Azure Search Service used for search functionality.
•	Azure Search Index: The name of the Azure Search Index used for search functionality.
•	Azure Search Secret Name: The name of the secret in Azure Key Vault that contains the Azure Search API key.
•	Azure Key Vault Name: The name of the Azure Key Vault used for storing secrets.
•	Other configuration options related to different approaches and features.
Please make sure to configure these settings before running the API.
Getting Started
To run the API, follow these steps:
1.	Install the required dependencies by running pip install -r requirements.txt.
2.	Set the necessary environment variables or update the configuration settings in the code.
3.	Run the API using the command python app.py.
4.	Access the API endpoints using a web browser or API testing tool.
Make sure to replace the placeholder values with your own values where applicable.
Contributing
Contributions to this API are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.
License
This API is licensed under the MIT License.