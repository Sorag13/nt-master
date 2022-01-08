# Project template

Template already has [`breeze`](https://laravel.com/docs/8.x/starter-kits#laravel-breeze-installation) installed.



## Setup

1. Copy `.env.example` and create `.env`
2. In `.env` fill these field:
   - DB_PORT (if needed)
   - DB_DATABASE
   - DB_USERNAME
   - DB_PASSWORD
3. Install composer packages:
```
composer install
```
4. Generate application key:
```
php artisan key:generate
```
5. Run migrations:
```
php artisan migrate
```

## Templates

Template already using Tailwind CSS and AlphineJS loading from CDN.

If needed add custom CSS or use already defined classes https://tailwindcss.com/

If needed add custom JS or use https://alpinejs.dev

For layouts use:
- `layouts/app.blade.php`
- `layouts/guest.blade.php`

Examples how to use the templates:
- `views/dahsboard.blade.php` - `app.blade.php` layout example
- `views/auth/login.blade.php` - `guest.blade.php` layout example

Advice try structure application in pages by folder:
- `view/product/index.blade.php` (Product list page)
- `view/product/create.blade.php` (Product create form page)
- `view/product/edit.blade.php` (Product edit form page)
- `view/product/show.blade.php` (Product show form page)


## Seeders

Currently there is only one seeder:
- `database/seeders/CreateAdminUser.php` - it creates admin user

To run seeders use command:
```
php artisan db:seed
```

### Seeded admin user credentials

Email: admin@admin.test

Password: secret
