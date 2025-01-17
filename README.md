# React Project + Express.js + PostgreSQL
## Project Description:
This Full-Stack Project which I called MyPlaces with React, Express.js and PostgreSQL is a web application that combines frontend built with React and backend using Express.js and PostgreSQL. Тhe purpose of this application is to create a list of places you want to visit or have already visited. Each place includes a title, the place itself, the country in which it is located, a link with a picture of the place and a short description. The application also allows you to correct information about a place or delete a place as well. 

## Features:
1. Responsive Design: The application is fully responsive, ensuring an optimal viewing experience across a wide range of devices, from desktops to mobile phones.
2. Full-Stack Architecture: Combines a React frontend with an Express.js backend and PostgreSQL database.
3. Places List: Displays a list of places, each with a title, description and the place itself.
4. Place Details View: Provides a detailed view of each place with additional information.

## Technologies Used:
1. Frontend: React.js, JSX, CSS.
2. Backend: Node.js, Express.js.
3. Database: PostgreSQL, Sequelize.
4. State Management: React Hooks.
5. Routing: React Router.
6. Version Control: Git, GitHub.

## Project Structure:
Frontend: Contains all React components and frontend logic.
 1. Components: Components(some of them reusable) for different sections of the project, including Menu.
 2. Pages: Separate pages for Home, Places and Add Place.

Backend: Contains all Express.js server-side code and database logic.
 1. Routes: Define API endpoints for fetching and manipulating project data.
 2. Controllers: Handle the logic for each API endpoint.
 3. Models: Define the PostgreSQL schemas using Sequelize.
 4. Config: Configuration files, including database connection settings.

## To run this project locally, follow these steps:
1. Clone the repository: git clone https://github.com/goshy29/react-express-postgresql.git
2. Open the project with your code editor(VS Code) and open TWO New Terminals
3. At the First Terminal to install Frontend dependencies, in the root directory run: npm install
4. At the Second Terminal to install Backend dependencies, type "cd backend" then run: npm install
5. To start the Frontend development server, in the root directory run: npm start
6. To start the Backend server, in the backend directory run: npm start
7. Ensure PostgreSQL is installed and running
8. Open the application in your browser: http://localhost:3000 

## Example Data to Enter in the User Form: 
1. title: The most visited urban park in the United States
2. place: Central Park, New York
3. country: United States of America
4. image url: https://upload.wikimedia.org/wikipedia/commons/thumb/f/f1/Global_Citizen_Festival_Central_Park_New_York_City_from_NYonAir_%2815351915006%29.jpg/1280px-Global_Citizen_Festival_Central_Park_New_York_City_from_NYonAir_%2815351915006%29.jpg
5. description: Central Park is the fifth-largest park in New York City, behind Pelham Bay Park, the Staten Island Greenbelt, Van Cortlandt Park, and Flushing Meadows–Corona Park, with an area of 843 acres (341 ha; 1.317 sq mi; 3.41 km2).

## PostgreSQL Connection:
You will find this connection code at directory "backend/utils/db-connection.js".

const sequelize = new Sequelize("database", "username", "password", {
    host: "localhost",
    dialect: "postgres"
});

Replace that sequelize connection properties("database", "username", "password") with your own database credentials for PostgreSQL.

**Note: When you start the application for first time, after successfully post a place by you, database table "place" will be automatically created by Sequelize and you are ready to go.**

