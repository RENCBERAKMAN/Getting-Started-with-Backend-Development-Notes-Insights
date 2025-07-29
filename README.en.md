<p align="center">
  <img src="https://img.icons8.com/external-flaticons-lineal-color-flat-icons/64/000000/external-coding-web-development-flaticons-lineal-color-flat-icons.png" alt="Coding Icon" />
</p>

## 🔍 What does a backend developer do, and how is it different from frontend?
A backend developer works on the parts of a software or web application that users don’t see. That includes the logic behind the scenes, data management, user sessions, security, APIs, and database operations.

While frontend developers build the interface users interact with, backend developers make sure that this interface works properly by handling the data and logic it needs.

For example, when a user submits a form, it’s the backend system that processes that data — validating, storing, and sometimes analyzing it.

I personally chose the backend path because I enjoy working with logic and data. Solving complex problems and building the foundation of a system feels more meaningful and exciting to me.
<hr style="border: 2px solid #4CAF50; margin: 20px 0;">

## 🔍 What is a REST API and what is it used for?
A REST API is a structure that allows different systems to communicate with each other. It's especially used so the frontend and backend can exchange data.

REST stands for "Representational State Transfer" and works over the HTTP protocol. An API is like a communication gateway that lets an application talk to the outside world.

✅For example, when a user wants to view a list of products through the app interface, the frontend sends this request to the backend via a REST API. The backend receives the request, processes it, fetches the data from the database, and sends it back to the frontend.

Thanks to REST APIs, systems can work independently from each other. This makes the software easier to scale and manage.
<hr style="border: 2px solid #4CAF50; margin: 20px 0;">

## 🔍 What are HTTP methods? What are they used for? (GET, POST, PUT, DELETE)
HTTP methods allow a client (usually the frontend) to tell the server (backend) what action it wants to perform.

Here’s a brief explanation of the four most commonly used HTTP methods:

GET: Used to retrieve data from the server. For example, when we want to view a list of products, the frontend sends a GET request to the backend.

POST: Used to send and save new data to the server. For instance, submitting a registration form is done via a POST request.

PUT: Used to completely update existing data. For example, updating a user's profile information is done using PUT.

DELETE: Used to delete specific data from the server. For example, deleting a user account.

✅These methods help ensure clear and organized communication between the frontend and backend. In REST APIs, we use these methods to perform different operations in a standardized way.
<hr style="border: 2px solid #4CAF50; margin: 20px 0;">

## 🔍 What is the difference between POST and PUT?
Both POST and PUT are used to send data to the server, but their purposes and typical use cases are different.

POST is usually used to create new data. For example, when submitting a user registration form, we use POST. The server creates a new user.

PUT is used to update existing data. For instance, if we want to change a user’s email address, we use PUT.

One key difference is:

POST can create a new record every time it is called (like a new object with a different ID).

PUT updates the content of an existing record with a specific ID, keeping the ID the same.

✅In short:
→ POST = Create.
→ PUT = Update.

<hr style="border: 2px solid #4CAF50; margin: 20px 0;">
## 🔍 What is Stateless Architecture?
A stateless architecture means that each request from a client to a server is independent. The server does not remember any previous requests.

Every request must contain all necessary information (like authentication data and parameters), because the server treats each request as if it comes for the first time.
Example:
Think of a REST API. Every GET or POST request must include information like who you are and what you want. Even if the server responded to your previous request, it won't remember it for the next one.
✅Benefits:
The server becomes scalable, as it doesn’t store user sessions.
Load balancing is easier.
The system is faster, simpler, and easier to maintain.
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=footer&text=Thanks%20for%20visiting!%20🚀&fontSize=30&fontColor=ffffff" />
</p>
