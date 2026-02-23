# CS465-Full-Stack-Application
CS465 Full Stack Application using MEAN (MongoDB, Eexpress, Angular, and Node)

**Architecture**
***Compare and contrast the types of frontend development you used in your full stack project, including Express HTML, JavaScript, and the single-page application (SPA).
Why did the backend use a NoSQL MongoDB database?***

In this project, I used two types of frontend development which were server rendered pages with Express, and a single page application (SPA) built with Angular. The Express frontend used HTML and JavaScript that were rendered on the server. Each time the user navigated to a new page, the browser reloaded and refreshed the content. In contrast, the Angular SPA dynamically refreshed through API calls. This created a smoother and more modern user experience where the user doesn't need to refresh to see updates.

The backend for this project used MongoDB, which is a NoSQL database that stores data in flexible, JSON-like documents. The reason we used the NoSQL database is because it works well with JavaScript and allows for easy changes to the data structure as the application grows.

**Functionality**
***How is JSON different from Javascript and how does JSON tie together the frontend and backend development pieces?
Provide instances in the full stack process when you refactored code to improve functionality and efficiencies, and name the benefits that come from reusable user interface (UI) components.***

JSON is a format used to send and receive data. It looks similar to JavaScript objects, but it only contains data and not functions. JavaScript is a programming language, while JSON is just a data format. In this project, JSON connects the frontend and backend through the server sending data in JSON format, and the frontend reading that JSON to display information.

During the development of this project, I refactored code several times. For example, we moved hard coded data objects into MongoDB for API calls versus direct storage.
We created a service in Angular to handle API calls instead of continuing to repeat code. We also built reusable UI components like trip cards that essentially created themselves every time a new entry was added to the database. These reusable components make the code easier to maintain, reduce duplication, and make the application easier to expand in the future.

**Testing**
***Methods for request and retrieval necessitate various types of API testing of endpoints, in addition to the difficulties of testing with added layers of security. Explain your understanding of methods, endpoints, and security in a full stack application.***

In this full stack application, the endpoints are URLs where the frontend communicates with the backend (such as /api/trips). I completed most testing using Postman and DBeaver. DBeaver allows us to view and interact with our database and Postman allows us to directly use HTTP methods on our project. 
The HTTP methods that we use for testing are:

* GET – Retrieve data

* POST – Create data

* PUT – Update data

* DELETE – Remove data

I tested these endpoints with Postman to make sure they returned the correct data and status codes, or to see what errors were causing the app to fail. The testing here showed me a lot of issues stemming from outdated documents I was referring to, so I had to change a lot of syntax and code to make the HTTP methods actually work. Eventually we started focusing on security which added another layer of complexity to development. Some endpoints required authentication, meaning users must provide valid credentials or tokens. This ensures that only authorized users can access or modify data. Testing helped confirm both functionality and security.

**Reflection**
***How has this course helped you in reaching your professional goals? What skills have you learned, developed, or mastered in this course to help you become a more marketable candidate in your career field?***

This course helped me understand how the frontend, backend, and database all work together in a full stack application. This project required a lot of troubleshooting, which was pretty difficult toward the end of the project trying to figure out where a problem was stemming from. My professional goal is to become a Software Engineer, so this course directly strengthens my skills in this area. 

I strengthened my skills in:

* Building REST APIs with Express

* Working with MongoDB

* Creating an SPA with Angular

* Connecting frontend and backend using JSON

* Testing API endpoints

* Refactoring code for better organization

Overall, this project improved my confidence in building and understanding complete web applications. It made me more prepared for software engineering roles by giving me hands on experience with real full stack development. The project from this course will increase my marketability as a potential employee for any roles I may apply for.
