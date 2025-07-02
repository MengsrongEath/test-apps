# My Awesome Project

A simple web application that demonstrates CRUD operations with user authentication and API integration.

## Features

- User registration and login
- Create, read, update, and delete operations
- RESTful API endpoints
- Responsive design
- Database integration

## Technologies Used

- **Backend**: PHP 8.4.3
- **Framework**: Laravel 12.2.0
- **Database**: MySQL 8.0.40
- **Package Manager**: Composer 2.8.6
- **Development Environment**: MAMP Pro
- **Frontend**: HTML, CSS, JavaScript

## Prerequisites

Before you begin, ensure you have the following installed:

- PHP >= 8.1
- Composer
- MySQL or MariaDB
- A web server (Apache/Nginx)
- Git

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/your-project-name.git
cd your-project-name
```

### 2. Install dependencies

```bash
composer install
npm install
```

### 3. Environment setup

Copy the example environment file and configure it:

```bash
cp .env.example .env
```

Update your `.env` file with your database credentials:

```env
APP_NAME="My Awesome Project"
APP_ENV=local
APP_KEY=
APP_DEBUG=true
APP_URL=http://localhost

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=your_username
DB_PASSWORD=your_password
```

### 4. Generate application key

```bash
php artisan key:generate
```

### 5. Run database migrations

```bash
php artisan migrate
```

### 6. Seed the database (optional)

```bash
php artisan db:seed
```

### 7. Start the development server

```bash
php artisan serve
```

Your application will be available at `http://localhost:8000`

## Usage

### Basic Operations

1. **Registration**: Visit `/register` to create a new account
2. **Login**: Use `/login` to access your account
3. **Dashboard**: Navigate through the main interface
4. **CRUD Operations**: Create, view, edit, and delete records

### API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/items` | Get all items |
| POST | `/api/items` | Create new item |
| GET | `/api/items/{id}` | Get specific item |
| PUT | `/api/items/{id}` | Update item |
| DELETE | `/api/items/{id}` | Delete item |

### Example API Usage

```bash
# Get all items
curl -X GET http://localhost:8000/api/items

# Create a new item
curl -X POST http://localhost:8000/api/items \
  -H "Content-Type: application/json" \
  -d '{"name": "Sample Item", "description": "This is a test item"}'
```

## Configuration

### Database Configuration

For MAMP users, your database settings might look like:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=8889
DB_DATABASE=your_database
DB_USERNAME=root
DB_PASSWORD=
DB_SOCKET=/Applications/MAMP/tmp/mysql/mysql.sock
```

### Mail Configuration

To enable email features:

```env
MAIL_MAILER=smtp
MAIL_HOST=smtp.gmail.com
MAIL_PORT=587
MAIL_USERNAME=your-email@gmail.com
MAIL_PASSWORD=your-app-password
MAIL_ENCRYPTION=tls
```

## Testing

Run the test suite:



- Thanks to the Laravel community
- Inspiration from various open-source projects
- Special thanks to contributors

---

⭐ If you found this project helpful, please give it a star on GitHub!
