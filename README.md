# User Profile Management System

This project is a simple user management system allowing users to register, log in, update their profiles, and view a personalized homepage. The application is built with PHP and SQLite and uses Quill as a rich text editor for user self-introductions.

## Features

- **User Registration**: Users can register with a unique username, email, password, and an optional profile image. Passwords are validated to meet specific security criteria.
- **User Login**: Registered users can log in with their credentials.
- **Profile Update**: Users can update their password, profile image, and self-introduction.
- **Rich Text Self-Introduction**: The self-introduction field supports rich text formatting (bold, italics, links) using Quill.
- **Homepage**: Once logged in, users can view their profile information, profile image, and self-introduction on their homepage.

## How to Use

1. **Setup**: Ensure you have XAMPP or any local server with PHP support, as well as SQLite enabled.

2. **Database Setup**:
   - This project uses SQLite, which automatically creates a `user_db.sqlite` file in the project folder upon first connection.
   - The `db.php` file handles database connection and ensures the necessary `users` table is created if it doesn't exist.

3. **Running the Project**:
   - Place the project files in your server’s root directory (e.g., `htdocs` folder in XAMPP).
   - Start the server and open the browser at `http://localhost/project_folder_name`.

4. **User Registration**:
   - Go to the `register.php` page to create a new account.
   - Fill in the username, email, password, upload an optional profile image, and write a self-introduction in the rich text editor.
   - Submit the form to register.

5. **Login**:
   - Go to `login.php` to log in with your registered username and password.
   - Upon successful login, you’ll be redirected to your homepage (`home.php`).

6. **Profile Update**:
   - On your homepage, click "Edit Profile" to navigate to `profile.php`.
   - Here, you can update your password, change your profile image, and edit your self-introduction using the rich text editor.

7. **Logout**:
   - Click "Logout" on the homepage to log out of your account.

## Notes

- **Image Uploads**: Uploaded images are stored in the `uploads` folder in the project directory.
- **Rich Text Editor**: The self-introduction field on both `register.php` and `profile.php` uses Quill, allowing users to add formatted text.