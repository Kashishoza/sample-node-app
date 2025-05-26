# Sample Node App

This is a simple Node.js application used to demonstrate CI/CD pipelines with GitHub Actions and Docker.

## Features

- Basic HTTP server using Node.js
- Dockerized for easy deployment
- Automated CI/CD workflow with GitHub Actions

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or above)
- [npm](https://www.npmjs.com/)
- [Docker](https://www.docker.com/) (optional, for containerization)

### Installation

1. Clone the repository or copy this folder.
2. Install dependencies:

   ```sh
   npm install
   ```

### Running Locally

Start the server:

```sh
npm start
```

The server will run on [http://localhost:3000](http://localhost:3000).

### Running with Docker

Build the Docker image:

```sh
docker build -t sample-node-app .
```

Run the Docker container:

```sh
docker run -p 3000:3000 sample-node-app
```

## CI/CD

This project includes a GitHub Actions workflow for:

- Installing dependencies
- Running tests
- Building and pushing a Docker image to Docker Hub

See [`.github/workflows/main.yml`](.github/workflows/main.yml) for details.
