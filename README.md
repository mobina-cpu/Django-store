# Django Store

This project is a Django-based store application that provides functionality for managing products, categories, and shopping carts.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.9 or higher
- Pipenv installed for managing dependencies
- A running MySQL database

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/mobina-cpu/Django-store.git
   cd Django-store
   ```

2. Install the required dependencies:

   ```bash
   pipenv install
   ```

3. Create a `.env` file in the project root and add your environment variables, including your database settings.

## Running the Application

### Running the Development Server

To start the development server, run:

```bash
 python manage.py runserver
```

### Running Celery

To run Celery for handling background tasks, open a new terminal and execute:

```bash
 celery -A storefront worker --loglevel=info
```

### Generating Sample Data

To generate sample data, you can run the following command:

```bash
 python manage.py seed_db
```

## Running Tests

To run the tests, execute:

```bash
 python manage.py pytest
```

