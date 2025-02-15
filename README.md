# Blog Website Project

## Overview
This project is a dynamic blog website where users can browse articles, search for content, create an account, and write an article. Users can also perform CRUD opertaions on their uploaded articles under POST section , sort content by date, and subscribe to a newsletter.

## Features
### 1. Homepage
- Displays all blog articles as **thumbnails** (each with a title and an image).
- Pagination system to navigate through multiple pages.
- Search bar to find articles by title or content.
- Sorting options (Newest First, Oldest First).
- **Newsletter Subscription:** A field in the footer where users can subscribe to receive updates.


### 2. Article Page
- Displays the **full content** of a selected article dynamically.
- Shows three **related articles** as thumbnails for further reading.

### 3. Article Management
- Articles are manually written and stored in a **MySQL database**.
- Images are stored in the project folder, with their file paths saved in the database.
- Users with an account can create new articles using a **submission form**.

### 4. User Authentication System
- **Sign-up** (Registration) and **Login** (Authentication).
- Secure password handling with hashing.
- **account Page** where users can upload an article and perform CRUD operations on  their posts (uploaded articles will be displayed in their account under the section POST) and manage their content.

## Technologies Used
- **Frontend:** HTML5, CSS3 
- **Backend:** PHP (for user authentication, article management)
- **Database:** MySQL (stores user data, articles, and image paths)

## Installation & Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/blog-project.git
   ```
2. Set up a local server (e.g., XAMPP, WAMP, or MAMP).
3. Import the SQL database:
   ```sh
   mysql -u root -p database_name < blog_database.sql
   ```
4. Configure database settings in `config.php`.
5. Start your local server and access the project via `http://localhost/blog-project`.

## Future Improvements
- **Reset Password:** Generates a unique token (e.g., `bin2hex(random_bytes(32))`) and stores it in the database to allow users to reset their passwords securely.
- **Newsletter Subscription:** A field in the footer where users can subscribe to receive updates.
- Implement a comment section for articles.
- Add a category/tag system for better content filtering.
- Improve user profile customization options.
- Enable image uploads for articles.

## Contributors
- **muhisina** – Developer

## License
This project is open-source and available under the [MIT License](LICENSE).

