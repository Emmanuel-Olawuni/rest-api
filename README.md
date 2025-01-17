# Simple REST API with Laravel

This project is a simple RESTful API built using Laravel. It includes authentication, CRUD operations for managing posts, and proper error handling. The API is secured using JWT authentication, and only authorized users can perform certain actions.

---

## Features

-   **User Authentication**:

    -   Register new users.
    -   Login and receive a JWT token.
    -   Logout users and invalidate tokens.

-   **CRUD Operations**:

    -   Create, Read, Update, and Delete posts.
    -   Only the post creator can update or delete their posts.

-   **Error Handling**:

    -   Validation errors for incorrect input.
    -   Unauthorized access and permissions.

-   **Optional**:
    -   Rate limiting to prevent API abuse.
    -   User activity logging.

---

## Requirements

-   PHP >= 8.0
-   Composer
-   Laravel >= 9.x
-   MySQL or any supported database
-   Postman (for testing endpoints)

---

## Installation

1.  **Clone the Repository**:
    ```bash
    git clone https://github.com/emmanuel-olawuni/rest-api.git
    cd rest-api
    ```
2.  **Install Dependencies:**

    ```bash
    composer install
    ```

3.  **Set Up Environment:**

    ```bash
        cp .env.example .env
    ```

    Update the .env file with your database credentials:

     ```bash
        DB_CONNECTION=mysql
        DB_HOST=127.0.0.1
        DB_PORT=3306
        DB_DATABASE=your_database
        DB_USERNAME=your_username
        DB_PASSWORD=your_password
    ```

4.  **Generate App Key**:
    ```bash
      php artisan key:generate
    ```
5.  **Run Migrations:**
    ```bash
      php artisan migrate
    ```
6.  **Set Up JWT Secret:**:
    ```bash
       php artisan jwt:secret
    ```
7.  **Start the Server:**
    ```bash
        php artisan serve
    ```

**Video URL**
The video is uploaded on google drive [https://drive.google.com/file/d/1vHaBAGRvx9JMvuA62Z_6gDYlAP06cfC7/view?usp=sharing](https://drive.google.com/file/d/1vHaBAGRvx9JMvuA62Z_6gDYlAP06cfC7/view?usp=sharing)
