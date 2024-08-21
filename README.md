# Go & TypeScript Fullstack Template

This repository provides a template for building full-stack applications using Go for the backend and TypeScript (with React) for the frontend. It is designed to help developers quickly start building robust applications by providing a pre-configured project structure and essential dependencies.

## Features

- **Backend**: 
  - Built with Go
  - RESTful API
  - Basic authentication and JWT support
  - Database integration with PostgreSQL (can be configured for other databases)
  - Modular structure for easy scalability

- **Frontend**:
  - Built with TypeScript and React
  - State management using Redux or Context API
  - Routing using React Router
  - Styled Components for styling
  - API integration with the backend

## Prerequisites

- **Go**: version 1.18 or higher
- **Node.js**: version 14 or higher
- **npm** or **yarn**: for managing frontend dependencies
- **Docker** (optional): for containerization
- **PostgreSQL** (or any other preferred database)

## Project Structure

```bash
├── backend
│ ├── main.go # Main entry point for the Go backend
│ ├── api # API handlers
│ ├── models # Data models and database schema
│ ├── services # Business logic and service layer
│ └── config # Configuration files (e.g., env variables)
│
└── frontend
├── src
│ ├── components # React components
│ ├── pages # Different pages of the application
│ ├── store # State management setup
│ └── App.tsx # Main entry point for the React frontend
└── public # Static assets like images, icons, etc.
```

## Getting Started

### Cloning the Repository

```bash
git clone https://github.com/LSP20xx/go-ts-template.git
cd go-ts-template
```

Setting Up the Backend

    Navigate to the backend directory:
```bash
cd backend
```

Install Go dependencies:

```bash
go mod tidy
```

Run the backend server:

```bash
go run main.go
```

Setting Up the Frontend

    Navigate to the frontend directory:
```bash
cd frontend
```
Install Node.js dependencies:

```bash
npm install
# or
yarn install
```

Run the frontend development server:

```bash
npm start
# or
yarn start
```

Running the Application

Once both servers are running, you can access the application by navigating to http://localhost:3000 in your web browser.
Running Tests

Backend:

```bash
go test ./...
```

Frontend:

```bash
npm test
# or
yarn test
```

Docker Support

If you prefer to run the application in a Docker container, you can use the provided Dockerfile and docker-compose.yaml (if applicable).

Build and run the Docker containers:

```bash
docker-compose up --build
```

Contributing

Feel free to fork this repository and submit pull requests. All contributions are welcome!
License

This project is licensed under the MIT License. See the LICENSE file for more details.