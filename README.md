# Arthub Web Application

## Project Overview

Arthub is a web application developed as part of an academic project. It is built using the Symfony framework and provides functionalities for user management and blog management. This repository contains my contributions to the project, which include implementing user management features and blog management functionalities.

## Features

### User Management

- **Twilio Integration for Password Reset:**
    - Implemented an API using Twilio to send verification codes via SMS for password reset functionality.
- **reCAPTCHA v2 Integration:**
    - Added reCAPTCHA v2 with a checkbox to enhance security during the login process.
- **Admin User Management:**
    - Developed a datatable using AJAX to view user information efficiently.
    - Implemented a banning system that allows the admin to ban and unban users.

### Blog Management

- **Pagination:**
    - Developed pagination for the blog section using the Symfony pagination bundle to ensure a user-friendly browsing experience.

## Technologies Used

- **Framework:** Symfony
- **API:** Twilio for SMS notifications
- **Security:** reCAPTCHA v2
- **Frontend:** AJAX for dynamic data handling
- **Others:** Symfony pagination bundle for paginated blog views

## Setup Instructions

1. **Clone the Repository:**

    ```sh
    git clone https://github.com/yourusername/arthub.git
    cd arthub
    ```

2. **Install Dependencies:**

    ```sh
    composer install
    npm install
    ```

3. **Configure Environment Variables:**

    Create a `.env.local` file and add the necessary environment variables:

    ```ini
    APP_ENV=dev
    APP_SECRET=your_app_secret
    DATABASE_URL="mysql://user:password@127.0.0.1:3306/database"
    TWILIO_ACCOUNT_SID=your_twilio_account_sid
    TWILIO_AUTH_TOKEN=your_twilio_auth_token
    TWILIO_FROM_NUMBER=your_twilio_from_number
    ```

4. **Run Migrations:**

    ```sh
    php bin/console doctrine:migrations:migrate
    ```

5. **Start the Server:**

    ```sh
    symfony server:start
    ```

## Usage

- **User Registration and Login:**
    - Users can register and log in to the application. In case of a forgotten password, they can request a reset code sent via SMS.
- **Admin Panel:**
    - Admins can log in to access the user management panel, where they can view user details, and ban or unban users.
- **Blog Section:**
    - Users can browse blog posts with paginated views for a better user experience.

## Contribution

This repository includes only my contributions to the project. I was responsible for the following tasks:

- Implementing the Twilio API for password reset.
- Adding reCAPTCHA v2 for login security.
- Developing the user management datatable and banning system.
- Creating the pagination for the blog section.
