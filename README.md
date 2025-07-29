# Mushroom Motors Rental Frontend

Mushroom Motors Rental Frontend is a modern web application designed to streamline the process of vehicle rental for both customers and administrators. Built with React and Vite, it delivers a fast, intuitive, and responsive user experience, enabling users to easily browse, book, and manage vehicle rentals online.

## Overview

This application serves as the customer-facing portal for Mushroom Motors, a vehicle rental service. Users can explore a catalog of available vehicles, view detailed specifications, and make bookings with real-time availability. The platform also provides authenticated users with booking management features and equips administrators with tools to oversee inventory and reservations.

## Key Features

- **Vehicle Catalog:** Browse a diverse selection of vehicles with advanced filtering and search capabilities.
- **Detailed Listings:** Access comprehensive information for each vehicle, including images, specifications, and pricing.
- **Online Booking:** Reserve vehicles for specific dates, with secure authentication and real-time availability checks.
- **Booking Management:** View, modify, or cancel existing reservations through a personalized dashboard.
- **Admin Tools:** Manage vehicle inventory, review bookings, and perform administrative tasks via a dedicated interface.
- **Responsive Design:** Optimized for seamless use on desktops, tablets, and mobile devices.
- **Performance & Reliability:** Built with Vite for rapid development and optimized production builds.

## Technology Stack

- **Frontend:** React, Vite, React Router
- **API Communication:** Axios
- **Styling:** Tailwind CSS
- **Quality Assurance:** ESLint
- **Optional:** TypeScript for type safety

## Getting Started

- **Install dependencies:**  
  `npm install` or `yarn install`
- **Start development server:**  
  `npm run dev` or `yarn dev`
- **Build for production:**  
  `npm run build` or `yarn build`
- **Lint the codebase:**  
  `npm run lint` or `yarn lint`


## Configuration

Create a `.env` file in the project root to specify environment variables such as API endpoints:
```
VITE_API_URL=your backend api 
```

## Contributing

We welcome contributions from the community! Please fork the repository, create a feature branch, and submit a pull request for review.

## License

This project is licensed under the MIT License.


## Environment Variables

Create a `.env` file in the root directory for API endpoints and secrets:
```
VITE_API_URL=https://api.mushroommotors.com
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/my-feature`)
3. Commit your changes (`git commit -am 'Add feature'`)
4. Push to the branch (`git push origin feature/my-feature`)
5. Open a pull request

## License

This project is licensed under the MIT License.


---

Happy renting with Mushroom Motors!


INCREMENTAL PROCESS MODEL FOR MUSHROOM MOTORS CAR RENTAL SYSTEM
-------------------------------------------------------------
Overview of the Model
---------------------
The Incremental Process Model divides the development of the system into smaller, manageable builds (increments). Each increment delivers a functional part of the system, progressively enhancing features until the complete application is ready.
This model is ideal for your Mushroom Motors Rental System because it allows early deployment of core features (vehicle catalogue and booking) while gradually adding advanced functionalities (authentication, admin tools, etc.).

Increments

Increment 1: Core Vehicle Catalogue & Backend Setup

Frontend:
  •	Set up React project with Vite.
  •	Implement Vehicle Catalogue UI (vehicle listing and filtering).
  •	Basic styling with Tailwind CSS.
Backend:
  •	Build Flask API for fetching vehicle data.
  •	Integrate PostgreSQL database schema for Vehicle model.
  •	Provide API endpoint: GET /vehicles (fetch all vehicles).
Output:
  •	Users can browse available vehicles.
  •	Backend serves vehicle data via API.

Increment 2: Booking System & Authentication

Frontend:
  •	Implement Online Booking form with date selection.
  •	Add user authentication (login/register).
  •	Connect frontend booking form to backend API.
Backend:
  •	Create User and Booking models.
  •	Implement JWT-based authentication.
  •	Create booking API endpoints (POST /bookings, GET /bookings/:userId).
Output:
  •	Users can register, log in, and book vehicles.
  •	Bookings are stored securely in the backend.

Increment 3: Booking Management Dashboard

Frontend:
  •	Add dashboard for authenticated users to view, edit, or cancel bookings.
  •	Implement protected routes using React Router.
Backend:
  •	Expand API with booking management endpoints (PUT /bookings/:id, DELETE /bookings/:id).
  •	Enforce role-based access (user vs. admin).
Output:
  •	Users can manage their reservations.
  •	Authentication ensures secure access to personal bookings.

Increment 4: Admin Tools

Frontend:
  •	Add admin interface to manage vehicles (add/edit/remove vehicles).
  •	Integrate admin booking review tools.
Backend:
  •	Implement admin endpoints for managing inventory and viewing all bookings.
  •	Secure routes with admin-only permissions.
Output:
  •	Admins can oversee the fleet and bookings.
  •	Backend enforces role-based permissions.

Increment 5: Performance, QA, and Deployment

Frontend:
  •	Optimize app with code splitting and lazy loading.
  •	Implement ESLint for code quality.
  •	Finalize responsive design.
Backend:
  •	Implement rate limiting and security best practices (Flask middlewares).
  •	Optimize database queries and indexing.
  Deployment:
  •	Host frontend using (., Vercel /Netlify) and backend using (., Railway/Heroku).
  •	Set up CI/CD pipeline.
Output:
  •	Fully functional, optimized, and deployed system.

Technology Stack
  •	Frontend: React, Vite, React Router, Tailwind CSS
  •	Backend: Flask (Python), PostgreSQL, JWT Authentication
  •	API Communication: Axios
  •	Quality Assurance: ESLint
  •	Deployment: Netlify/Vercel (Frontend), Railway/Heroku (Backend)
