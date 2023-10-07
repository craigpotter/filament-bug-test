# Filament Bug Test

## Installation and testing
- Clone this repository
- `composer install`
- Create a database and add the credentials to your `.env` file copied over from `.env.example`
- `php artisan migrate --seed`
- `php artisan serve`
- Visit `localhost:8000/admin/login` and login with the credentials `test@example.com` and `password`
- Visit the user resource and edit the existing user. 
- Add lotto numbers which will fail the validation. e.g String or numbers greater than 49.
- Save the user and you will see no validation errors.

## Optional Debugging
- Checkout the `debug` branch and repeat the testing steps above.
- The views have been published and some dumps have been added.

## Expected Behaviour
- Validation errors should be displayed on the page.
