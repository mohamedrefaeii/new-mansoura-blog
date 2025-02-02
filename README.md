# New Mansoura Project - Simple Blogging System

This is a simple blogging system built using Laravel, allowing users to create, edit, and delete blog posts. It provides basic CRUD (Create, Read, Update, Delete) functionality for managing articles.

## Features
- **Home Page:** Displays a list of all blog posts.
- **Post Management:** Users can create, edit, update, and delete posts.
- **Post Details:** View individual blog posts.
- **Authentication:** User login and registration for managing posts (using Laravel UI package).
- **Database Integration:** Uses migration files to store blog posts.
- **Validation:**
  - Title & description are required.
  - Minimum length for title: 3 characters (must be unique).
  - Minimum length for description: 10 characters.
  - Validation errors are displayed appropriately.
- **Bonus Features:**
  - Formatted timestamps using Carbon.
  - PostSeeder & PostFactory to generate 500 sample posts.
  - Pagination on the index page.

---

## Installation
### 1. Clone the Repository
```sh
 git clone https://github.com/yourusername/new-mansoura-blog.git
 cd new-mansoura-blog
```

### 2. Install Dependencies
```sh
 composer install
 npm install && npm run dev
```

### 3. Configure Environment Variables
Copy the `.env.example` file and update database credentials:
```sh
 cp .env.example .env
```

### 4. Generate Application Key
```sh
 php artisan key:generate
```

### 5. Run Migrations & Seed Data
```sh
 php artisan migrate --seed
```

### 6. Run the Application
```sh
 php artisan serve
```
Now, visit `http://127.0.0.1:8000` in your browser.

---

## Usage
1. Register or log in.
2. Create a new blog post.
3. Edit or delete your posts.
4. View posts on the homepage.

---

## Bonus Features
- **Formatted timestamps:** Uses Carbon for human-friendly dates.
- **Seeder & Factory:** Run `php artisan db:seed` to generate 500 posts.
- **Pagination:** Displays paginated results on the index page.

---

## Technologies Used
- Laravel (PHP Framework)
- Laravel UI (Authentication)
- MySQL (Database)
- Bootstrap (Frontend Styling)
- Carbon (Date Formatting)

---

## Contribution
Feel free to fork this repository, submit issues, or create pull requests.

---

## License
This project is open-source and available under the [MIT License](LICENSE).

