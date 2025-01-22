# Category-Product CRUD Application

This is a Spring Boot application that implements CRUD operations for Categories and Products with a one-to-many relationship. It uses MySQL as the database, JPA and Hibernate for ORM, and provides server-side pagination for efficient data retrieval.

## Features

- **Category CRUD Operations**:
  - Create, Read, Update, and Delete categories.
  - Paginated listing of categories.

- **Product CRUD Operations**:
  - Create, Read, Update, and Delete products.
  - Paginated listing of products.
  - Products are linked to categories via a one-to-many relationship.

- **Database**: MySQL
- **ORM**: JPA and Hibernate

## API Endpoints

### Category Endpoints

- `GET /api/categories?page={page}`: Get paginated list of categories.
- `POST /api/categories`: Create a new category.
- `GET /api/categories/{id}`: Get a category by ID.
- `PUT /api/categories/{id}`: Update a category by ID.
- `DELETE /api/categories/{id}`: Delete a category by ID.

### Product Endpoints

- `GET /api/products?page={page}`: Get paginated list of products.
- `POST /api/products`: Create a new product.
- `GET /api/products/{id}`: Get a product by ID (includes category details).
- `PUT /api/products/{id}`: Update a product by ID.
- `DELETE /api/products/{id}`: Delete a product by ID.

