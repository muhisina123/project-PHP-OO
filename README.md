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
click on the  user profile icon  next to the search bar) for registration
- **Sign-up** (Registration) and **Login** (Authentication).
- Secure password handling with hashing.
- **account Page** where users can upload an article and perform CRUD operations on  their posts (uploaded articles will be displayed in their account under the section POST) and manage their content.
- User Profile Page:
1)Users can create and post articles.
2)Users can edit or delete their own articles.
- 

## Technologies Used
- **Frontend:** HTML5, CSS3 
- **Backend:** PHP (for user authentication, article management)
- **Database:** MySQL (stores user data, articles, and image paths)

## Database Structure
The database is named `bloggers` and contains two tables:

### 1. `blogs` Table
This table stores manually added articles.

| Column Name | Data Type | Description |
|------------|-----------|-------------|
| id         | INT (AUTO_INCREMENT) | Primary key |
| photo      | VARCHAR(255) | Path to article image |
| title      | VARCHAR(255) | Article title |
| description| TEXT | Article content |
| user_id    | INT    | user id  |


when new user creates an article , the id from the blogger table is added to the blog table for that particular article under user_id

### 2. `bloggers` Table
This table stores information about users who create accounts and post articles.

| Column Name | Data Type | Description |
|------------|-----------|-------------|
| id         | INT (AUTO_INCREMENT) | Primary key |
| username   | VARCHAR(255) | Blogger's username |
| email      | VARCHAR(255) | Blogger's email |
| password   | VARCHAR(255) | Hashed password |


## Installation & Setup
1. Clone this repository:
   ```sh
   git clone https://github.com/your-username/your-repo.git
   ```
2. Navigate to the project folder:
   ```sh
   cd your-repo
   ```
3. Set up the database:
   - Import the SQL file (`database.sql`) into MySQL.
   - Configure the database connection in your backend files.
4. Start the project using a local server (e.g., XAMPP, WAMP, or a custom PHP server).
5. Open the website in a browser and explore the features!


## Screenshots
(Add screenshots here showing different pages of your project.)




## Installation & Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/blog-project.git
   ```
2. Set up a local server (e.g., XAMPP, WAMP, or MAMP).
3. Import the SQL database:
   ```sh
   mysql -u root -p database_name < bloggers.sql
   ```
4. Configure database settings in `config.php`.
5. Start your local server and access the project via `http://localhost/project_name`.

## Future Improvements
- **Reset Password:** Generates a unique token (e.g., `bin2hex(random_bytes(32))`) and stores it in the database to allow users to reset their passwords securely.
- **Newsletter Subscription:** A field in the footer where users can subscribe to receive updates.
- Implement a comment section for articles.
- Add a category/tag system for better content filtering.
- Improve user profile customization options.

## Contributors
- **muhisina** – Developer

## License
This project is open-source and available under the [MIT License](LICENSE).




