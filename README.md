# Laravel 12 Project

A Laravel 12 web application using MySQL as the database.

## Table of Contents
- [Requirements](#requirements)
- [Setup & Installation](#setup--installation)
- [Configuration](#configuration)
- [Database Setup](#database-setup)
- [Running the Project](#running-the-project)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

---

## Requirements

- PHP 8.1 or higher
- Composer
- MySQL
- Node.js & NPM (optional, if using front-end tooling)

---

## Setup & Installation

Follow these steps in order:

### 1. Clone the repository

```bash
git clone <your-repository-url> project
cd project
```

### 2. Install PHP dependencies

```bash
composer install
```

### 3. Install front-end dependencies (if your project uses them)

```bash
npm install
npm run dev
```

### 4. Copy the environment file

```bash
cp .env.example .env
```

**Windows CMD:**
```cmd
copy .env.example .env
```

### 5. Generate the application key

```bash
php artisan key:generate
```

---

## Configuration

Open `.env` and set your MySQL credentials:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=your_mysql_username
DB_PASSWORD=your_mysql_password
```

---

## Database Setup

### 1. Create the database (if not already created)

```sql
CREATE DATABASE your_database_name;
```

### 2. Run migrations to create tables

```bash
php artisan migrate
```

### 3. (Optional) Seed the database with sample data

```bash
php artisan db:seed
```

---

## Running the Project

Start the development server:

```bash
php artisan serve
```

Open your browser at: **http://127.0.0.1:8000**

---

## Project Structure

```
app/         - Core application logic
routes/      - Web, API, and console routes
resources/   - Views, CSS, JS
database/    - Migrations and seeders
public/      - Public assets
```

---

## Contributing

1. Fork the repository
2. Create a new branch:
   ```bash
   git checkout -b feature/my-feature
   ```
3. Make changes
4. Commit changes:
   ```bash
   git commit -m "Add new feature"
   ```
5. Push to your branch:
   ```bash
   git push origin feature/my-feature
   ```
6. Open a Pull Request

---

## License

MIT License
