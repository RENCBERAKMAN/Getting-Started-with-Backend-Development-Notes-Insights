<p align="center">
  <img src="https://img.icons8.com/external-flaticons-lineal-color-flat-icons/64/000000/external-coding-web-development-flaticons-lineal-color-flat-icons.png" alt="Coding Icon" />
</p>

## 🔍 What does a backend developer do, and how is it different from frontend?
A backend developer works on the parts of a software or web application that users don’t see. That includes the logic behind the scenes, data management, user sessions, security, APIs, and database operations.

While frontend developers build the interface users interact with, backend developers make sure that this interface works properly by handling the data and logic it needs.

For example, when a user submits a form, it’s the backend system that processes that data — validating, storing, and sometimes analyzing it.

I personally chose the backend path because I enjoy working with logic and data. Solving complex problems and building the foundation of a system feels more meaningful and exciting to me.

<hr style="border: 5px solid #4CAF50; margin: 20px 0;">


## 🔍 What is a REST API and what is it used for?
A REST API is a structure that allows different systems to communicate with each other. It's especially used so the frontend and backend can exchange data.

REST stands for "Representational State Transfer" and works over the HTTP protocol. An API is like a communication gateway that lets an application talk to the outside world.

✅For example, when a user wants to view a list of products through the app interface, the frontend sends this request to the backend via a REST API. The backend receives the request, processes it, fetches the data from the database, and sends it back to the frontend.

Thanks to REST APIs, systems can work independently from each other. This makes the software easier to scale and manage.

<hr style="border: 5px solid #4CAF50; margin: 20px 0;">


## 🔍 What are HTTP methods? What are they used for? (GET, POST, PUT, DELETE)
HTTP methods allow a client (usually the frontend) to tell the server (backend) what action it wants to perform.

Here’s a brief explanation of the four most commonly used HTTP methods:

GET: Used to retrieve data from the server. For example, when we want to view a list of products, the frontend sends a GET request to the backend.

POST: Used to send and save new data to the server. For instance, submitting a registration form is done via a POST request.

PUT: Used to completely update existing data. For example, updating a user's profile information is done using PUT.

DELETE: Used to delete specific data from the server. For example, deleting a user account.

✅These methods help ensure clear and organized communication between the frontend and backend. In REST APIs, we use these methods to perform different operations in a standardized way.

<hr style="border: 5px solid #4CAF50; margin: 20px 0;">


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

<hr style="border: 5px solid #4CAF50; margin: 20px 0;">

## 🔍 What is Stateless Architecture?
A stateless architecture means that each request from a client to a server is independent. The server does not remember any previous requests.

Every request must contain all necessary information (like authentication data and parameters), because the server treats each request as if it comes for the first time.
Example:
Think of a REST API. Every GET or POST request must include information like who you are and what you want. Even if the server responded to your previous request, it won't remember it for the next one.
✅Benefits:
The server becomes scalable, as it doesn’t store user sessions.
Load balancing is easier.
The system is faster, simpler, and easier to maintain.

<hr style="border: 5px solid #4CAF50; margin: 20px 0;">

## 🔍What is the MVC(Model-View-Controller) Architecture and Why is it Used?

MVC is a software architecture divided into three main components:

Model (Data and Business Logic)
Contains all the data, rules, and business logic of the application. Communication with the database, data processing, and rules are handled in this layer.

View (User Interface)
This is the interface with which the user interacts. Visual designs, buttons, forms—everything displayed to the user—belongs to this layer.

Controller
Handles requests from the user, communicates with the appropriate Model, and sends the result to the View. In essence, it acts as a bridge between the Model and the View.

-----✅WHY USE MVC?-----
1. Separation of Concerns
Each component has its own responsibility. This makes the code more understandable, organized, and easier to maintain. For example, if the interface changes, updating just the View is enough.

2. Improved Testability
Since the Model and Controller are separate, it's easier to test individual units. This is a big advantage in large projects where automated testing is important.

3. Reusability
The same data (Model) can be used with different interfaces (View) multiple times. For example, the same user information can be displayed in different ways on different pages.

4. Facilitates Parallel Development in Teams
While frontend developers work on the View, backend developers can work on the Model and Controller. This increases team productivity.

5. Scalable Architecture
As the application grows, it's easier to expand parts or add new components. It's especially ideal for projects that require modular design.

<hr style="border: 5px solid #4CAF50; margin: 20px 0;">


## 🔍What are Request and Response?
Request and Response define the communication between the client and the server in web-based systems. A Request is the message sent by the client to the server. This request typically includes actions such as viewing a page, sending data, or retrieving information. For example, when a user accesses a website, the browser sends a GET request to the server to retrieve the page content.

Once the server receives this request, it processes it and sends back a Response. This response could be an HTML page, a JSON object, an error message, or any other type of result.

In short: a Request represents the client's demand, while a Response is the server's reply to that demand. This pair forms the foundation of modern web applications. Communication usually takes place over the HTTP or HTTPS protocols, and each step follows specific rules.

Thanks to this structure, the actions users perform through a browser can be understood, processed, and responded to by the server.
<p align="center">

<hr style="border: 5px solid #4CAF50; margin: 20px 0;">



## 🌐 HTTP Status Codes (200, 201, 400, 401, 403, 404, 500)
HTTP status codes are numerical indicators that show how a request from the client was handled by the server.
Each code indicates whether the request was successful, contained errors, or requires further action.

200 – OK
The request was successfully processed, and the server returned the expected response.
Example: When requesting a product list, the server returns the list in JSON format.

201 – Created
The request was successful, and the server created a new resource.
Example: Submitting a registration form that results in a new user being created.

400 – Bad Request
The request is invalid, incomplete, or cannot be understood by the server.
Example: Submitting a form with required fields left empty.

401 – Unauthorized
Authentication has not been provided or is invalid. Valid credentials are required for access.
Example: Sending a request to a protected API without logging in.

403 – Forbidden
Authentication is provided but the user does not have permission to access the resource.
Example: A regular user attempting to access the admin panel.

404 – Not Found
The requested resource could not be found on the server.
Example: Navigating to a non-existent URL.

500 – Internal Server Error
The server encountered an unexpected error while processing the request.
Example: A coding error or a database connection failure.

✅ Summary:

2xx → Successful operations

4xx → Client-side errors

5xx → Server-side errors
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=footer&text=Thanks%20for%20visiting!%20🚀&fontSize=30&fontColor=ffffff" />
</p>
