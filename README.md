# Academic-Project-Web-
Arthub is a web application developed as part of an academic project using the Symfony framework. My contributions include user management and blog management features. 

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Arthub Web Application</title>
</head>
<body>
    <h1>Arthub Web Application</h1>

    <h2>Project Overview</h2>
    <p>Arthub is a web application developed as part of an academic project. It is built using the Symfony framework and provides functionalities for user management and blog management. This repository contains my contributions to the project, which include implementing user management features and blog management functionalities.</p>

    <h2>Features</h2>
    <h3>User Management</h3>
    <ul>
        <li><strong>Twilio Integration for Password Reset:</strong> Implemented an API using Twilio to send verification codes via SMS for password reset functionality.</li>
        <li><strong>reCAPTCHA v2 Integration:</strong> Added reCAPTCHA v2 with a checkbox to enhance security during the login process.</li>
        <li><strong>Admin User Management:</strong> Developed a datatable using AJAX to view user information efficiently. Implemented a banning system that allows the admin to ban and unban users.</li>
    </ul>

    <h3>Blog Management</h3>
    <ul>
        <li><strong>Pagination:</strong> Developed pagination for the blog section using the Symfony pagination bundle to ensure a user-friendly browsing experience.</li>
    </ul>

    <h2>Technologies Used</h2>
    <ul>
        <li><strong>Framework:</strong> Symfony</li>
        <li><strong>API:</strong> Twilio for SMS notifications</li>
        <li><strong>Security:</strong> reCAPTCHA v2</li>
        <li><strong>Frontend:</strong> AJAX for dynamic data handling</li>
        <li><strong>Others:</strong> Symfony pagination bundle for paginated blog views</li>
    </ul>

    <h2>Setup Instructions</h2>
    <ol>
        <li><strong>Clone the Repository:</strong>
            <pre><code>git clone https://github.com/yourusername/arthub.git
cd arthub</code></pre>
        </li>
        <li><strong>Install Dependencies:</strong>
            <pre><code>composer install
npm install</code></pre>
        </li>
        <li><strong>Configure Environment Variables:</strong>
            <pre><code>Create a .env.local file and add the necessary environment variables:
APP_ENV=dev
APP_SECRET=your_app_secret
DATABASE_URL="mysql://user:password@127.0.0.1:3306/database"
TWILIO_ACCOUNT_SID=your_twilio_account_sid
TWILIO_AUTH_TOKEN=your_twilio_auth_token
TWILIO_FROM_NUMBER=your_twilio_from_number</code></pre>
        </li>
        <li><strong>Run Migrations:</strong>
            <pre><code>php bin/console doctrine:migrations:migrate</code></pre>
        </li>
        <li><strong>Start the Server:</strong>
            <pre><code>symfony server:start</code></pre>
        </li>
    </ol>

    <h2>Usage</h2>
    <ul>
        <li><strong>User Registration and Login:</strong> Users can register and log in to the application. In case of a forgotten password, they can request a reset code sent via SMS.</li>
        <li><strong>Admin Panel:</strong> Admins can log in to access the user management panel, where they can view user details, and ban or unban users.</li>
        <li><strong>Blog Section:</strong> Users can browse blog posts with paginated views for a better user experience.</li>
    </ul>

    <h2>Contribution</h2>
    <p>This repository includes only my contributions to the project. I was responsible for the following tasks:</p>
    <ul>
        <li>Implementing the Twilio API for password reset.</li>
        <li>Adding reCAPTCHA v2 for login security.</li>
        <li>Developing the user management datatable and banning system.</li>
        <li>Creating the pagination for the blog section.</li>
    </ul>

    <h2>License</h2>
    <p>This project is licensed under the MIT License.</p>
</body>
</html>
