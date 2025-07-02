# Laravel Quote Management API Project

Allows users to fetch random quotes from an external API, save their favorites, and manage them via CRUD operations with proper authentication.

## Setup Instructions

### I'm using:

- PHP 8.4.3
- Laravel Framework 12.2.0
- Composer 2.8.6
- MySQL (Port 8889) Ver 8.0.40 for macos12.7 on arm64 (Source distribution)
- MAMP Pro

## Installation Steps

### 1. Clone this repository to your local machine:

```bash
git clone https://github.com/sereitepy/laravel-quote-management.git
cd quote-management
```

### 2. My `.env` file: according to what my MAMP settings are.

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=8889
DB_DATABASE=quote-management
DB_USERNAME=root
DB_PASSWORD=
DB_SOCKET=/Applications/MAMP/tmp/mysql/mysql.sock
```

### 3. Run database migrations:

```bash
php artisan migrate
```

## Key Markdown Formatting Tips:

- Use `#` for main headings, `##` for subheadings, `###` for sub-subheadings
- Use `-` or `*` for bullet points (both work the same)
- Use numbered lists with `1.`, `2.`, etc.
- Wrap code in backticks `` ` `` for inline code
- Use triple backticks ``` for code blocks
- Add language name after opening ``` for syntax highlighting (e.g., ```bash, ```php)
- Use **bold** or __bold__ for emphasis
- Use *italic* or _italic_ for italics

## Additional Sections You Might Want:

### Features
- User authentication
- Quote management (CRUD operations)
- External API integration
- Favorite quotes system

### Requirements
- PHP >= 8.1
- Composer
- MySQL/MariaDB
- Web server (Apache/Nginx)

### Usage
After installation, you can:
1. Register a new account
2. Browse random quotes
3. Save favorites
4. Manage your quote collection

### API Endpoints
- `GET /api/quotes` - Fetch random quotes
- `POST /api/quotes/favorite` - Save favorite quote
- `GET /api/user/favorites` - Get user's favorites
- `DELETE /api/favorites/{id}` - Remove favorite

### Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
