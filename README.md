# Restaurant Platform 🍽️

**Full-stack restaurant platform built with React, Express and MongoDB.**

A web application designed to connect customers with small and independent restaurants through food ordering and business funding features. The platform supports separate customer and business functionality, allowing restaurant owners to manage their restaurants and menus while customers can browse, order and contribute donations.

## 📸 Showcase

<!-- Add screenshots or a demo GIF here -->

---

## 🚀 Overview

The Restaurant Platform was developed as a full-stack web application combining a React client with an Express/Node.js backend and MongoDB database.

The project focuses on two sides of the platform:

* **Customers** can browse restaurants, view menus, add items to a basket and make donations.
* **Businesses** can register as restaurant owners, create and manage their restaurants, and manage their menu items.

The application was designed with smaller and independent businesses in mind, combining restaurant ordering with a funding feature that allows customers to support restaurants directly.

---

## ✨ Features

### 👤 Customer Features

* User account registration and authentication.
* Browse available restaurants.
* View individual restaurant information and menus.
* Add menu items to a basket.
* Manage items in the basket before ordering.
* Support restaurants through donations.
* View restaurant funding progress.
* Persistent user session handling.

### 🏪 Business Features

* Register as a business account.
* Create a restaurant profile.
* Add restaurant information and images.
* Edit restaurant details.
* Delete restaurants owned by the account.
* Add menu items with names and prices.
* Edit and remove menu items.
* Manage restaurant-specific data through the application.

### 💰 Restaurant Funding

A key feature of the application is the ability for customers to contribute towards restaurants.

Each restaurant has:

* A funding goal.
* A current funding amount.
* A visible funding progress state.
* Donation functionality for customers.

This adds a second purpose to the platform beyond traditional restaurant ordering and gives customers a way to directly support smaller businesses.

---

## 🧠 Technical Implementation

### Full-Stack Architecture

The application uses a separate frontend and backend structure.

```text
React Client
     │
     │ HTTP requests
     ▼
Express / Node.js API
     │
     │ MongoDB queries
     ▼
MongoDB Database
```

The frontend is responsible for the user interface and application state, while the Express server handles API requests, authentication, business logic and database operations.

### REST API

The backend exposes API routes for functionality such as:

* User authentication
* Restaurant creation and management
* Menu management
* Donations
* Application data retrieval and updates

The frontend communicates with these endpoints to create, retrieve, update and delete application data.

### MongoDB

MongoDB is used to persist application data including:

* User accounts
* Restaurant information
* Menu items
* Funding information
* Other application state

The database structure allows restaurant and user data to be associated with the relevant accounts.

### Authentication & Sessions

User authentication and session handling are implemented on the backend.

The application distinguishes between standard users and business accounts so that restaurant-management functionality is available only to the appropriate users.

API requests involving authenticated functionality use session credentials between the React client and Express server.

### Image Uploads

Restaurant images are handled through the backend using file upload functionality.

Uploaded images are stored and associated with the relevant restaurant rather than requiring the frontend to manage image data directly.

---

## 🛠️ Technology Stack

| Technology       | Purpose                                    |
| ---------------- | ------------------------------------------ |
| **React**        | Frontend user interface                    |
| **JavaScript**   | Application logic                          |
| **Express**      | Backend API framework                      |
| **Node.js**      | Backend runtime                            |
| **MongoDB**      | Database and persistent application data   |
| **Multer**       | Handling image uploads                     |
| **REST API**     | Communication between frontend and backend |
| **HTML / CSS**   | Structure and styling                      |
| **Git / GitHub** | Version control                            |

---

## 📁 Project Structure

The repository separates the main parts of the application:

```text
CreativeWebApp/
├── client/
│   └── React frontend
│
├── server/
│   └── Express / Node.js backend
│
├── views/
│   └── Supporting application views
│
├── package.json
├── package-lock.json
└── README.md
```

The separation between client and server allows the frontend and backend responsibilities to remain independent and makes the application easier to develop and maintain.

---

## 🔄 Example Application Flow

### Customer ordering

```text
User
 │
 ▼
Browse Restaurants
 │
 ▼
Select Restaurant
 │
 ▼
View Menu
 │
 ▼
Add Items to Basket
 │
 ▼
Submit Order
 │
 ▼
Backend API
 │
 ▼
Database
```

### Business management

```text
Business User
 │
 ▼
Sign In
 │
 ▼
Create / Select Restaurant
 │
 ├── Edit Restaurant
 ├── Manage Menu
 ├── Add Menu Items
 └── Remove Menu Items
 │
 ▼
Express API
 │
 ▼
MongoDB
```

---

## 🔐 Data & Access Control

The application separates customer and business functionality.

Business users can manage restaurants associated with their account, while customers use the platform primarily to browse restaurants, interact with menus and support businesses.

This required the application to keep track of the relationship between authenticated users and the restaurants they own.

---

## 🧪 Development & Testing

Development involved testing the application across both frontend and backend functionality.

Areas tested during development included:

* User registration and authentication.
* Customer and business account functionality.
* Restaurant creation, editing and deletion.
* Menu item management.
* Basket functionality.
* Donation functionality.
* MongoDB data persistence.
* API requests between the React client and Express server.
* Image uploads.
* Session handling.
* Cross-origin requests between the frontend and backend.

The application was developed iteratively using Git, allowing individual features and bug fixes to be tracked throughout development.

---

## 🎯 Project Goals

The project was built to provide practical experience with:

* Full-stack web application development.
* React component-based interfaces.
* REST API development.
* Express backend architecture.
* MongoDB database integration.
* Authentication and session management.
* CRUD operations.
* File uploads.
* Persistent application data.
* Managing different user roles and permissions.
* Connecting a frontend application to a backend API.

---

## 📚 What I Learned

Developing this application provided practical experience with building and connecting the different layers of a full-stack application.

Key areas of learning included:

* Designing React components for a multi-feature application.
* Building REST API endpoints with Express.
* Connecting an application to MongoDB.
* Managing authenticated sessions between a frontend and backend.
* Implementing CRUD functionality.
* Handling image uploads with a Node.js backend.
* Managing application state between different user workflows.
* Debugging frontend/backend integration issues.
* Structuring a project into separate client and server responsibilities.

---

## 👨‍💻 Developer

**Callum Candy**

BSc (Hons) Creative Computing — Bath Spa University

[GitHub](https://github.com/lolalolabob123)
