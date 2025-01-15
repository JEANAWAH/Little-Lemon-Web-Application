# Little-Lemon-Web-Application
This is a final project for Meta-backend professional certificate

# Little Lemon Restaurant API

This project is a Django-based API for managing menu items and table bookings for Little Lemon Restaurant. It connects to a MySQL database and supports user registration, authentication, and CRUD operations for menu items and bookings.

## Installation
1. Clone the repository:
   git clone https://github.com/JEANAWAH/Little-Lemon-Web-Application.git
2. Activate the virtual environment:
   pipenv shell
3. Install dependencies:
   pipenv install
4. Perform migrations:
   python manage.py makemigrations
   python manage.py migrate
5. Run the server:
   python manage.py runserver

## API Endpoints
### User Management
- **POST /api/auth/users/**: Register a new user.
- **POST /api/auth/token/login/**: Log in to retrieve an auth token.
- **GET /api/auth/users/me/**: Get current user details.

### Menu Management
- **GET /api/menu-items/**: List all menu items.
- **POST /api/menu-items/**: Add a new menu item (requires authentication).
- **PUT/PATCH/DELETE /api/menu-items/{id}/**: Update/delete a menu item (requires authentication).

### Booking Management
- **GET /api/bookings/**: List all bookings for a specific date.
- **POST /api/bookings/**: Create a new booking.

## Testing
You can test the APIs using the Insomnia REST client. Import the provided Insomnia workspace and test the endpoints.

## Unit Tests
Run the following command to execute the unit tests:
python manage.py test
