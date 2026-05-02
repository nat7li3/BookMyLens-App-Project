# BookMyLens

![Node.js](https://img.shields.io/badge/Node.js-18+-green?logo=node.js)
![Express](https://img.shields.io/badge/Express.js-Backend-black?logo=express)
![MySQL](https://img.shields.io/badge/MySQL-Database-blue?logo=mysql)
![License](https://img.shields.io/badge/License-ISC-lightgrey)
![Status](https://img.shields.io/badge/Status-Active-success)

---

## Description

BookMyLens is a full-stack web application designed to streamline the process of discovering, customizing, and booking photography services. The platform allows customers and photographers to create listings, communicate, and negotiate photography packages through an integrated system.

This project demonstrates full-stack development, REST API design, relational database modeling, and user authentication.

---

## Overview

BookMyLens connects customers and photographers through customizable packages, messaging, and negotiation features.

---

## Quick Start

Run the following commands to start the project:

```bash
npm install
node server.js
```

Then open:

```plaintext
home_page.html
```

---

## Features

### Authentication

* Customer and Photographer account creation
* Secure login with password hashing (bcrypt)
* Session handling via browser storage

### Package Builder

* Create customizable photography packages
* Dynamic pricing based on:

  * Add-ons
  * Location
  * Number of people
* Live preview before submission

### Browse Packages

* Filter by category and location
* View community-created packages
* Pre-built event templates

### Messaging System

* Chat between users
* Conversation history
* Linked packages inside chats
* Negotiation via proposals

### Proposal System

* Send and receive offers
* Status tracking:

  * Pending
  * Accepted
  * Rejected
  * Cancelled

---

## Tech Stack

### Frontend

* HTML
* CSS
* JavaScript

### Backend

* Node.js
* Express

### Database

* MySQL

### Dependencies

* express
* mysql2
* bcrypt
* cors
* body-parser

---

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/nat7li3/BookMyLens-App-Project.git
cd BookMyLens-App-Project
```

---

### 2. Install Dependencies

```bash
npm install
```

This will automatically create the `node_modules` folder.

---

### 3. Setup MySQL Database

Make sure MySQL is installed and running.

Run the following command in MySQL:

```sql
CREATE DATABASE software_engineering;
```

Then execute the SQL script provided in:

```plaintext
SQL.txt
```

---

### 4. Configure Database Connection

Open `server.js` and ensure the database credentials match your local MySQL setup:

```js
const db = mysql.createConnection({
    host: 'localhost',
    user: 'root',
    password: 'your_password_here',
    database: 'software_engineering'
});
```

---

### 5. Start the Server

```bash
node server.js
```

You should see:

```plaintext
Server running at http://localhost:3000
```

---

### 6. Run the Frontend

Open the application manually by opening this file in your browser:

```plaintext
home_page.html
```

---

## API Endpoints

### Authentication

```
POST /customer/register
POST /customer/login
POST /photographer/register
POST /photographer/login
```

### Messaging

```
POST /send-message
GET /get-messages
GET /conversations
```

### Packages

```
POST /package/create
GET /packages/browse
```

---

## Project Structure

```plaintext
BookMyLens-App-Project/
│
├── browse_packages.html
├── chat.html
├── create_package.html
├── customer_register.html
├── home_page.html
├── login.html
├── photographer_register.html
├── style.css
├── script.js
├── server.js
├── SQL.txt
├── package.json
├── package-lock.json
├── README.md
```

---

## Security

* Password hashing with bcrypt
* Basic validation on API endpoints

---

## Future Enhancements

* Image uploads for packages
* Payment integration
* Real-time messaging
* Reviews and rating system
* Advanced search filters

---

## Author

Natalie Torres
Alex Upreti
Connor Wade
Andrew Walker
Muhammad Woday

Computer Science Students

---

## License

ISC License

---

## Notes

* The `node_modules` folder is not included in this repository and is automatically generated using `npm install`.
* Ensure MySQL credentials match your local setup before running the server.

---

## Support

If you find this project useful, consider starring the repository.


