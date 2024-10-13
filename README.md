# Testem API

Testem is an API for a quiz application. This API provides endpoints for managing users, admins, instructors, students, and tests.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Environment Variables](#environment-variables)
- [License](#license)

## Installation

1. Clone the repository:

```sh
git clone https://github.com/Almuhanad-1/testem-api
cd testem-api
```

2. Install dependencies:

```sh
npm install
```

3. Set up environment variables by creating a `.env` file in the root directory. Refer to the [Environment Variables](#environment-variables) section for required variables.

4. Run database migrations:

```sh
npx sequelize-cli db:migrate
```

## Usage

To start the server, run:

```sh
npm start
```

The server will start on the port specified in the environment variables or default to port 3000.

## API Endpoints

### Admin Routes

- `GET /api/v1/admin/...`

### User Routes

- `GET /api/v1/users/...`

### Instructor Routes

- `GET /api/v1/instructors/...`

### Student Routes

- `GET /api/v1/students/...`

### Test Routes

- `GET /api/v1/tests/...`

Refer to the specific route files for detailed endpoint information:

- `lib/admins/routes`
- `lib/users/routes`
- `lib/instructors/routes`
- `lib/students/routes`
- `lib/tests/routes`

## Environment Variables

The following environment variables are required:

- `PORT`: The port on which the server will run (default: 3000).
- `DATABASE_URL`: The database connection string.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
