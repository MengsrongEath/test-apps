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

```bash
# Run all tests
php artisan test

# Run specific test file
php artisan test tests/Feature/ExampleTest.php

# Run tests with coverage
php artisan test --coverage
```

## Troubleshooting

### Common Issues

1. **Permission errors**: Make sure storage and cache directories are writable
   ```bash
   chmod -R 775 storage bootstrap/cache
   ```

2. **Database connection failed**: Check your `.env` database credentials

3. **Composer dependencies**: Clear and reinstall if needed
   ```bash
   composer clear-cache
   composer install
   ```

4. **Application cache**: Clear Laravel caches
   ```bash
   php artisan cache:clear
   php artisan config:clear
   php artisan route:clear
   ```

## Contributing

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Changelog

### Version 1.2.0 (2024-12-15)
- Added user authentication
- Implemented API endpoints
- Fixed database migration issues

### Version 1.1.0 (2024-12-01)
- Added CRUD operations
- Improved UI design
- Bug fixes and performance improvements

### Version 1.0.0 (2024-11-15)
- Initial release
- Basic functionality implemented

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

- **Author**: Your Name
- **Email**: your.email@example.com
- **GitHub**: [@yourusername](https://github.com/yourusername)
- **Website**: [yourwebsite.com](https://yourwebsite.com)

## Acknowledgments

- Thanks to the Laravel community
- Inspiration from various open-source projects
- Special thanks to contributors

---

⭐ If you found this project helpful, please give it a star on GitHub!
