# Books
Graphql API for a books catalog application created with [Django](https://www.djangoproject.com/), [Graphene](https://graphene-python.org/) and [SQLite](https://www.sqlite.org/index.html).

It has the following route to access the Graphql endpoints:
- `GET /graphql` - Graphql endpoints

In addition, as it is also a REST API, it has the following endpoints:
- `POST /api/v1/books` - Create a new book
- `GET /api/v1/books` - Get all books
- `GET /api/v1/books/<id>` - Get a specific book
- `PUT /api/v1/books/<id>` - Update a whole book
- `PATCH /api/v1/books/<id>` - Update specific fields of a book
- `DELETE /api/v1/books/<id>` - Delete a book

## Installation
1. Clone the repository
2. Run `python3 -m venv venv`
3. Run `source venv/bin/activate`
4. Run `pip3 install -r requirements.txt` to install the dependencies
5. Run `python3 manage.py migrate` to run the migrations
6. Run `python3 manage.py runserver` to run the server
7. Go to <a>http://localhost:8000 to see the server running
8. Go to <a>http://localhost:8000/graphql to see the Graphql playground


## Database migrations
1. Run `python3 manage.py makemigrations` to create a new migration file
2. Run `python3 manage.py migrate` to apply the migrations
3. Run `python3 manage.py showmigrations` to see the migration history
4. Run `python3 manage.py migrate <app_name> zero` to revert all migrations of an app
5. Run `python3 manage.py migrate zero` to revert all migrations