# Wanderlust 🌍✈️

Wanderlust is a full-stack web application designed as a vacation rental marketplace (inspired by Airbnb). Users can seamlessly browse unique stays, list their own properties, leave detailed reviews, and manage their profiles securely. The project strictly follows the **MVC (Model-View-Controller)** architecture pattern to ensure clean, decoupled, and scalable code.

---

## 📌 Core Features

* **Complete CRUD Operations:** Users can Create, Read, Update, and Delete property listings (titles, descriptions, images, prices, and locations).
* **Secure User Authentication:** Implemented secure signup and login flows using **JWT (JSON Web Tokens)** to protect private routes and manage stateless sessions.
* **Interactive Review System:** Authenticated users can leave star ratings and text reviews on individual listings, which dynamically update the user interface.
* **Dynamic Server Routing:** Robust RESTful API backend routes designed to manage listings, users, and reviews securely.
* **Responsive Server-Side Rendering:** A fully responsive frontend rendered dynamically on the server side to support all screen types (mobile, tablet, desktop).

---

## 🛠️ Tech Stack & Architecture

### Backend & Database
* **Node.js & Express.js:** Server-side runtime environment and framework handling the RESTful API routing, cookies, and middleware pipelines.
* **MongoDB Atlas:** Cloud NoSQL database storing user profiles, listing schemas, and review models with relational data mapping via **Mongoose**.
* **JWT (JSON Web Tokens):** Handles stateless user session authorization and backend route protection middleware.

### Frontend
* **EJS (Embedded JavaScript Templates):** Used for rendering dynamic HTML pages directly from the backend server with injected database variables.
* **HTML5 & CSS3:** Structured layout with custom styling, flexbox grids, and interactive interactive UI transitions.
* **JavaScript (ES6+):** Client-side scripts handling front-end UI interactions, interactive validations, and async form handling.

---

## 🗺️ Database Schema Design

The data is organized into three interconnected MongoDB collections using Mongoose object referencing:
1. **User Schema:** Stores unique usernames, encrypted passwords, and registered emails.
2. **Listing Schema:** Stores property details (title, description, image URL, price, location, country) along with an array of **Review ObjectIDs** and an **Owner ObjectID**.
3. **Review Schema:** Stores comments, star ratings (1-5), and the **Author ObjectID**.

---

## 🚀 Local Installation & Setup

To run Wanderlust locally on your machine, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-github-username/Wanderlust.git](https://github.com/your-github-username/Wanderlust.git)
