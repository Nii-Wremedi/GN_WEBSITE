# GN Group Website

This is the official website for **GN Group**, which includes **GN Incorporated** and **GN Ventures Inc.**. The website provides information about the company, its services, subsidiaries, and allows users to contact the company directly via a form.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup Instructions](#setup-instructions)
- [Environment Variables](#environment-variables)
- [Usage](#usage)
- [Testing Contact Form Locally](#testing-contact-form-locally)
- [Folder Structure](#folder-structure)
- [License](#license)

---

## Project Overview

GN Group’s website is designed to:

- Showcase company information and subsidiaries
- Provide a modern, responsive UI for users on desktop and mobile
- Allow users to send messages to the company via a contact form
- Maintain a consistent navigation menu and footer across all pages

---

## Features

- **Responsive Navbar** with mobile hamburger menu
- **Dedicated pages** for GN Incorporated and GN Ventures Inc.
- **Contact form** that sends emails directly to the company
- **Footer** with company info and quick links
- **Tailwind CSS** for modern, responsive design
- **Node.js backend** using Express and Nodemailer for email submissions

---

## Technologies Used

- **Frontend:** HTML, Tailwind CSS, JavaScript
- **Backend:** Node.js, Express.js, Nodemailer
- **Other Tools:** Body-parser, dotenv

---

## Setup Instructions

1. **Clone the repository:**

```bash
git clone <your-repo-url>
cd GN_Website

```

Create a .env file inside backend/:

EMAIL_USER=yourgmail@gmail.com
EMAIL_PASS=your_app_password
EMAIL_TO=recipient@gmail.com
PORT=5000

Start the backend server:

node server.js

Open frontend pages in a browser (e.g., index.html) and test the contact form.

Environment Variables
Variable Description
EMAIL_USER Gmail address used to send emails
EMAIL_PASS Gmail App Password (required if 2FA is enabled)
EMAIL_TO Recipient email for contact form submissions
PORT Port number for the backend server (default: 5000)
Usage

Homepage: Provides general info and links to subsidiary pages

Subsidiary Pages: Detail GN Incorporated and GN Ventures Inc. services

Contact Form: Users can submit messages, which are emailed via Nodemailer

Testing Contact Form Locally

Ensure your backend server is running:

cd backend
node server.js

Open contact_us.html in your browser.

Fill in the Name, Email, and Message fields.

Click Send.

If successful, the server console will display:

Server running on http://localhost:5000

You should receive the email at the address specified in EMAIL_TO.

✅ Tip: Use a tool like Mailtrap for testing emails safely if you don’t want to send real emails.

Folder Structure
GN_Website/
│
├── backend/
│ ├── server.js
│ ├── package.json
│ ├── package-lock.json
│ └── .env
│
├── index.html
├── GN_INCORPORATED.html
├── GN_VENTURES.html
├── contact_us.html
└── assets/ (images, logos, etc.)
