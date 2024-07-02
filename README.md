# HNG-11-Backend-Stage-1 My Vercel Node.js API

This project is a simple Node.js server using Express that provides a greeting API endpoint. It is hosted on Vercel and demonstrates basic deployment and usage of a Node.js application on a serverless platform.

Features
Greeting API Endpoint: Responds with a personalized greeting message.
IP Address Reporting: Returns the client’s IP address.
Static Location: Provides a hardcoded location for demonstration purposes.
Live Demo
The live version of this project is hosted on Vercel and can be accessed here:

Live Demo

API Usage
Endpoint: /api/hello
Returns a greeting message with the visitor’s name and the client IP address.

Request:

http
GET /api/hello?visitor_name=<YourName>
Response:

json
{
  "client_ip": "127.0.0.1",
  "location": "New York",
  "greeting": "Hello, <YourName>! The temperature is 11 degrees Celsius in New York."
}

Example Request
http
GET https://my-vercel-ck14v9q3w-maxsights-projects.vercel.app/api/hello?visitor_name=Mark

Example Response
json
{
  "client_ip": "203.0.113.42",
  "location": "New York",
  "greeting": "Hello, Mark! The temperature is 11 degrees Celsius in New York."
}
Project Setup
Prerequisites
Node.js
npm (Node Package Manager)
Installation
Clone the repository:

bash
git clone https://github.com/maxsights-projects/my-vercel-app.git
cd my-vercel-app
Install the dependencies:

bash
npm install
Local Development
To run the server locally, use:

bash
npm start
The server will run on http://localhost:3000.

Deployment
This project is deployed to Vercel. To deploy your own version, follow these steps:

Install the Vercel CLI:

bash
npm install -g vercel
Log in to Vercel:

bash
npx vercel login
Deploy to Vercel:

bash
npx vercel
Follow the prompts to complete the deployment.

Configuration
The Vercel deployment is configured using vercel.json. The server code is located in the api directory.

Contributing
Feel free to submit pull requests or open issues to contribute to this project.

License
This project is licensed under the MIT License. See the LICENSE file for more details.

