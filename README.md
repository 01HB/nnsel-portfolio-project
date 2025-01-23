# A Simple Portfolio Management Website
### Overview
<p>
  This is a Portfolio Management Website built using Next.js for the frontend and NestJS for the backend. 
  It provides functionalities to display portfolio projects with a responsive UI and a dashboard to manage 
  (add, update, delete) projects dynamically via RESTful APIs and persisting the data in a Postgres database.
</p>

## Key Features
### Frontend:
Pixel-perfect design based on a Figma file.
Fully responsive layout for seamless usability on all devices.
Styled with Tailwind CSS.
<br /><br />
### Backend:
RESTful API endpoints for fetching and managing project data.
A simple dashboard to manage portfolio projects (CRUD operations).
Organized structure for easy maintenance and scalability


## Getting Started
### Follow these steps to set up and run the project locally.

### Prerequisites
<ul>
  <li>Node.js (v18 or higher)</li>
  <li>npm or yarn</li>
  <li>PostgreSQL</li>
  <li>Git</li>
</ul>

### Setting Up the NestJS Back-end:
#### Navigate to the NestJS Backend Repository and clone it. Then install dependencies:
```
npm install
```

#### Create a .env file in the backend directory with the following variables:
```
DATABASE_HOST=localhost
DATABASE_PORT=5432
DATABASE_USER=your_username
DATABASE_PASSWORD=your_password
DATABASE_NAME=portfolio_db
```

<br /><br />

### Setting Up the NextJS Front-end:
#### Navigate to the Front-end Repository and clone it. Then run:
```
npm install
```

#### Create a .env.local file in the frontend directory with the following variables:
```
NEXT_PUBLIC_BACKEND_URL=http://localhost:9000
```


#### Running the Entire Application
Open two terminals <br />
One for the frontend (npm run dev) <br />
One for the backend (npm run start:dev) <br />
Visit http://localhost:3000 in your browser to view the application. <br />

<br /><br />

### API Endpoints:
#### Projects-
GET /projects/view/all (view all projects) <br />
GET /projects/view/:projectid (view details of a specific project) <br />
POST /projects/create (create a new project) <br />
PUT /projects/update/:projectid (update a specific project) <br />
DELETE /projects/delete/:projectid (delete a project) <br />

<br /><br />
