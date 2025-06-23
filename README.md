# airbnb-clone-project


## Team Roles
This is an airbnb-clone-project built with python
Backend Developer: Responsible for implementing API endpoints, database schemas, and business logic.
Database Administrator: Manages database design, indexing, and optimizations.
DevOps Engineer: Handles deployment, monitoring, and scaling of the backend services.
QA Engineer: Ensures the backend functionalities are thoroughly tested and meet quality standards.

## Technology Stack

- Django: A high-level Python web framework used for building the RESTful API.
- Django REST Framework: Provides tools for creating and managing RESTful APIs.
- PostgreSQL: A powerful relational database used for data storage.
- GraphQL: Allows for flexible and efficient querying of data.
- Celery: For handling asynchronous tasks such as sending notifications or processing payments.
- Redis: Used for caching and session management.
- Docker: Containerization tool for consistent development and deployment environments.
- CI/CD Pipelines: Automated pipelines for testing and deploying code changes.

## Database Design
- Users

Represents individuals using the platform, either as property owners or renters.


Relationships:

A user can own multiple properties.

A user can make multiple bookings.

A user can leave multiple reviews.

- Properties

Represents property listings on the platform.


Relationships:

   A property belongs to one user (the owner).

   A property can have many bookings and reviews.

- Bookings

Tracks reservations made by users for properties.

Relationships:

  A booking belongs to one user and one property.

  A booking can have an associated payment.

- Payments

Handles transactions for bookings.

Relationships:

  A payment belongs to one booking.

- Reviews

User-generated reviews for properties.


Relationships:

  A review is associated with one user and one property.

